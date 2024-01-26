DB Exercise Part 1

Exercise 1
Objective: Retrieve all data from the Products table.
Table: Products
Columns: ProductID (int), ProductName (text), Price (float), Category (text)
Data:
(1, 'Laptop', 1200.00, 'Electronics')
(2, 'Desk Chair', 250.50, 'Furniture')
The expected outcome should be

| ProductID | ProductName | Price  | Category    |
| --------- | ----------- | ------ | ----------- |
| 1         | Laptop      | 1200.0 | Electronics |
| 2         | Desk Chair  | 250.5  | Furniture   |

Exercise 2
Objective: Select only the FirstName and LastName columns from the Employees table.
Table: Employees
Columns: EmployeeID (int), FirstName (text), LastName (text), Department (text)
Data:
(1, 'Alice', 'Johnson', 'HR')
(2, 'Bob', 'Smith', 'IT')
The expected outcome should be

| FirstName | LastName |
| --------- | -------- |
| Alice     | Johnson  |
| Bob       | Smith    |

Exercise 3
Objective: Display details of items in the Inventory table that have less than 20 units in stock.
Table: Inventory
Columns: ItemID (int), ItemName (text), UnitsInStock (int)
Data:
(1, 'Printer Paper', 15)
(2, 'Staples', 30)
The expected outcome should be

| ItemID | ItemName      | UnitsInStock |
| ------ | ------------- | ------------ |
| 1      | Printer Paper | 15           |

Exercise 4
Objective: Retrieve all data from the Books table.
Table: Books
Columns: BookID (int), Title (text), Author (text), Price (float)
Data:
(1, 'The Great Gatsby', 'F. Scott Fitzgerald', 10.99)
(2, '1984', 'George Orwell', 8.99)
(3, 'The Catcher in the Rye', 'J. D. Salinger', 7.99)
The expected outcome should be

| BookID | Title                  | Author              | Price |
| ------ | ---------------------- | ------------------- | ----- |
| 1      | The Great Gatsby       | F. Scott Fitzgerald | 10.99 |
| 2      | 1984                   | George Orwell       | 8.99  |
| 3      | The Catcher in the Rye | J. D. Salinger      | 7.99  |

Exercise 5
Objective: Display the course names and their corresponding department from the Courses table.
Table: Courses
Columns: CourseID (int), CourseName (text), Department (text), Credits (int)
Data:
(101, 'Introduction to Psychology', 'Psychology', 3)
(102, 'Principles of Economics', 'Economics', 4)
(103, 'Introduction to Computer Science', 'Computer Science', 3)
The expected outcome should be

| CourseName                       | Department       |
| -------------------------------- | ---------------- |
| Introduction to Psychology       | Psychology       |
| Principles of Economics          | Economics        |
| Introduction to Computer Science | Computer Science |

Exercise 6
Objective: Retrieve the names of restaurants that have received a rating of "Excellent".
Table: RestaurantReviews
Columns: ReviewID (int), RestaurantName (text), Rating (text), Reviewer (text), ReviewDate (date)
Data:
(1, 'Cafe Mocha', 'Excellent', 'John Doe', '2022-01-15')
(2, 'Burger Corner', 'Good', 'Jane Smith', '2022-02-20')
(3, 'Pasta Place', 'Excellent', 'Alice Jones', '2022-02-22')
The expected outcome should be

| RestaurantName |
| -------------- |
| Cafe Mocha     |
| Pasta Place    |

Exercise 7
Objective: Find the total sales amount for each product.
Table: Sales
Columns: SaleID (int), ProductID (int), SaleAmount (float)
Data:
(1, 1, 1200.00)
(2, 2, 250.50)
The expected return should be the sum which is 1450.50

Exercise 8
Objective: Calculate the average price of all products in the Products table.
Table: Products
Columns: ProductID (int), ProductName (text), Price (float), Category (text)
Data:
(1, 'Apple', 0.50, 'Fruit')
(2, 'Bread', 1.50, 'Bakery')
The expected return should be the average which is 1.00

Exercise 9
Objective: Find the total quantity sold for a specific product such as the product with the id of 1 from the Sales table.
Table: Sales
Columns: SaleID (int), ProductID (int), QuantitySold (int), SaleDate (date)
Data:
(101, 1, 50, '2022-01-01')
(102, 2, 30, '2022-01-02')
(103, 1, 20, '2022-01-03')
The expected return should be the sum which is 70.

Exercise 10
Objective: Retrieve the maximum and minimum temperature recorded in the WeatherData table.
Table: WeatherData
Columns: RecordID (int), Date (date), Temperature (float), City (text)
Data:
(1, '2022-01-01', 35.2, 'Springfield')
(2, '2022-01-01', 28.4, 'Shelbyville')
Exercise 11
Objective: Show the product names and their corresponding order dates.
Tables:
Orders: OrderID (int), ProductID (int), OrderDate (date)
Products: ProductID (int), ProductName (text)
Data:
Orders: (1, 1, '2023-01-01'), (2, 2, '2023-01-02')
Products: (1, 'Laptop'), (2, 'Desk Chair')
The expected return should be

| ProductName | OrderDate  |
| ----------- | ---------- |
| Laptop      | 2023-01-01 |
| Desk Chair  | 2023-01-02 |

Exercise 12
Objective: Display the name of each employee and the name of the department they work in.
Tables:
Employees: EmployeeID (int), FirstName (text), LastName (text), DepartmentID (int)
Departments: DepartmentID (int), DepartmentName (text)
Data:
Employees: (1, 'Alice', 'Johnson', 1), (2, 'Bob', 'Smith', 2)
Departments: (1, 'HR'), (2, 'IT')
==========================================================

DB Exercise Part2
Exercise 1
Objective: Insert data into a Customers table.
Table: Customers
Columns: CustomerID (int), Name (text), Email (text)
Task: Insert three new customers into the Customers table.
Data:
(1, 'Alice Johnson', 'alice.johnson@email.com')
(2, 'Bob Smith', 'bob.smith@email.com')
(3, 'Charlie Brown', 'charlie.brown@email.com')
The expected outcome should be

| CustomerID | Name          | Email                   |
| ---------- | ------------- | ----------------------- |
| 1          | Alice Johnson | alice.johnson@email.com |
| 2          | Bob Smith     | bob.smith@email.com     |
| 3          | Charlie Brown | charlie.brown@gmail.com |

Exercise 2
Continue from the previous exercises.

Objective: Update the email address of a specific customer.
Table: Customers
Task: Change the email address of the customer with CustomerID 2 to bob.smith@newdomain.com.
Exercise 3
Objective: Delete a customer from the Customers table.
Table: Customers
Task: Remove the customer with CustomerID 3 from the table.
Expected Outcome: The table should no longer include the customer with CustomerID 3.
Exercise 4
Objective: Retrieve detailed order information.
Tables: Customers, Orders, Books
Task: Write a query to display the customer name, book title, and quantity for each order.
Expected Outcome: A list of all orders with customer names, book titles, and quantities.
Exercise 5
Objective: Normalize a denormalized table.
Table: StudentGrades (denormalized)
Columns: StudentID, Name, Subject, Grade
Task: Split the StudentGrades table into two tables: Students and Grades, ensuring normalization.
Expected Outcome: Two tables, Students with StudentID and Name columns, and Grades with StudentID, Subject, and Grade columns.
ER Diagrams Exercises
Instructions
Use a cloud-based service or a local IDE to create ER diagrams. Recommended tools:
Lucid Charts
Diagrams.net
Visual Studio Code with the Draw.io Integration extension.
One to One Relationships
Using the above tools, create ER diagrams for the following exercises.

Exercise 1: Apartment Complex

Entities:

Apartment: id (Primary Key), room_number, active (Boolean), renter_id (Foreign Key)
Renter: id (Primary Key), first_name, last_name, email, license_number, apartment_id (Foreign Key)
Task: Create an ER diagram showing each apartment linked to one unique renter and vice versa.

Exercise 2: Airport

Entities:

Person: id (Primary Key), name, date_of_birth, passport_id (Foreign Key)
Passport: id (Primary Key), passport_number, issue_date, expiry_date, person_id (Foreign Key)
Task: Illustrate how each person has a unique passport, with a one-to-one correspondence.

One to Many Relationships
Create ER diagrams for the following exercises.

Exercise 3: Library

Entities:

Book: id (Primary Key), title, publication_year
Author: id (Primary Key), name, nationality
BookAuthor: book_id (Foreign Key), author_id (Foreign Key)
Task: Create an ER diagram to illustrate a scenario where each book can be written by multiple authors. The "BookAuthor" table acts as an intermediary to link books with their authors, reflecting a one-to-many relationship from authors to books.

Exercise 4: Rent (Customers and Cars)

Entities:

Customer: id (Primary Key), name, contact_info
Car: id (Primary Key), make, model
Rental: rental_id (Primary Key), customer_id (Foreign Key), car_id (Foreign Key), rental_date, return_date
Task: Develop an ER diagram showing how a customer can rent multiple cars over time. The "Rental" entity serves as an intermediary, linking customers with cars and capturing details of each rental transaction.

Many to Many Relationships
Exercise 5: Grade School

Entities:

Student: id (Primary Key), name, grade_level
Course: id (Primary Key), course_name, department
To establish a many-to-many relationship, we need to create a third table to link the two entities.

Task: Show how students can enroll in multiple courses, with courses having multiple students.

Exercise 6: Work

Entities:

Employee: id (Primary Key), name, department
Project: id (Primary Key), project_name, deadline
To establish a many-to-many relationship, we need to create a third table to link the two entities.

Task: Create an ER diagram where employees work on multiple projects, and each project involves multiple employees.

Optional
Revisit the project you've worked on in the Front End Cohort and design an entity relationship diagram for the database you've created.
