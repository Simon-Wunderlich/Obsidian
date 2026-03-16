Created: Mar 08 2026
Class: [[Software engineering fundamentals]] 
- - -
Must include:
- Specification
	- Defining what the system should do
- Design and implementation
	- Defining the organisation of the system and implementing the system
- Validation
	- Checking that it does what the customer wants
- Evolution 
	- Changing the system in response to changing customer needs

# Types of development process
## Waterfall
#### Description
Plan driven
Separate and sequential phases for 
	- Specification
	- Design and implementation
	- Validation
	- Evolution 
![[Pasted image 20260308125045.png]]
#### Disadvantages
- Impossible to know all requirements up front 
	- Especially for large systems
- Not flexible to changing requirements
- Users don’t know what they want until they see it
	- Not true in all cases
- Design risks difficult to identify before implementation
- Ineffective resource utilisation
	- Employees unable to start work until current phase is complete
- Issues from previous phases affect later phases


## Iterative and incremental
#### Description
Plan driven / Agile
Specification development and validation are interweaved
Delivery is broken into increments
Iterations between 2-6 weeks
##### Timeboxing
- Iterations are fixed in length with set deadlines to ensure iterations don't go on too long and cause scope creep and diverge from stakeholders' needs. If unable to meet deadline, descope to ensure you have an executable product at the end of the iteration
![[Pasted image 20260308125741.png]]
#### Benefits
- Less project failure, better productivity and lower defect rates
- Early mitigation of high risks
- Early feedback to align more closely with stateholders' needs

# Design process
![[Pasted image 20260308132104.png]]
#### Design activities
- Architectural design
	- Identify overall structure
	- Principle components 
		- Relationships
		- Distributions
- Database design
	- System data structures
	- How to represent in database
- Interface design
	- Define interfaces between components
- Component selection and design
	- Search for reusable components
		- If unavailable, design how it will operate
		
![[Pasted image 20260314180907.png]]