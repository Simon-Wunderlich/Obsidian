Created: Mar 23 2026
Class: [[Full stack development]] 
- - -
Pass setState function as prob to child
```ts
const [state, setState] = useState(0)

<Child set={setState}/>

- - -
  
function Child({set}) {
	set(10);
}
```