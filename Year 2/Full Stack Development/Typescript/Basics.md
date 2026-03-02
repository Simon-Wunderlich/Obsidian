Created: Mar 02 2026
Class: [[Full stack development]] 
- - -
# Types
- string
- number
	- Can support ints and floats, auto converts hex, binary and octals
- bigint
	- for numbers > $2^{53}-1$
- boolean
- Symbols
	- Creates unique identifiers for dict
	- let sym: Symbol = Symbol('description);
```ts
let var:type = value;
```

## Unions
```ts
// Type union
type type1 = number | string;
const var1: type1 = 10;
const var2: type1 = "hello"; 

// Value union (kinda just an enum but worse)
type Status = "success" | "error";  
let response: Status = "success";
```
# Special types
## Any
```ts
let v: any = true;  
v = "string"; // no error as it can be "any" type  
Math.round(v); // no error as it can be "any" type
```

## Undefined / null
```ts
let var1: null = null;
let var2: undefined = undefined;
```

# Functions
```ts
function (a: type, b: type) {
	return a;
}
```
# Interfaces
```ts
interface A {
	var1: type;
	readonly var2: type; //Readonly (const)
	var3?: type; //Optional
}
let a:A = {var1: value, var2:value, var3:value};
```
# Collections
## Array
```ts
let arr:type[] = [value1, value2];
```
## Tuple
```ts
let arr: [type1, type2] = [ value1, value2 ]; //order of items is important
```
## Hashmap
```ts
let hashmap : Map<keyType, valueType> = new Map();
hashmap.set(key1, value1);
hashmap.get(key1); // returns value1
hashmap.has(key1); // check key1 exist
hashmap.delete(key1);
hashmap.size(); // return 1
hashmap.clear();
```
## Object
```ts
const obj: { field1: type1, field2: type2} = {
	field1: val1,
	field2: val2
};

// Dynamic fields
const obj2: { [ index : string ] : type } = {};
obj2.field3 = val3;
```


