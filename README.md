# SQL_Store_Project
This was the second assignment while doing the level 3 bootcamp at Just IT

In this assignment, we allocated into small teams and the area of focus was to work as a team to improve our problem-solving skills with a collaborative approach. 
This was done by examining MySQL syntax and query writing to develop scripts on a database that was assigned called the store database
We rewrote scripts based on filtering & sorting using MySQL
We also worked on schemas to help get a better understanding of primary and foreign keys (PK and FK) and their relationships within a group of tables that was included with the database that was assigned for this assignment 
We discovered that using the Enhanced Entity-Relationship (EER) diagrams we could make adjustments to scripts without the need to manually adjust the existing script itself.
EER is an essential part of the modeling interface in the MySQL Workbench. EER diagrams provide a visual representation of the relationships among the tables in models.
We recreated Relational Database Schemas and then went on to write our own SQL queries using the assigned tables only.

![query 1](https://github.com/DanielMitchell45/SQL_Store_Project/assets/65592585/743c8ed5-e4fd-47e5-9714-9152080b5541)

![query 2](https://github.com/DanielMitchell45/SQL_Store_Project/assets/65592585/21a73810-f9ff-4185-b48c-5cd65e008019)

•	“Using the Query 2 you created change the points to read times by 10 and plus 100. Record your results in your Word document”

![Task 1](https://github.com/DanielMitchell45/SQL_Store_Project/assets/65592585/1f1aac36-9feb-4ec3-af47-7b18e5e6d896)

•	“Change the Query 2 code to create a discount factor so the table now shows a discount header and changing the (point + 10) *100”

![task 1 continued](https://github.com/DanielMitchell45/SQL_Store_Project/assets/65592585/d4f16d27-2945-4bae-bbf1-c50328dac053)

Task 2
•	“Using the Query 2 you created change the points to read times by 10 and plus 100. Record your results in your Word document”
![Task 2](https://github.com/DanielMitchell45/SQL_Store_Project/assets/65592585/cda60746-892d-43cc-9107-dd88cb4479af)

![Task 3](https://github.com/DanielMitchell45/SQL_Store_Project/assets/65592585/7eda1da4-b643-41a8-aaad-bb696a669bc4)

The original Foreign & Primary Keys identifications for the “create-db-store” database

Here are the original settings of the relational database model for the store database:

•	The primary Key for the products table is product_id. There is no foreign key for this table.

•	The Primary Key for the shippers table is shipper_id. There is no foreign key for this table.

•	The Primary Key for the customers table is customer_id. There is no foreign key for this table.

•	The primary Key for the order_statuses table is order_status_id. There is no foreign key for this table.

•	The Primary Key for the orders table is order_id.  The foreign keys for this table are: customer_id, shippers & status

•	The order_items table has a composite (compound key) key that consists of two columns of foreign keys from other tables in order to make a unique condition for this table. The combination of these two foreign keys that make up the compound keys are order_id from the orders table and product_id from the products table.

•	The order_item_notes has the note_id primary key.

![EER 1](https://github.com/DanielMitchell45/SQL_Store_Project/assets/65592585/cdf27cd6-7824-43fc-ab18-a7d41d94fe66)

As can be seen above, the ‘order_item_notes’ table did not have any connections to the other tables that could be queried. 
After this information was concluded, script modifications were made to the order_item_notes and the order_items table. 
This is because it was believed by our group at this time that these tables did not previously have unique columns where the values would always be unique. This was also before discovering the use of composite keys 

The First Modified EER Diagram

The diagram below shows the EER diagram after design modifications were made to link the order_item_notes table in the diagram with the other tables so that this table could be used for query joins for this group of tables via the order_items table. 
Modifications were also made to experiment in several ways to attempt to make the relationships between these seven tables more concise for queries. The first modification was done by creating additional columns to replace the two foreign keys that made the composite key for the order_items table. Adjustments were also made by actually adjusting the script via the script editor based on this theory. 
However, at this stage, it was discovered that the use of “forward engineering could actually make it possible and much easier to define the relations between tables by designing within the EER diagram. These procedures were implemented and the results can be seen in the EER diagrams below. 

![EER 2](https://github.com/DanielMitchell45/SQL_Store_Project/assets/65592585/e2521dcf-0dc5-4158-87f7-425f66a19202)

![2nd modified EER](https://github.com/DanielMitchell45/SQL_Store_Project/assets/65592585/0b6b5f92-893a-4b6e-baba-d5aa5d2f1933)

After all, adjustments were made with the EER diagram, The “Synchronise Model” option was selected so that the new changes with the EER diagram would be added to the live database in order to adjust the existing script that will show the new relationship constraints and all other changes made.
This was as far as this experiment got we ran out of time while working as a small team

Conclusion

Additional new columns were created and inserted in the first column’s location in several experiments.
 
Values were inserted into newly created columns during this process in an attempt to resolve theories for testing purposes 

I also investigated what would need to be written to ensure that duplicates could not be created and investigated using the ‘AUTO_INCREMENT’ function.  However, too much time was spent on this and this is as far as EER diagrams experimenting went on this occasion.

I have actually done additional changes and experiments since. However, the main focus was to develop personal queries using the methods that were shown during the previous classes on other databases for this database

Below are some screenshots of the queries that were created along with comments that may have been updated on the assignment script file that will be included with this. 

![SQL Query 6](https://github.com/DanielMitchell45/SQL_Store_Project/assets/65592585/49e69f76-c819-40dc-b5b5-702d593225c3)
![SQL QUERY 7](https://github.com/DanielMitchell45/SQL_Store_Project/assets/65592585/c9d421fc-9a81-446f-996e-46af229ad316)
![SQL Query 8](https://github.com/DanielMitchell45/SQL_Store_Project/assets/65592585/cdef4530-8914-4389-8b00-be62400bc291)
