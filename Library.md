# Library Management System

A **full-featured MySQL database** for managing library operations, including books, authors, members, categories, and loan tracking. This system demonstrates relational database design, relationships, constraints, and advanced features like timestamps and loan status tracking.

## Author
Fortune Akioya

---

## Features

- Manage **Books**, **Authors**, **Categories**, and **Members**.  
- Track **Loans** with status (`borrowed`, `returned`, `overdue`).  
- Enforces **relational integrity** using PRIMARY and FOREIGN keys.  
- Prevents duplicate active loans using unique constraints.  
- Timestamps for creation and updates on all records.  
- Many-to-Many relationship between Books and Authors via `BookAuthors`.  

---

## Database Schema

**Tables:**
1. `Authors` – Stores author information.  
2. `Categories` – Stores book categories/genres.  
3. `Books` – Stores book details and links to categories.  
4. `BookAuthors` – Junction table for many-to-many relationship between books and authors.  
5. `Members` – Stores library member information.  
6. `Loans` – Tracks which member borrowed which book, with status and dates.  

---

## Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com/<your-username>/library-management-system.git
