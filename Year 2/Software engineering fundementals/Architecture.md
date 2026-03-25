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