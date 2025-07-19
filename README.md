---

## ✅ MySQL Learning Roadmap

---

### 🟢 **Beginner Level**

#### 📘 Topics:

1. **What is MySQL & SQL**
2. **Installing MySQL (Workbench/XAMPP)**
3. **Basic SQL Syntax**
4. **Creating Databases & Tables**
5. **Data Types (INT, VARCHAR, DATE, etc.)**
6. **CRUD Operations:**

   * `CREATE` – add data
   * `READ (SELECT)` – fetch data
   * `UPDATE` – modify data
   * `DELETE` – remove data
7. **Filtering with WHERE**
8. **Sorting with ORDER BY**
9. **LIMIT keyword**

#### 🧪 Practice:

```sql
CREATE TABLE users (
  id INT PRIMARY KEY AUTO_INCREMENT,
  name VARCHAR(100),
  email VARCHAR(100)
);

INSERT INTO users (name, email) VALUES ('Fakhir', 'fakhir@example.com');

SELECT * FROM users WHERE name = 'Fakhir';
```

#### 📚 Free Resources:

* [W3Schools SQL](https://www.w3schools.com/sql/)
* [SQLBolt](https://sqlbolt.com/)
* [SQLZOO](https://sqlzoo.net/)

---

### 🟡 **Intermediate Level**

#### 📘 Topics:

1. **Relationships & Foreign Keys**
2. **JOINs (INNER, LEFT, RIGHT, FULL)**
3. **GROUP BY & Aggregate Functions:**

   * `COUNT()`, `SUM()`, `AVG()`, `MAX()`, `MIN()`
4. **Subqueries**
5. **Aliases using AS**
6. **Data Normalization (1NF, 2NF, 3NF)**
7. **Indexing**
8. **Basic Views**

#### 🧪 Practice:

```sql
-- Join example
SELECT orders.id, users.name
FROM orders
JOIN users ON orders.user_id = users.id;

-- Aggregate
SELECT user_id, COUNT(*) as total_orders
FROM orders
GROUP BY user_id;
```

#### 📚 Resources:

* [Khan Academy SQL Course](https://www.khanacademy.org/computing/computer-programming/sql)
* [LeetCode SQL Problems](https://leetcode.com/problemset/database/)
* YouTube: **Programming with Mosh**, **BroCode**

---

### 🔴 **Advanced Level**

#### 📘 Topics:

1. **Stored Procedures & Functions**
2. **Triggers**
3. **Transactions & COMMIT/ROLLBACK**
4. **Advanced Indexing**
5. **Performance Optimization**
6. **User Permissions & Security**
7. **Backup and Restore**
8. **Partitioning**

#### 🧪 Practice:

```sql
-- Stored procedure
DELIMITER //
CREATE PROCEDURE GetUserById(IN uid INT)
BEGIN
  SELECT * FROM users WHERE id = uid;
END //
DELIMITER ;

CALL GetUserById(1);
```

#### 📚 Resources:

* [MySQL Official Docs](https://dev.mysql.com/doc/)
* [Mode SQL Tutorial](https://mode.com/sql-tutorial/)
* YouTube: **The Net Ninja - MySQL**, **Traversy Media**

---

## 🚀 Bonus: Projects to Practice

| Project Idea            | Tech Stack                     |
| ----------------------- | ------------------------------ |
| Login System            | HTML + PHP + MySQL             |
| Blog Website            | React + Node.js + MySQL        |
| Todo List with Auth     | React + PHP + MySQL            |
| Inventory Management    | MySQL + Express.js             |
| School/Student Database | MySQL + any backend (PHP/Node) |

---
