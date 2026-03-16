```js
// Define db
const db = new Dexie("dataBaseName");

db.version(1).stores({
	table1: "++id, field1, field2"
});

//Queries
await db.table1.add({
	field1: "a",
	field2: 3
});

const val = await db.table1
				.where("field1").above(4)
				.toArray();
```