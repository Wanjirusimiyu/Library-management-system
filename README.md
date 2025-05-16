# Library Management System – MySQL Database

This project is a simple **Library Management System** built using **MySQL**.  
It demonstrates how to design and implement a **relational database** using SQL for a real-world scenario.  
It includes well-structured tables, primary and foreign key relationships, and constraints.

---

## Minimum Viable Product

- Model a real-world library system using MySQL.
- Create relational tables with proper keys and constraints.
- Demonstrate 1-to-many and many-to-1 relationships.
- Store data about books, authors, categories, members, and borrowing history.

---

## Entities & Tables

| Table Name    | Description                                           |
|---------------|-------------------------------------------------------|
| `authors`     | Stores information about book authors.                |
| `categories`  | Stores the category (genre) of each book.             |
| `books`       | Contains book details and links to authors & categories. |
| `members`     | Tracks library users who borrow books.                |
| `borrowings`  | Records who borrowed which book and when.            |

---

## Relationships & Constraints

- Each book **belongs to** one author (`author_id`) → many-to-one.
- Each book is **categorized under** one category (`category_id`) → many-to-one.
- One member can borrow **many books**, but each borrowing links to one book → many-to-one.
- All foreign key references ensure **data integrity**.

---

## Technologies Used

- **MySQL** (Structured Query Language)
- `library.sql` file containing all `CREATE TABLE` statements.

---

## Files Included

- `library.sql`  
  → Contains all SQL `CREATE TABLE` statements for the 5 tables.

---

##  How to Use

1. Open **MySQL Workbench** or your MySQL terminal.
2. Create a new database:
   ```sql
   CREATE DATABASE library;
   USE library;
