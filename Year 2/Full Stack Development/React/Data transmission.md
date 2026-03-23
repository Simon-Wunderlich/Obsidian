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
[[useContext]]. Makes variables defined in context global for all components within context
