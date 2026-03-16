Created: Mar 16 2026
Class: [[Full stack development]] 578025957424758785
- - -
```ts
const [state, setState] = useState<int | null>(null);
console.log(state); // null

setState(5);
console.log(state); // 5

setState(prev => prev + 1)
console.log(state); // 6

const [obj, setObj] = userState<Obj>(Obj);
setObj(prevState => (
	...prevState, // Copies old fields of prevState
	field1: prevState + 1 // Overrides field1
	));
```
