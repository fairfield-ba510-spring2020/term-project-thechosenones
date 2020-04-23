BA 0510 Final Project - The Chosen Ones
Erik Hren, Brain Doyle, Travis Fuller

1) The first deliverable for the project was to create an ERD based on our understanding of the existing data, and normalizing it to BCNF or better.  A pdf of that document can be found here:

term-project-thechosenones/docs/The Chosen CourseDataERD.pdf

2) The second deliverable for the project was to write an ETL to create the database, per our ERD, and perform the extraction, transformation and loading of the source data into our database.  This document can be found here:

term-project-thechosenones/CourseDataETL.ipynb

The code includes
- SQL code to create the tables, per our ERD
- Python is used to automate the import data.  In a previous iteration this was done manually via renaming and relocating the files, and reading them through the terminal.
- SQl code to validate the imports.
- SQL code to insert the imported data into appropriate table in the database.
- Deletion of the import tables after they are no longer necessary, followed by a vacuum.

3) The third deliverable was to run some code to validate the ETL from (2).  This can be found here:

term-project-thechosenones/CourseDataTests.ipynb

Some of the queries were basic to test the information in each table.  Other queries were more specific and with a question in mind.

NOTE:  We note that the courses table doesn't have a match for the course_catalog for years prior 2017-2018.  Presumably, this data could be created manually (or programatically) via the pdfs, so that we could have course data information matching course catalog information for years prior to 2017-2018.

4) The fourth deliverable was to create a datawarehouse.  The pdf and ETL docs can be found at these locations, respectively:

term-project-thechosenones/docs/The Chosen DataWarehouseERD.pdf

term-project-thechosenones/CourseDataWarehouseETL.ipynb

This was similar to the steps 1 and 2 described in this document.

5) The fifth deliverable was to test the integrity and functionality of the data warehouse.  This was done in two documents.  The first document was to simply test the success of the ETL with simple queries of the tables in the datawarehouse.  The second document has more advanced queries with specific questions in mind.  Those two documents can be found at the below listed locations:

term-project-thechosenones/DataWarehouseTest.ipynb

term-project-thechosenones/DataWarehouseDemo.ipynb