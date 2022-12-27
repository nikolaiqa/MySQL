# The "Elite parking" schema

As it was mentioned in the About part of this repository, the generated schema is a kind of database for a parking application. So the schema below involves four tables: Cars, Persons, Drivers and Schedule.

![messages_4](Sourses/Schema.png)
 
***The Cars*** table contains a list of cars that are allowed to be parked, each car has its single owner but the car might be used by several drivers at once or not used at all. 
___
Information about each person who associated with the cars is stored in the ***Persons*** table which may also help define how some persons could be interconnected to each other. If the "***chieff_id***" column of some row has a value it means that the row is about a personal driver. If some rows have the same values in the "***family_id***" column it means that those persons are relatives.
___
Who is permitted to drive a specific automobile is displayed in the Drivers table, there are their identities data as well. Since safety of the parking is ensured by it that's the most important table.
___  
All actions committing by drivers are recorded into the ***Schedule*** table if their authentication was passed successfully through the Drivers table.