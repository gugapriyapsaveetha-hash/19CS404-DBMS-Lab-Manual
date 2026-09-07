# Experiment 5: Subqueries and Views

## AIM
To study and implement subqueries and views.

## THEORY

### Subqueries
A subquery is a query inside another SQL query and is embedded in:
- WHERE clause
- HAVING clause
- FROM clause

**Types:**

- **Single-row subquery**:
  Sub queries can also return more than one value. Such results should be made use along with the operators in and any.
- **Multiple-row subquery**:
  Here more than one subquery is used. These multiple sub queries are combined by means of ‘and’ & ‘or’ keywords.
- **Correlated subquery**:
  A subquery is evaluated once for the entire parent statement whereas a correlated Sub query is evaluated once per row processed by the parent statement.

**Example:**
```sql
SELECT * FROM employees
WHERE salary > (SELECT AVG(salary) FROM employees);
```
### Views
A view is a virtual table based on the result of an SQL SELECT query.
**Create View:**
```sql
CREATE VIEW view_name AS
SELECT column1, column2 FROM table_name WHERE condition;
```
**Drop View:**
```sql
DROP VIEW view_name;
```

**Question 1**

<img width="830" height="453" alt="image" src="https://github.com/user-attachments/assets/31333c9e-dc33-4154-bf08-37a0aaf3cf8a" />

SQL :

<img width="771" height="85" alt="image" src="https://github.com/user-attachments/assets/2efb89ad-5d84-4958-9114-1a23dbff14da" />

**Output:**

<img width="841" height="235" alt="image" src="https://github.com/user-attachments/assets/cc6151cb-7707-44c1-8466-9f98296f2891" />

**Question 2**

<img width="831" height="585" alt="image" src="https://github.com/user-attachments/assets/01d926af-9f72-44ac-8308-d3fcd446c5fa" />

SQL :

<img width="591" height="212" alt="image" src="https://github.com/user-attachments/assets/c94e3093-294a-4e81-a9f5-1f206c3aae36" />


**Output:**

<img width="840" height="382" alt="image" src="https://github.com/user-attachments/assets/56c743e8-c1c3-4835-ae5d-06ccb37f78c5" />


**Question 3**

<img width="831" height="511" alt="image" src="https://github.com/user-attachments/assets/6bcacddd-d2e9-4c2c-b83d-103fbf95ab22" />

SQL :

<img width="637" height="90" alt="image" src="https://github.com/user-attachments/assets/ded2f081-2fb2-452a-b25c-34f8020677d4" />

**Output:**

<img width="847" height="225" alt="image" src="https://github.com/user-attachments/assets/28e7e2be-9575-4519-9821-1dbc48c0f44f" />

**Question 4**

<img width="825" height="478" alt="image" src="https://github.com/user-attachments/assets/4114892b-7841-4ab9-9779-46944fc72fbc" />

SQL :

<img width="542" height="137" alt="image" src="https://github.com/user-attachments/assets/e4257f75-c7b8-48d4-ba51-c299e7344980" />

**Output:**

<img width="836" height="598" alt="image" src="https://github.com/user-attachments/assets/9f529e27-3f39-4ff6-b11e-f58fb4c77f44" />

**Question 5**

<img width="772" height="547" alt="image" src="https://github.com/user-attachments/assets/1f9b9696-5da1-4d64-bf4d-3c1a03b6a9ed" />

SQL :

<img width="470" height="32" alt="image" src="https://github.com/user-attachments/assets/93141d2e-fb6d-4664-b5e3-52b4dbad5573" />

**Output:**

<img width="847" height="453" alt="image" src="https://github.com/user-attachments/assets/826ca982-f3dd-4b90-ab00-323afa72b7d8" />

**Question 6**

<img width="857" height="497" alt="image" src="https://github.com/user-attachments/assets/1b27fc47-98fc-40a2-9794-9efa870317b0" />

SQL :

<img width="668" height="287" alt="image" src="https://github.com/user-attachments/assets/27280ad7-389a-4dac-8b25-07c9532f330b" />

**Output:**

<img width="811" height="380" alt="image" src="https://github.com/user-attachments/assets/4e1a324b-8eb6-48fd-a16b-f434081165b5" />

**Question 7**

<img width="583" height="113" alt="image" src="https://github.com/user-attachments/assets/379a9552-446e-4bf3-926e-d34e8056cdf9" />

SQL :

<img width="832" height="355" alt="image" src="https://github.com/user-attachments/assets/4130c9ea-b480-482d-9808-ee366522275a" />

**Output:**

<img width="846" height="472" alt="image" src="https://github.com/user-attachments/assets/997dac54-2aee-4a62-840e-43c4f8d0c622" />

**Question 8**

<img width="645" height="130" alt="image" src="https://github.com/user-attachments/assets/a51a8bdb-7b94-4770-bc84-347910a63cff" />

SQL :

<img width="597" height="277" alt="image" src="https://github.com/user-attachments/assets/f088ee63-aadb-4601-82fa-13884a2e7353" />

**Output:**

<img width="845" height="323" alt="image" src="https://github.com/user-attachments/assets/5ef8f329-2c07-44ec-bd8a-b945dd0edc53" />

**Question 9**

<img width="662" height="97" alt="image" src="https://github.com/user-attachments/assets/62180f69-89c6-48ed-bace-e6cdc2a4a11c" />

SQL :

<img width="598" height="288" alt="image" src="https://github.com/user-attachments/assets/3432b7e3-0402-4c45-b298-c6f4dac07864" />

**Output:**

<img width="850" height="395" alt="image" src="https://github.com/user-attachments/assets/00d0cdf7-4fb2-40de-b24c-492e063cd110" />

**Question 10**

<img width="605" height="133" alt="image" src="https://github.com/user-attachments/assets/a26dbed0-0a02-489a-bf31-eab3cd3ac85b" />

SQL :

<img width="833" height="340" alt="image" src="https://github.com/user-attachments/assets/2e4dad48-9b23-4a8a-b873-3c48a500346a" />

**Output:**

<img width="833" height="340" alt="image" src="https://github.com/user-attachments/assets/ef6840d9-0439-4634-af44-84e7b4bac606" />

## RESULT
Thus, the SQL queries to implement subqueries and views have been executed successfully.
