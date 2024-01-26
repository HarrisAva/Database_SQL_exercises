CREATE TABLE Employees (
EmployeeID int,
FirstName varchar(255),
LastName varchar(255),
Department varchar(255)
);

CREATE TABLE Employees2 (
EmployeeID int,
FirstName varchar(255),
LastName varchar(255),
DepartmentID int
);

CREATE TABLE Departments (
DepartmentID int,
DepartmentName varchar(255)
);

CREATE TABLE Inventory (
ItemID int,
ItemName varchar(255),
UnitsInStock int
);

CREATE TABLE Books (
BookID int,
Title varchar(255),
Author varchar(255),
Price float
);

CREATE TABLE Courses (
CourseID int,
CourseName varchar(255),
Department varchar(255),
Credits int
);

CREATE TABLE RestaurantReviews (
ReviewID int,
RestaurantName varchar(255),
Rating varchar(255),
Reviewer varchar(255),
ReviewDate date
);

CREATE TABLE Sales (
SaleID int,
ProductID int,
QuantitySold int,
SaleDate date
);

CREATE TABLE Products (
ProductID int,
ProductName varchar(255),
Price float,
Category varchar(255)
);

CREATE TABLE Products2(
ProductID int,
ProductName varchar(255)
);

CREATE TABLE Orders (
OrderID int,
ProductID int,
OrderDate date
);

CREATE TABLE WeatherData (
RecordID int,
Date date,
Temperature float,
City varchar(255)
);

INSERT INTO Employees (EmployeeID, FirstName, LastName, Department) VALUES (1, 'Alice', 'Johnson', 'HR');
INSERT INTO Employees (EmployeeID, FirstName, LastName, Department) VALUES (2, 'Bob', 'Smith', 'IT');

INSERT INTO Inventory (ItemID, ItemName, UnitsInStock) VALUES (1, 'Printer Paper', 15);
INSERT INTO Inventory (ItemID, ItemName, UnitsInStock) VALUES (2, 'Staples', 30);

INSERT INTO Books (BookID, Title, Author, Price) VALUES (1, 'The Great Gatsby', 'F. Scott Fitzgerald', 10.99);
INSERT INTO Books (BookID, Title, Author, Price) VALUES (2, '1984', 'George Orwell', 8.99);
INSERT INTO Books (BookID, Title, Author, Price) VALUES (3, 'The Catcher in the Rye', 'J. D. Salinger', 7.99);

INSERT INTO Courses (CourseID, CourseName, Department, Credits) VALUES (101, 'Introduction to Psychology', 'Psychology', 3);
INSERT INTO Courses (CourseID, CourseName, Department, Credits) VALUES (102, 'Principles of Economics', 'Economics', 4);
INSERT INTO Courses (CourseID, CourseName, Department, Credits) VALUES (103, 'Introduction to Computer Science', 'Computer Science', 3);

INSERT INTO RestaurantReviews (ReviewID, RestaurantName, Rating, Reviewer, ReviewDate)
VALUES (1, 'Cafe Mocha', 'Excellent', 'John Doe', '2022-01-15');
INSERT INTO RestaurantReviews (ReviewID, RestaurantName, Rating, Reviewer, ReviewDate)
VALUES (2, 'Burger Corner', 'Good', 'Jane Smith', '2022-02-20');
INSERT INTO RestaurantReviews (ReviewID, RestaurantName, Rating, Reviewer, ReviewDate)
VALUES (3, 'Pasta Place', 'Excellent', 'Alice Jones', '2022-02-22');

INSERT INTO Sales (SaleID, ProductID, QuantitySold, SaleDate) VALUES (101, 1, 50, '2022-01-01');
INSERT INTO Sales (SaleID, ProductID, QuantitySold, SaleDate) VALUES (102, 2, 30, '2022-01-02');
INSERT INTO Sales (SaleID, ProductID, QuantitySold, SaleDate) VALUES (103, 1, 20, '2022-01-03');

INSERT INTO Products (ProductID, ProductName, Price, Category) VALUES (1, 'Apple', 0.50, 'Fruit');
INSERT INTO Products (ProductID, ProductName, Price, Category) VALUES (2, 'Bread', 1.50, 'Bakery');

INSERT INTO Products2 (ProductID, ProductName) VALUES (1, 'Laptop');
INSERT INTO Products2 (ProductID, ProductName) VALUES (2, 'Desk Chair');

INSERT INTO Orders (OrderID, ProductID, OrderDate) VALUES (1, 1, '2023-01-01');
INSERT INTO Orders (OrderID, ProductID, OrderDate) VALUES (2, 2, '2023-01-02');

INSERT INTO WeatherData (RecordID, Date, Temperature , City) VALUES (1, '2022-01-01', 35.2, 'Springfield');
INSERT INTO WeatherData (RecordID, Date, Temperature , City) VALUES (2, '2022-01-01', 28.4, 'Shelbyville');

INSERT INTO Employees2 (EmployeeID, FirstName, LastName, DepartmentID) VALUES (1, 'Alice', 'Johnson', 1);
INSERT INTO Employees2 (EmployeeID, FirstName, LastName, DepartmentID) VALUES (2, 'Bob', 'Smith', 2);

INSERT INTO Departments (DepartmentID, DepartmentName) VALUES (1, 'HR');
INSERT INTO Departments (DepartmentID, DepartmentName) VALUES (2, 'IT');
SELECT e.FirstName, e.LastName, d.DepartmentName from Employees2 e
INNER JOIN Departments d ON e.DepartmentID = d.DepartmentID;

=================================================

-- Exercise 2
-- Objective: Select only the FirstName and LastName columns from the Employees table.
-- Table: Employees
-- Columns: EmployeeID (int), FirstName (text), LastName (text), Department (text)
-- Data:
-- (1, 'Alice', 'Johnson', 'HR')
-- (2, 'Bob', 'Smith', 'IT')
-- The expected outcome should be

| --  | FirstName | LastName |
| --- | --------- | -------- |
| --  | Alice     | Johnson  |
| --  | Bob       | Smith    |

CREATE TABLE Employees (
EmployeeID int,
FirstName varchar(255),
LastName varchar(255),
Department varchar(255)
);

INSERT INTO Employees (EmployeeID, FirstName, LastName, Department) VALUES (1, 'Alice', 'Johnson', 'HR');
INSERT INTO Employees (EmployeeID, FirstName, LastName, Department) VALUES (2, 'Bob', 'Smith', 'IT');

SELECT FirstName, LastName FROM Employees;

-- Exercise 3
-- Objective: Display details of items in the Inventory table that have less than 20 units in stock.
-- Table: Inventory
-- Columns: ItemID (int), ItemName (text), UnitsInStock (int)
-- Data:
-- (1, 'Printer Paper', 15)
-- (2, 'Staples', 30)
-- The expected outcome should be

| --  | ItemID | ItemName      | UnitsInStock |
| --- | ------ | ------------- | ------------ |
| --  | 1      | Printer Paper | 15           |

CREATE TABLE Inventory (
ItemID int,
ItemName varchar(255),
UnitsInStock varchar(255)
);

INSERT INTO Inventory (ItemID, ItemName, UnitsInStock) VALUES (1, 'Printer Paper', 15);
INSERT INTO Inventory (ItemID, ItemName, UnitsInStock) VALUES (2, 'Staples', 30);

SELECT \* FROM Inventory
WHERE UnitsInStock < 20;
