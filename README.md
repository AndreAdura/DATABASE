# DATABASE

	PRESENTATION 1

SQL - Structured Query Language
ISBN -  International Standard Book Number
Types of Database - Relational,Network,Objected Oriented,Hierarcal
BLOB - Big Large OBjects
Acces format = .accdb > actual /  .mdb> old format
Database Objetcts - Tables, Forms, Reports, Queries

what is database?
function of database?

--------------------------------------------------------------------------------
	PRESENTATION 3
ER - Entity Relationship
AI - Auto Increment

Fan trap  - 1:*:*  One to many Relations
Composite Keys - is a key resulted of the combination of two items

Chasm trap - *:1:* many to many

-----------------------------------------------------------------------------------------
	PRESENTATION 3

NF - NORMALIZATION FORMS

------------------------------------------------------------------------------
	PRESENTATION 4(Comands, insert, change)

SELECIONAR MULTIPLOS CONTEUDOS - Create/Query Wizard/Ok  Selecionar oq vc quer selecionar. 
CONSOL - CREATE/QUERY DESIGN - Abrir Tabelas / View / SQL View / comandos 

Ex1: SELECT FirstName, LastName, Department FROM Employees
Ex2: SELECT * FROM Employees

Query from two different tables = 
SELECT Employees.FirstName, EmployeePhone.Number
FROM Employees INNER JOIN EmployeePhone ON Employees.EmployeeID = EmployeePhone.EmployeeID;

Query for a information inside the cell
SELECT FirstName, LastName, Department, Status FROM Employees WHERE Status = 'Full Time'
or
SELECT FirstName, LastName, Department, Salary FROM Employees WHERE Salary > 70000

Insert Content from SQL Consol
INSERT INTO tbl_student (Name, LastName, Gender, Grade) VALUES ('Satori', 'Shimokawa', 'Yes', 100);
OBS:Don't consider the Auto Number ID in this command

Change content
UPDATE Table SET Colum = 'new content' WHERE Column = 'cell content'
UPDATE Employees SET employees.salary = 1000000 WHERE Department = 'IT' 

Different sign ( <> Different )
UPDATE Employees SET BenefitDental = yes WHERE employees.Department <> 'Sales'


Operator	Description
=	Equal
<>	Not equal. Note: In some versions of SQL this operator may be written as !=
>	Greater than
<	Less than
>=	Greater than or equal
<=	Less than or equal
BETWEEN	Between an inclusive range
LIKE	Search for a pattern
IN	To specify multiple possible values for a column
