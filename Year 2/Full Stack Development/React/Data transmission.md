Created: Mar 23 2026
Class: [[Full stack development]] 
- - -
# Child -> Parent
Pass setState function as prob to child
```ts
const [state, setState] = useState(0)

<Child set={setState}/>

- - -
  
function Child({set}) {
	set(10);
}
```

# Sibling -> Sibling
useContext. Makes variables defined in context global for all components within context
```ts
import { createContext, useContext, ReactNode } from "react";

type ObjContext
{
	field1: number,
	field2, number
}

const _Context = createContext<ObjContext | undefined>(undefined);


type ContextProviderProps = {
  children: ReactNode;
  value: ObjContext;
};

export function ContextProvider({ children, value }: ContextProviderProps) {
  return (
    <_Context.Provider value={value}>{children}</_Context.Provider>
  );
}

export function useCounter() {
  const context = useContext(_Context);
  if (context === undefined) {
    throw new Error("");
  }
  return context;
}

- - - 
import { ContextProvider } from "../context/Context";
<ContextProvider value={{ count, increment, decrement }}>
	<Child />
	<Child />
	<Child />
	<Child />
</ContextProvider>
  
```