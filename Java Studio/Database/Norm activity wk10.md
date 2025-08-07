Works on(**ESSN**, PNo*, PName, PLocation, DNo, Hours)
Employee(**SSN**, FName, MInit, LName, DoB, Position, Salary)

Functional dependancies
PName, PLocation -> PNo
DNo, Hours -> ESSN, PNo
Salary -> Position
FNamr, MInit, LName, DoB,  -> SSN




- - -

Bus(**Rego**\*, Brand, Model, YearMade, noSeats, ServiceInterval, LastServiceDate)
RouteAllocation(**Rego**\*, **RouteNo**\*, StartTerminus, EndTerminus, StartTime, EndTime, Remarks)

Functional dependencies
1
Bus
Rego -> brand, model, yearMade, noSeats

2
RouteAllocation
RouteNo -> StartTerminus, EndTerminus
3.

1st yes
2nd No
3rd No


Route(**RouteNo**, StartTerminus, EndTerminus)
Bus(**Rego**\*, ServiceInterval, LastServiceDate)
RouteAllocation(**Rego**\*, **RouteNo**\*, startTime, EndTime)
Model(**Brand, Model, YearMade**, noSeats)


Customer(**CustId**, CustName, Addr, CustPostCode)
SaleItem(**Invoice no\*,  ProdName,** Manufacturer, Country of origin, qty)
Invoice(**Invoice no**, CustId\*)
