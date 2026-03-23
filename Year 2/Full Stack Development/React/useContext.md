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