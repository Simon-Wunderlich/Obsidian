Created: Mar 27 2025
Class: [[Database]]
- - -

### Relational keys
| Name          | Definition                                                                                                 |
| ------------- | ---------------------------------------------------------------------------------------------------------- |
| Primary key   | Unique value(s) within a relation to identify a tuple<br>Minimal (Only requires necessary info)            |
| Super Key     | Set of attributes which contains a primary key                                                             |
| Candidate key | Minimal super key.<br>Set of attributes which can act as a primary key. Includes no unnecessary attributes |
| Foreign Key   | Unique value within a relation to identify a tuple from a different relation                               |

### Constraints
| **Name**             | **Definition**                                                          |
| -------------------- | ----------------------------------------------------------------------- |
| Entity Integrity     | Primary keys cannot be null in a base relation                          |
| Relational integrity | Foreign keys must match a candidate key in its home relation or be null |

### UML
#### Multiplicity
| Name                    | Definition                                                                            |
| ----------------------- | ------------------------------------------------------------------------------------- |
| Cardinality             | The highest number of possible relationships for a given entity                       |
| Participation           | The lowest number of possible relationships for a given entity                        |
| Simple attributes       | Stores single value                                                                   |
| Composite attributes    | Groups multiple different attributes                                                  |
| Multi-valued attributes | Store multiple values for the same attribute                                          |
| Relationship attributes | Defines extra info abt a relationship between entities                                |
| Strong entities         | - An entity which can stand alone<br>- Unique primary key                             |
| Weak entities           | - An entity that is dependant on another entity<br>- No primary key, only partial key |

