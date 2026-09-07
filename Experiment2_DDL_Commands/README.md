# Experiment 2: DDL Commands

## AIM
To study and implement DDL commands and different types of constraints.

## THEORY

### 1. CREATE
Used to create a new relation (table).

**Syntax:**
```sql
CREATE TABLE (
  field_1 data_type(size),
  field_2 data_type(size),
  ...
);
```
### 2. ALTER
Used to add, modify, drop, or rename fields in an existing relation.
(a) ADD
```sql
ALTER TABLE std ADD (Address CHAR(10));
```
(b) MODIFY
```sql
ALTER TABLE relation_name MODIFY (field_1 new_data_type(size));
```
(c) DROP
```sql
ALTER TABLE relation_name DROP COLUMN field_name;
```
(d) RENAME
```sql
ALTER TABLE relation_name RENAME COLUMN old_field_name TO new_field_name;
```
### 3. DROP TABLE
Used to permanently delete the structure and data of a table.
```sql
DROP TABLE relation_name;
```
### 4. RENAME
Used to rename an existing database object.
```sql
RENAME TABLE old_relation_name TO new_relation_name;
```
### CONSTRAINTS
Constraints are used to specify rules for the data in a table. If there is any violation between the constraint and the data action, the action is aborted by the constraint. It can be specified when the table is created (using CREATE TABLE) or after it is created (using ALTER TABLE).
### 1. NOT NULL
When a column is defined as NOT NULL, it becomes mandatory to enter a value in that column.
Syntax:
```sql
CREATE TABLE Table_Name (
  column_name data_type(size) NOT NULL
);
```
### 2. UNIQUE
Ensures that values in a column are unique.
Syntax:
```sql
CREATE TABLE Table_Name (
  column_name data_type(size) UNIQUE
);
```
### 3. CHECK
Specifies a condition that each row must satisfy.
Syntax:
```sql
CREATE TABLE Table_Name (
  column_name data_type(size) CHECK (logical_expression)
);
```
### 4. PRIMARY KEY
Used to uniquely identify each record in a table.
Properties:
Must contain unique values.
Cannot be null.
Should contain minimal fields.
Syntax:
```sql
CREATE TABLE Table_Name (
  column_name data_type(size) PRIMARY KEY
);
```
### 5. FOREIGN KEY
Used to reference the primary key of another table.
Syntax:
```sql
CREATE TABLE Table_Name (
  column_name data_type(size),
  FOREIGN KEY (column_name) REFERENCES other_table(column)
);
```
### 6. DEFAULT
Used to insert a default value into a column if no value is specified.

Syntax:
```sql
CREATE TABLE Table_Name (
  col_name1 data_type,
  col_name2 data_type,
  col_name3 data_type DEFAULT 'default_value'
);
```

**Question 1**
<img width="817" height="258" alt="image" src="https://github.com/user-attachments/assets/c8d656a7-cdf5-4664-a186-d0b94285f408" />

sql
<img width="626" height="135" alt="image" src="https://github.com/user-attachments/assets/aa547cf6-ad2f-4e1a-aa87-6670b66f34c3" />

**Output:**
<img width="856" height="207" alt="image" src="https://github.com/user-attachments/assets/95bee9b7-7a4a-4428-8a89-9d5b029917a2" />


**Question 2**

<img width="836" height="297" alt="image" src="https://github.com/user-attachments/assets/dabba20a-f9d0-4249-a325-33f10e7eff40" />

sql :
<img width="650" height="122" alt="image" src="https://github.com/user-attachments/assets/eac4da82-3e83-41b0-a851-37f4cafaed01" />

**Output:**

<img width="841" height="387" alt="image" src="https://github.com/user-attachments/assets/87ba4658-4d68-4708-ac33-192455d0477a" />


**Question 3**

sql :
<img width="595" height="82" alt="image" src="https://github.com/user-attachments/assets/1e0714fd-c5a1-46d6-9cad-47d221cba2e9" />

**Output:**

<img width="850" height="290" alt="image" src="https://github.com/user-attachments/assets/3ee00c77-eb33-44b0-9621-be0c6bb92196" />

**Question 4**

<img width="816" height="287" alt="image" src="https://github.com/user-attachments/assets/3c48a7d4-9eaa-466b-8fe4-b8939b5aaaa6" />

sql :

<img width="385" height="95" alt="image" src="https://github.com/user-attachments/assets/38ca1689-e128-479c-a83b-eee8385ecb9c" />

**Output:**

<img width="857" height="353" alt="image" src="https://github.com/user-attachments/assets/d939f378-09ca-4561-bd4b-8b443c19f711" />

**Question 5**

<img width="855" height="371" alt="image" src="https://github.com/user-attachments/assets/f655bade-afae-45d7-8181-1f6714e2c952" />

sql :

<img width="567" height="97" alt="image" src="https://github.com/user-attachments/assets/02398e40-c018-4844-8acb-bc729aa063c4" />

**Output:**

<img width="837" height="230" alt="image" src="https://github.com/user-attachments/assets/105f8a94-32b3-4fb4-810e-b3063ce76bb8" />

**Question 6**

<img width="795" height="323" alt="image" src="https://github.com/user-attachments/assets/0b5c61ae-26e9-4fa5-9f3a-54f60e6ffc0d" />

sql :

<img width="470" height="128" alt="image" src="https://github.com/user-attachments/assets/fe9fcda6-9103-408a-b0d2-10b08daceee6" />

**Output:**

<img width="860" height="293" alt="image" src="https://github.com/user-attachments/assets/2a01abae-6ac1-43cf-ba42-a6641a4d6cb9" />

**Question 7**

<img width="845" height="273" alt="image" src="https://github.com/user-attachments/assets/b92d069e-0b89-406d-8fab-4571e19d6f41" />

sql :

<img width="601" height="55" alt="image" src="https://github.com/user-attachments/assets/26e0ccd3-a07a-46f6-92f8-148eb80bd716" />

**Output:**

<img width="827" height="216" alt="image" src="https://github.com/user-attachments/assets/e267cdbf-ac7a-4e0b-af1f-eb3c3a9a0a25" />

**Question 8**

<img width="850" height="342" alt="image" src="https://github.com/user-attachments/assets/714e0408-15c0-45a8-afe2-11a1b6db1bc2" />

sql :

<img width="520" height="145" alt="image" src="https://github.com/user-attachments/assets/2c218fdb-2ca9-4fb2-a6f3-31344b39bc60" />

**Output:**

<img width="840" height="353" alt="image" src="https://github.com/user-attachments/assets/b90ddf85-7abc-4543-a66c-ad5a95dec752" />

**Question 9**

<img width="782" height="323" alt="image" src="https://github.com/user-attachments/assets/59d72757-5188-42ee-92d4-986cc42b79e6" />

sql :

<img width="523" height="131" alt="image" src="https://github.com/user-attachments/assets/772eb24c-e77d-4afc-8478-9375595cc1e0" />

**Output:**

<img width="832" height="291" alt="image" src="https://github.com/user-attachments/assets/dabea851-97c2-4560-b55f-863399d00db2" />
<img width="836" height="223" alt="image" src="https://github.com/user-attachments/assets/8d7aed5d-7c8f-483b-a50e-b488b45f1d6d" />

**Question 10**

<img width="845" height="432" alt="image" src="https://github.com/user-attachments/assets/335e9fc9-0e58-4e5d-beca-12cb193c67b3" />

sql :

<img width="420" height="47" alt="image" src="https://github.com/user-attachments/assets/fe938329-8681-4722-9562-13e9cb6609bf" />

**Output:**

<img width="851" height="416" alt="image" src="https://github.com/user-attachments/assets/02141475-633b-47f8-a11d-acab77310f6a" />


## RESULT
Thus, the SQL queries to implement different types of constraints and DDL commands have been executed successfully.
