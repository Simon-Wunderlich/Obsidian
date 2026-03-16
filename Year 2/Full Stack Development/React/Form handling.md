Created: Mar 16 2026
Class: [[Full stack development]] 
- - -
```ts
// Define form data obj
interface FormData {
	field1: string,
	field2: number
}

function Component() {
	const [formData, setFormData] = useState<FormData | null>(null);
	
	// Update form data on change
	const handleChange = (e : HTMLInputElement) {
		const {name, value} = e.target;
		setFormData((prevState) => {
			...prevState,
			[name]: value
		});
	};
	
	const submit = (e: FormEvent) => {
		console.log(formData)
	};
	
	return (
	<form onSubmit={submit()}>
		<input 
		required 
		name="field1"
		onChange={handleChange}/>
	<form onSubmit={submit()}>
		<input 
		required 
		name="field2"
		type: number
		onChange={handleChange}/>
	</form>
	
	);
}
```
