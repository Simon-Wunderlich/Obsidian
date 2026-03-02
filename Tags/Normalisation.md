Created: Jun 04 2025
Class: [[Database]] 
- - -
![[Armstrongs axioms]]

## Crud anomalies

#### Insert
Can't insert element without primary key

#### Update
Can't update smth that dont exist?

#### Delete 
Can't delete smth thats not real


## Normalisation
Delete repeated groups
Remove non-atomic cells (make it 1 value per cell)

#### First normal form
Using partial keys

#### Second normal form
Already in first normal form AND removed partial dependency (ie columns not relevent to all primary keys)

Only applies to tables with composite keys
Every non-key column is dependant on all primary keys

#### Third normal form
Required to also be in 1st and 2nd normal forms

Remove transitive dependencies
All columns are independent from each other

All non-key columns are dependant on all primary keys alone