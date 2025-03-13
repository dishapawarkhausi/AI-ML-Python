# Python MySQL Queries Cheat Sheet

## 1. **Database Queries**
- CREATE DATABASE mydatabase;
- SHOW DATABASES;
- USE mydatabase;
- DROP DATABASE mydatabase;

## 2. **Table Queries**
- CREATE TABLE users (id INT AUTO_INCREMENT PRIMARY KEY, name VARCHAR(255), email VARCHAR(255), age INT);
- SHOW TABLES;
- DESCRIBE users;
- DROP TABLE users;
- ALTER TABLE users ADD COLUMN phone VARCHAR(15);
- ALTER TABLE users DROP COLUMN phone;
- ALTER TABLE users MODIFY COLUMN age SMALLINT;
- RENAME TABLE users TO customers;

## 3. **Insert Queries**
- INSERT INTO users (name, email, age) VALUES ('John Doe', 'john@example.com', 30);
- INSERT INTO users (name, email, age) VALUES ('Alice', 'alice@example.com', 25), ('Bob', 'bob@example.com', 28);

## 4. **Select Queries**
- SELECT * FROM users;
- SELECT name, email FROM users;
- SELECT * FROM users WHERE age > 25;
- SELECT * FROM users WHERE name LIKE 'J%';
- SELECT * FROM users ORDER BY age DESC;
- SELECT * FROM users LIMIT 5;
- SELECT DISTINCT name FROM users;
- SELECT COUNT(*) FROM users;
- SELECT AVG(age) FROM users;
- SELECT SUM(age) FROM users;
- SELECT MIN(age), MAX(age) FROM users;

## 5. **Update Queries**
- UPDATE users SET age = 35 WHERE name = 'John Doe';
- UPDATE users SET email = 'john.doe@example.com' WHERE name = 'John Doe';
- UPDATE users SET age = age + 1;

## 6. **Delete Queries**
- DELETE FROM users WHERE name = 'Bob';
- DELETE FROM users WHERE age < 20;
- DELETE FROM users;

## 7. **Joins Queries**
- SELECT users.name, orders.amount FROM users INNER JOIN orders ON users.id = orders.user_id;
- SELECT users.name, orders.amount FROM users LEFT JOIN orders ON users.id = orders.user_id;
- SELECT users.name, orders.amount FROM users RIGHT JOIN orders ON users.id = orders.user_id;
- SELECT users.name, orders.amount FROM users FULL JOIN orders ON users.id = orders.user_id;

## 8. **Index Queries**
- CREATE INDEX idx_name ON users(name);
- DROP INDEX idx_name ON users;

## 9. **Constraints Queries**
- CREATE TABLE employees (id INT PRIMARY KEY, name VARCHAR(255) NOT NULL, email VARCHAR(255) UNIQUE);
- ALTER TABLE employees ADD CONSTRAINT chk_age CHECK (age > 18);

## 10. **Transaction Queries**
- START TRANSACTION;
- INSERT INTO users (name, email) VALUES ('Mike', 'mike@example.com');
- COMMIT;
- ROLLBACK;

## 11. **Views Queries**
- CREATE VIEW user_emails AS SELECT name, email FROM users;
- SELECT * FROM user_emails;
- DROP VIEW user_emails;

## 12. **Stored Procedures Queries**
- CREATE PROCEDURE GetUsers() BEGIN SELECT * FROM users; END;
- CALL GetUsers();
- DROP PROCEDURE GetUsers;

## 13. **Triggers Queries**
- CREATE TRIGGER before_insert BEFORE INSERT ON users FOR EACH ROW SET NEW.name = UPPER(NEW.name);
- DROP TRIGGER before_insert;

## 14. **Functions Queries**
- CREATE FUNCTION get_total_users() RETURNS INT BEGIN RETURN (SELECT COUNT(*) FROM users); END;
- SELECT get_total_users();
- DROP FUNCTION get_total_users;

## 15. **Privileges Queries**
- GRANT ALL PRIVILEGES ON mydatabase.* TO 'username'@'localhost';
- REVOKE ALL PRIVILEGES ON mydatabase.* FROM 'username'@'localhost';
- SHOW GRANTS FOR 'username'@'localhost';

This cheat sheet contains 100 essential MySQL queries for database operations. 🚀
