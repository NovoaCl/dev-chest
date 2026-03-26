
# SQL Reference / Referencia SQL

### 1. Data Types

**Description:** Common SQL data types for defining table columns.

| Description            | Function / Feature | Example               |
| ---------------------- | ------------------ | --------------------- |
| Integer numeric type   | `INT`              | `id INT`              |
| Large integer type     | `BIGINT`           | `big_number BIGINT`   |
| Variable length string | `VARCHAR(n)`       | `name VARCHAR(50)`    |
| Fixed length string    | `CHAR(n)`          | `code CHAR(5)`        |
| Text data type         | `TEXT`             | `description TEXT`    |
| Date                   | `DATE`             | `birth_date DATE`     |
| Time                   | `TIME`             | `start_time TIME`     |
| Date and time          | `DATETIME`         | `created_at DATETIME` |
| Boolean                | `BOOLEAN`          | `is_active BOOLEAN`   |
| Decimal / Numeric      | `DECIMAL(p,s)`     | `price DECIMAL(10,2)` |

---

### 2. Table Creation & Modification

**Description:** Commands to create and modify database tables.

| Description        | Function / Feature            | Example                                                      |
| ------------------ | ----------------------------- | ------------------------------------------------------------ |
| Create a new table | `CREATE TABLE`                | `CREATE TABLE users (id INT PRIMARY KEY, name VARCHAR(50));` |
| Add column         | `ALTER TABLE ... ADD COLUMN`  | `ALTER TABLE users ADD COLUMN email VARCHAR(100);`           |
| Modify column      | `ALTER TABLE ... MODIFY`      | `ALTER TABLE users MODIFY COLUMN name VARCHAR(100);`         |
| Drop column        | `ALTER TABLE ... DROP COLUMN` | `ALTER TABLE users DROP COLUMN email;`                       |
| Drop table         | `DROP TABLE`                  | `DROP TABLE users;`                                          |

---

### 3. Basic Clauses

**Description:** Essential SQL clauses for querying data.

| Description    | Function / Feature | Example                                                                               |
| -------------- | ------------------ | ------------------------------------------------------------------------------------- |
| Select columns | `SELECT`           | `SELECT id, name FROM users;`                                                         |
| Filter rows    | `WHERE`            | `SELECT * FROM users WHERE is_active = TRUE;`                                         |
| Order results  | `ORDER BY`         | `SELECT * FROM users ORDER BY name ASC;`                                              |
| Group rows     | `GROUP BY`         | `SELECT department, COUNT(*) FROM employees GROUP BY department;`                     |
| Filter groups  | `HAVING`           | `SELECT department, COUNT(*) FROM employees GROUP BY department HAVING COUNT(*) > 5;` |

---

### 4. Joins & Relationships

**Description:** Combine rows from multiple tables.

| Description     | Function / Feature | Example                                                                  |
| --------------- | ------------------ | ------------------------------------------------------------------------ |
| Inner join      | `INNER JOIN`       | `SELECT * FROM orders o INNER JOIN customers c ON o.customer_id = c.id;` |
| Left join       | `LEFT JOIN`        | `SELECT * FROM orders o LEFT JOIN customers c ON o.customer_id = c.id;`  |
| Right join      | `RIGHT JOIN`       | `SELECT * FROM orders o RIGHT JOIN customers c ON o.customer_id = c.id;` |
| Full outer join | `FULL OUTER JOIN`  | `SELECT * FROM a FULL OUTER JOIN b ON a.id = b.id;`                      |

---

### 5. Aggregate Functions

**Description:** Functions to summarize data.

| Description   | Function / Feature | Example                              |
| ------------- | ------------------ | ------------------------------------ |
| Count rows    | `COUNT()`          | `SELECT COUNT(*) FROM users;`        |
| Sum values    | `SUM()`            | `SELECT SUM(salary) FROM employees;` |
| Average       | `AVG()`            | `SELECT AVG(salary) FROM employees;` |
| Maximum value | `MAX()`            | `SELECT MAX(salary) FROM employees;` |
| Minimum value | `MIN()`            | `SELECT MIN(salary) FROM employees;` |

---

### 6. Text Functions

**Description:** Functions for manipulating strings.

| Description         | Function / Feature | Example                                                 |
| ------------------- | ------------------ | ------------------------------------------------------- |
| Concatenate strings | `CONCAT()`         | `SELECT CONCAT(first_name, ' ', last_name) FROM users;` |
| Substring           | `SUBSTRING()`      | `SELECT SUBSTRING(name, 1, 3) FROM users;`              |
| Length              | `LENGTH()`         | `SELECT LENGTH(name) FROM users;`                       |
| Uppercase           | `UPPER()`          | `SELECT UPPER(name) FROM users;`                        |
| Lowercase           | `LOWER()`          | `SELECT LOWER(name) FROM users;`                        |

---

### 7. Date & Time Functions

**Description:** Functions to work with date and time values.

| Description              | Function / Feature | Example                                       |
| ------------------------ | ------------------ | --------------------------------------------- |
| Current date and time    | `NOW()`            | `SELECT NOW();`                               |
| Add interval             | `DATEADD()`        | `SELECT DATEADD(day, 7, NOW());`              |
| Difference between dates | `DATEDIFF()`       | `SELECT DATEDIFF('2026-03-26','2026-03-01');` |
| Extract part of date     | `EXTRACT()`        | `SELECT EXTRACT(YEAR FROM NOW());`            |

---

### 8. Numeric Functions

**Description:** Functions for numeric operations.

| Description    | Function / Feature | Example                    |
| -------------- | ------------------ | -------------------------- |
| Round a number | `ROUND()`          | `SELECT ROUND(3.14159,2);` |
| Ceiling        | `CEIL()`           | `SELECT CEIL(3.14);`       |
| Floor          | `FLOOR()`          | `SELECT FLOOR(3.14);`      |
| Absolute value | `ABS()`            | `SELECT ABS(-5);`          |

---

### 9. Subqueries

**Description:** Nested queries inside another query.

| Description        | Function / Feature          | Example                                                                                              |
| ------------------ | --------------------------- | ---------------------------------------------------------------------------------------------------- |
| Subquery in SELECT | `SELECT ... (SELECT ...)`   | `SELECT name, (SELECT COUNT(*) FROM orders WHERE customer_id = users.id) AS order_count FROM users;` |
| Subquery in WHERE  | `WHERE ... IN (SELECT ...)` | `SELECT * FROM users WHERE id IN (SELECT customer_id FROM orders);`                                  |

---

### 10. Operators

**Description:** Logical and comparison operators.

| Description  | Function / Feature | Example                                                     |
| ------------ | ------------------ | ----------------------------------------------------------- |
| Equals       | `=`                | `SELECT * FROM users WHERE id = 1;`                         |
| Not equals   | `!=` or `<>`       | `SELECT * FROM users WHERE id != 1;`                        |
| Greater than | `>`                | `SELECT * FROM users WHERE salary > 50000;`                 |
| Less than    | `<`                | `SELECT * FROM users WHERE salary < 50000;`                 |
| AND          | `AND`              | `SELECT * FROM users WHERE active = TRUE AND role='admin';` |
| OR           | `OR`               | `SELECT * FROM users WHERE role='admin' OR role='manager';` |
| IN           | `IN`               | `SELECT * FROM users WHERE id IN (1,2,3);`                  |
| BETWEEN      | `BETWEEN`          | `SELECT * FROM orders WHERE total BETWEEN 100 AND 500;`     |
| LIKE         | `LIKE`             | `SELECT * FROM users WHERE name LIKE 'J%';`                 |

---

### 11. Indexes & Constraints

**Description:** Ensure data integrity and improve query performance.

| Description      | Function / Feature | Example                                             |
| ---------------- | ------------------ | --------------------------------------------------- |
| Primary key      | `PRIMARY KEY`      | `id INT PRIMARY KEY`                                |
| Foreign key      | `FOREIGN KEY`      | `FOREIGN KEY(customer_id) REFERENCES customers(id)` |
| Unique           | `UNIQUE`           | `email VARCHAR(100) UNIQUE`                         |
| Check constraint | `CHECK`            | `salary INT CHECK (salary>0)`                       |
| Create index     | `CREATE INDEX`     | `CREATE INDEX idx_name ON users(name);`             |

---

### 12. Transactions & Concurrency

**Description:** Commands to manage transactions.

| Description          | Function / Feature  | Example          |
| -------------------- | ------------------- | ---------------- |
| Start transaction    | `BEGIN TRANSACTION` | `BEGIN;`         |
| Commit transaction   | `COMMIT`            | `COMMIT;`        |
| Rollback transaction | `ROLLBACK`          | `ROLLBACK;`      |
| Savepoint            | `SAVEPOINT`         | `SAVEPOINT sp1;` |

---

### 13. Stored Procedures & Triggers

**Description:** Reusable SQL code and automated actions.

| Description             | Function / Feature | Example                                                                                            |
| ----------------------- | ------------------ | -------------------------------------------------------------------------------------------------- |
| Create stored procedure | `CREATE PROCEDURE` | `CREATE PROCEDURE AddUser(IN name VARCHAR(50)) BEGIN INSERT INTO users(name) VALUES(name); END;`   |
| Execute procedure       | `CALL`             | `CALL AddUser('John');`                                                                            |
| Create trigger          | `CREATE TRIGGER`   | `CREATE TRIGGER trg_before_insert BEFORE INSERT ON users FOR EACH ROW SET NEW.created_at = NOW();` |

---

### 14. Views & CTE

**Description:** Virtual tables and reusable queries.

| Description             | Function / Feature | Example                                                                                                                              |
| ----------------------- | ------------------ | ------------------------------------------------------------------------------------------------------------------------------------ |
| Create view             | `CREATE VIEW`      | `CREATE VIEW active_users AS SELECT * FROM users WHERE active = TRUE;`                                                               |
| Common Table Expression | `WITH`             | `WITH dept_count AS (SELECT department, COUNT(*) AS cnt FROM employees GROUP BY department) SELECT * FROM dept_count WHERE cnt > 5;` |

---

### 15. Advanced Utilities

**Description:** Advanced SQL features and functions.

| Description         | Function / Feature | Example                                                                          |
| ------------------- | ------------------ | -------------------------------------------------------------------------------- |
| Limit rows          | `LIMIT`            | `SELECT * FROM users LIMIT 10;`                                                  |
| Offset rows         | `OFFSET`           | `SELECT * FROM users LIMIT 10 OFFSET 5;`                                         |
| Case expression     | `CASE`             | `SELECT name, CASE WHEN salary>50000 THEN 'High' ELSE 'Low' END FROM employees;` |
| COALESCE function   | `COALESCE`         | `SELECT COALESCE(nickname, name) FROM users;`                                    |
| CAST / Convert type | `CAST`             | `SELECT CAST(salary AS DECIMAL(10,2)) FROM employees;`                           |

---

## Versión en Español

### 1. Tipos de Datos

**Descripción:** Tipos de datos comunes para definir columnas de tablas.

| Descripción                 | Función / Característica | Ejemplo               |
| --------------------------- | ------------------------ | --------------------- |
| Entero                      | `INT`                    | `id INT`              |
| Entero grande               | `BIGINT`                 | `big_number BIGINT`   |
| Cadena de longitud variable | `VARCHAR(n)`             | `name VARCHAR(50)`    |
| Cadena de longitud fija     | `CHAR(n)`                | `code CHAR(5)`        |
| Texto                       | `TEXT`                   | `description TEXT`    |
| Fecha                       | `DATE`                   | `birth_date DATE`     |
| Hora                        | `TIME`                   | `start_time TIME`     |
| Fecha y hora                | `DATETIME`               | `created_at DATETIME` |
| Booleano                    | `BOOLEAN`                | `is_active BOOLEAN`   |
| Decimal / Numérico          | `DECIMAL(p,s)`           | `price DECIMAL(10,2)` |

---

### 2. Creación y Modificación de Tablas

**Descripción:** Comandos para crear y modificar tablas de base de datos.

| Descripción       | Función / Característica      | Ejemplo                                                      |
| ----------------- | ----------------------------- | ------------------------------------------------------------ |
| Crear nueva tabla | `CREATE TABLE`                | `CREATE TABLE users (id INT PRIMARY KEY, name VARCHAR(50));` |
| Añadir columna    | `ALTER TABLE ... ADD COLUMN`  | `ALTER TABLE users ADD COLUMN email VARCHAR(100);`           |
| Modificar columna | `ALTER TABLE ... MODIFY`      | `ALTER TABLE users MODIFY COLUMN name VARCHAR(100);`         |
| Eliminar columna  | `ALTER TABLE ... DROP COLUMN` | `ALTER TABLE users DROP COLUMN email;`                       |
| Eliminar tabla    | `DROP TABLE`                  | `DROP TABLE users;`                                          |

---

### 3. Cláusulas Básicas

**Descripción:** Cláusulas esenciales para consultar datos.

| Descripción          | Función / Característica | Ejemplo                                                                               |
| -------------------- | ------------------------ | ------------------------------------------------------------------------------------- |
| Seleccionar columnas | `SELECT`                 | `SELECT id, name FROM users;`                                                         |
| Filtrar filas        | `WHERE`                  | `SELECT * FROM users WHERE is_active = TRUE;`                                         |
| Ordenar resultados   | `ORDER BY`               | `SELECT * FROM users ORDER BY name ASC;`                                              |
| Agrupar filas        | `GROUP BY`               | `SELECT department, COUNT(*) FROM employees GROUP BY department;`                     |
| Filtrar grupos       | `HAVING`                 | `SELECT department, COUNT(*) FROM employees GROUP BY department HAVING COUNT(*) > 5;` |

---

### 4. Joins y Relaciones

**Descripción:** Combinar filas de varias tablas.

| Descripción     | Función / Característica | Ejemplo                                                                  |
| --------------- | ------------------------ | ------------------------------------------------------------------------ |
| Inner join      | `INNER JOIN`             | `SELECT * FROM orders o INNER JOIN customers c ON o.customer_id = c.id;` |
| Left join       | `LEFT JOIN`              | `SELECT * FROM orders o LEFT JOIN customers c ON o.customer_id = c.id;`  |
| Right join      | `RIGHT JOIN`             | `SELECT * FROM orders o RIGHT JOIN customers c ON o.customer_id = c.id;` |
| Full outer join | `FULL OUTER JOIN`        | `SELECT * FROM a FULL OUTER JOIN b ON a.id = b.id;`                      |

---

### 5. Funciones de Agregado

**Descripción:** Funciones para resumir datos.

| Descripción   | Función / Característica | Ejemplo                              |
| ------------- | ------------------------ | ------------------------------------ |
| Contar filas  | `COUNT()`                | `SELECT COUNT(*) FROM users;`        |
| Sumar valores | `SUM()`                  | `SELECT SUM(salary) FROM employees;` |
| Promedio      | `AVG()`                  | `SELECT AVG(salary) FROM employees;` |
| Valor máximo  | `MAX()`                  | `SELECT MAX(salary) FROM employees;` |
| Valor mínimo  | `MIN()`                  | `SELECT MIN(salary) FROM employees;` |

---

### 6. Funciones de Texto

**Descripción:** Funciones para manipular cadenas de texto.

| Descripción        | Función / Característica | Ejemplo                                                 |
| ------------------ | ------------------------ | ------------------------------------------------------- |
| Concatenar cadenas | `CONCAT()`               | `SELECT CONCAT(first_name, ' ', last_name) FROM users;` |
| Subcadena          | `SUBSTRING()`            | `SELECT SUBSTRING(name, 1, 3) FROM users;`              |
| Longitud           | `LENGTH()`               | `SELECT LENGTH(name) FROM users;`                       |
| Mayúsculas         | `UPPER()`                | `SELECT UPPER(name) FROM users;`                        |
| Minúsculas         | `LOWER()`                | `SELECT LOWER(name) FROM users;`                        |

---

### 7. Funciones de Fecha y Hora

**Descripción:** Funciones para trabajar con valores de fecha y hora.

| Descripción               | Función / Característica | Ejemplo                                       |
| ------------------------- | ------------------------ | --------------------------------------------- |
| Fecha y hora actual       | `NOW()`                  | `SELECT NOW();`                               |
| Agregar intervalo         | `DATEADD()`              | `SELECT DATEADD(day, 7, NOW());`              |
| Diferencia entre fechas   | `DATEDIFF()`             | `SELECT DATEDIFF('2026-03-26','2026-03-01');` |
| Extraer parte de la fecha | `EXTRACT()`              | `SELECT EXTRACT(YEAR FROM NOW());`            |

---

### 8. Funciones Numéricas

**Descripción:** Funciones para operaciones numéricas.

| Descripción      | Función / Característica | Ejemplo                    |
| ---------------- | ------------------------ | -------------------------- |
| Redondear número | `ROUND()`                | `SELECT ROUND(3.14159,2);` |
| Techo            | `CEIL()`                 | `SELECT CEIL(3.14);`       |
| Piso             | `FLOOR()`                | `SELECT FLOOR(3.14);`      |
| Valor absoluto   | `ABS()`                  | `SELECT ABS(-5);`          |

---

### 9. Subconsultas

**Descripción:** Consultas anidadas dentro de otra consulta.

| Descripción           | Función / Característica    | Ejemplo                                                                                              |
| --------------------- | --------------------------- | ---------------------------------------------------------------------------------------------------- |
| Subconsulta en SELECT | `SELECT ... (SELECT ...)`   | `SELECT name, (SELECT COUNT(*) FROM orders WHERE customer_id = users.id) AS order_count FROM users;` |
| Subconsulta en WHERE  | `WHERE ... IN (SELECT ...)` | `SELECT * FROM users WHERE id IN (SELECT customer_id FROM orders);`                                  |

---

### 10. Operadores

**Descripción:** Operadores lógicos y de comparación.

| Descripción     | Función / Característica | Ejemplo                                                     |
| --------------- | ------------------------ | ----------------------------------------------------------- |
| Igual           | `=`                      | `SELECT * FROM users WHERE id = 1;`                         |
| Diferente       | `!=` o `<>`              | `SELECT * FROM users WHERE id != 1;`                        |
| Mayor que       | `>`                      | `SELECT * FROM users WHERE salary > 50000;`                 |
| Menor que       | `<`                      | `SELECT * FROM users WHERE salary < 50000;`                 |
| Y (AND)         | `AND`                    | `SELECT * FROM users WHERE active = TRUE AND role='admin';` |
| O (OR)          | `OR`                     | `SELECT * FROM users WHERE role='admin' OR role='manager';` |
| IN              | `IN`                     | `SELECT * FROM users WHERE id IN (1,2,3);`                  |
| ENTRE (BETWEEN) | `BETWEEN`                | `SELECT * FROM orders WHERE total BETWEEN 100 AND 500;`     |
| LIKE            | `LIKE`                   | `SELECT * FROM users WHERE name LIKE 'J%';`                 |

---

### 11. Índices y Restricciones

**Descripción:** Asegurar la integridad de los datos y mejorar el rendimiento de las consultas.

| Descripción       | Función / Característica | Ejemplo                                             |
| ----------------- | ------------------------ | --------------------------------------------------- |
| Clave primaria    | `PRIMARY KEY`            | `id INT PRIMARY KEY`                                |
| Clave foránea     | `FOREIGN KEY`            | `FOREIGN KEY(customer_id) REFERENCES customers(id)` |
| Único             | `UNIQUE`                 | `email VARCHAR(100) UNIQUE`                         |
| Restricción CHECK | `CHECK`                  | `salary INT CHECK (salary>0)`                       |
| Crear índice      | `CREATE INDEX`           | `CREATE INDEX idx_name ON users(name);`             |

---

### 12. Transacciones y Concurrencia

**Descripción:** Comandos para gestionar transacciones.

| Descripción           | Función / Característica | Ejemplo          |
| --------------------- | ------------------------ | ---------------- |
| Iniciar transacción   | `BEGIN TRANSACTION`      | `BEGIN;`         |
| Confirmar transacción | `COMMIT`                 | `COMMIT;`        |
| Revertir transacción  | `ROLLBACK`               | `ROLLBACK;`      |
| Punto de guardado     | `SAVEPOINT`              | `SAVEPOINT sp1;` |

---

### 13. Procedimientos Almacenados y Triggers

**Descripción:** Código SQL reutilizable y acciones automatizadas.

| Descripción                    | Función / Característica | Ejemplo                                                                                            |
| ------------------------------ | ------------------------ | -------------------------------------------------------------------------------------------------- |
| Crear procedimiento almacenado | `CREATE PROCEDURE`       | `CREATE PROCEDURE AddUser(IN name VARCHAR(50)) BEGIN INSERT INTO users(name) VALUES(name); END;`   |
| Ejecutar procedimiento         | `CALL`                   | `CALL AddUser('John');`                                                                            |
| Crear trigger                  | `CREATE TRIGGER`         | `CREATE TRIGGER trg_before_insert BEFORE INSERT ON users FOR EACH ROW SET NEW.created_at = NOW();` |

---

### 14. Vistas y CTE

**Descripción:** Tablas virtuales y consultas reutilizables.

| Descripción                    | Función / Característica | Ejemplo                                                                                                                              |
| ------------------------------ | ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ |
| Crear vista                    | `CREATE VIEW`            | `CREATE VIEW active_users AS SELECT * FROM users WHERE active = TRUE;`                                                               |
| Expresión de Tabla Común (CTE) | `WITH`                   | `WITH dept_count AS (SELECT department, COUNT(*) AS cnt FROM employees GROUP BY department) SELECT * FROM dept_count WHERE cnt > 5;` |

---

### 15. Utilidades Avanzadas

**Descripción:** Funciones y características SQL avanzadas.

| Descripción           | Función / Característica | Ejemplo                                                                          |
| --------------------- | ------------------------ | -------------------------------------------------------------------------------- |
| Limitar filas         | `LIMIT`                  | `SELECT * FROM users LIMIT 10;`                                                  |
| Desplazar filas       | `OFFSET`                 | `SELECT * FROM users LIMIT 10 OFFSET 5;`                                         |
| Expresión CASE        | `CASE`                   | `SELECT name, CASE WHEN salary>50000 THEN 'High' ELSE 'Low' END FROM employees;` |
| Función COALESCE      | `COALESCE`               | `SELECT COALESCE(nickname, name) FROM users;`                                    |
| CAST / Convertir tipo | `CAST`                   | `SELECT CAST(salary AS DECIMAL(10,2)) FROM employees;`                           |

---

