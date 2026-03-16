Created: Mar 16 2026
Class: [[Full stack development]] 
- - -
```ts
interface FormData {
	field1: string
}

const [formData, setFormData] = useState<FormData | null>(null);
const handleChange = (e) {
	const {name, value} = e.target;
	setFormData((prevState) => {
		...prevState,
		[name]: value
	});
};
const submit = () => {
	console.log(formDat)
};
return (
<form onSubmit={submit()}>
	<input 
	required 
	name="input1"
	onChange={handleChange}/>
</form>
)
```