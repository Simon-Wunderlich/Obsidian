Created: Mar 23 2026
Class: [[Full stack development]] 
- - -
```ts
import { useState, useEffect, SetStateAction } from "react";

export function useLocalStorage<T>(
  key: string,
  initialValue: T
): [T, (value: SetStateAction<T>) => void] {
	const [storedValue, setStoredValue] = useState<T>(initialValue);
	
	 const setValue = (value: SetStateAction<T>) => {
	   setStoredValue(value);
	 };
	 return [storedValue, setStoredValue];
}
```

