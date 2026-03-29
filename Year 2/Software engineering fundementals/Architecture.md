Created: Mar 24 2026
Class: [[Software engineering fundamentals]] 
- - -
Link between design and requirements engineering
Describes how the system is organised as a set of communicating components

- Decompose software into modules with interfaces
- Specify high-level behaviour, interactions, and non-functional properties
- Consider key trade offs
	- Schedule vs. Budget
	- Cost vs. Robustness
	- Fault Tolerance vs. Size
	- Security vs. Speed
- Maintain a record of design decisions and traceability

# Components
• A component is a unit of computation or a data store.
• Components
	- Clients
	- Servers
	- Databases
	- Filters
	- Layers
	- Abstract Data Types (ADTs)
• A component may be simple or composite

# Connectors
Connectors model: 
- Interactions beween componenets
- Rules that governs those interactions
Simple interactions:
- Procedure calls
- Shared variable access
Complex and semantically rich interactions
- Client-Server protocols
- Database access protocols

# Characteristics
Performance
- Localise critical operations and minimise communications. Use large
rather than fine-grain components.
Security
- Use a layered architecture with critical assets in the inner layers.
Availability
- Include redundant components and mechanisms for fault tolerance.
Maintainability
- Use fine-grain, replaceable components.

# Types of architecture
## Layered
4 layers:
- presentation
	- Make data human readable and nice
	- front end
- business
	- Contains most program logic
	- backend
	- communicates with presentation layer via events or queries
- persistence
	- wrapper for database
	- maps relational database to OOP
- database
### Principles
- Layers Isolation principle
	- Changes in one layer shouldn't affect other layers
	- Layers communicate through strict protocols and well defined interfaces (contracts)
- Neighbour communication principle
	- Components can only communicate through directly neighbouring layers
- Downward dependency principle
	- Higher levels rely on lower layers, but lower layers do not rely on higher ones

## Pipeline
Inputs passed through a series of one way filter components to receive an output.
Filters are self contained and independent components which only perform one task. 
![[Pasted image 20260329115111.png]]
## Microkernel
2 components: Core system and plug in components.
Core system provides minimal function. Extended by plug in components
Plug in components are standalone, specialised components meant to enhance or extend the core system

## Service based 
User interface communicates to backend services via API
Services are typically coarse-grained “portions of an application” (usually called domain services)