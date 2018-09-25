I'm not necessarily interested in FileMaker Pro, but this course seems to have a lot of good basic info.  That
said, this type of software makes it easy for casual users (e.g., your boss) to view and enter contents in the
database...  So it may be worth keeping in mind as I design things going forward.

------------------------------------

A relational database design looks to capture data in multiple, atomic tables that are 
related to each other by keys.  This is in contrast to a flat database design, which
seeks to capture all information in one table.

Benefit of relational model:
* Information is broken down into atomic tables so that info is only entered once,
  eliminating inconsistencies (e.g., a customer name is associated with a customer id in
  the customer table, which is where any other table that references customer gets the
  info from)
  
 
### Relational Modeling
In data modeling, the "atomic tables" are called entities, which become tables inside the 
database. Entities have attributes, which become a table's fields inside the database.

<img src="./images/database-construction.png">
