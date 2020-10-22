# DB normalization

Normalization of DBs means to organize your data into tables and columns, where each table serves a specific purpose.

This is intended to reduce errors in your data, reduce duplication of data and simplify your queries.

For example, if you have a list of people at an office, all in a table

Employee ID | Name | Office | Office Phone | cust1 | cust2 |
----------- | ---- | ------ | ------------ | ----- | ----- |
1234 | Fred M | NYC | 555 123 4567 | acme inc | beta testers
4444 | Julie S | SF | 555 545 5454 | giant inv | small potatoes llc
5432 | Dave J | NYC | 555 123 4567 | | doItRight solutions

If you have to update the NYC office phone numberm you have to update it for each emplyee that works at that office

If you wanted to delete an employee, you'd lose information about the relationship of a cust to that office, or a phone # to that office, etc

You cannot enter a new employee without knowing superfluous information about that row, like what customers they might have, or their ID

You have to search a cust1, and cust2 column to get the right details.

Normalization of this data would mean that these relations would exist in different tables, rather than all on the same table.

[<-- Back](../README.md)
