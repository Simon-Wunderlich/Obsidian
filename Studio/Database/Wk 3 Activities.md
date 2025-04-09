Created: Apr 09 2025
Class: [[Database]]
- - -
#### Describe in your own words the following concepts:
- ##### Strong entities
	- An entity which can stand alone
	- Unique primary key
- ##### Weak entities
	- An entitiy that is dependant on another entitiy
	- No primary key, only partial key

#### Describe in your own words the following concepts: 

- Simple attributes
	- Stores single value
- Composite attributes
	- Groups multiple different attributes 
- Multi-valued attributes
	- Store multiple values for the same attribute
- Relationship attributes
	- Defines extra info abt a relationship between entities

### Multiplicity
#### Describe in your own words the following concepts: 
- Cardinality
	- The highest number of possible relationships for a given entity
- Participation
	- The lowest number of possible relationships for a given entity
{Participation}..{Cardinality}
ie
{Minimum}..{Maximum}

![[Pasted image 20250409112234.png]]
The entity closest to the multiplicity is what the relationship is relating to. Imaging arrows at the end
eg
The department is managed by 1 to 1 employees as shown in the diagram
An employee is manages 0 to 1 departments

![[Pasted image 20250409114703.png]]