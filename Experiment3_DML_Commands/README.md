# Experiment 3: DML Commands

## AIM
To study and implement DML (Data Manipulation Language) commands.

## THEORY
### 1. INSERT INTO
Used to add records into a relation.
These are three type of INSERT INTO queries which are as
A)Inserting a single record
**Syntax (Single Row):**
```sql
INSERT INTO table_name (field_1, field_2, ...) VALUES (value_1, value_2, ...);
```
**Syntax (Multiple Rows):**
```sql
INSERT INTO table_name (field_1, field_2, ...) VALUES
(value_1, value_2, ...),
(value_3, value_4, ...);
```
**Syntax (Insert from another table):**
```sql
INSERT INTO table_name SELECT * FROM other_table WHERE condition;
```
### 2. UPDATE
Used to modify records in a relation.
Syntax:
```sql
UPDATE table_name SET column1 = value1, column2 = value2 WHERE condition;
```
### 3. DELETE
Used to delete records from a relation.
**Syntax (All rows):**
```sql
DELETE FROM table_name;
```
**Syntax (Specific condition):**
```sql
DELETE FROM table_name WHERE condition;
```
### 4. SELECT
Used to retrieve records from a table.
**Syntax:**
```sql
SELECT column1, column2 FROM table_name WHERE condition;
```
**Question 1**

<img width="847" height="442" alt="image" src="https://github.com/user-attachments/assets/b1eda72f-dbfd-47fe-b607-f3d40d616c13" />

sql :

<img width="753" height="55" alt="image" src="https://github.com/user-attachments/assets/c9aeeccc-01ae-44a7-bb16-7876a564b2d0" />

**Output:**

<img width="840" height="207" alt="image" src="https://github.com/user-attachments/assets/7f6b7db2-2577-4cd8-a84a-0f828c45324a" />
<img width="851" height="192" alt="image" src="https://github.com/user-attachments/assets/3f7409ad-711f-4bda-b15a-5a9a910b90c4" />


**Question 2**

<img width="847" height="401" alt="image" src="https://github.com/user-attachments/assets/730b5518-8375-4e70-8f61-aa7c3c993ab9" />

sql :

<img width="670" height="76" alt="image" src="https://github.com/user-attachments/assets/b285b26b-e83d-44e4-ab7f-143ad71beb59" />

**Output:**

<img width="836" height="128" alt="image" src="https://github.com/user-attachments/assets/1acf0a38-3b12-467c-8bc8-ac3e7b6dd245" />
<img width="845" height="342" alt="image" src="https://github.com/user-attachments/assets/ad5044d8-efe4-4634-84bf-eef441730a44" />


**Question 3**

<img width="837" height="363" alt="image" src="https://github.com/user-attachments/assets/e60cd598-8375-49cb-8b82-87e158e0ae24" />

sql :

<img width="568" height="71" alt="image" src="https://github.com/user-attachments/assets/fc417f1e-1efd-46d7-983e-60481ab1f87a" />

**Output:**

<img width="833" height="127" alt="image" src="https://github.com/user-attachments/assets/93273df2-17f2-455b-904a-6c595cac4726" />
<img width="837" height="452" alt="image" src="https://github.com/user-attachments/assets/caf99085-2ae4-4452-b3ed-759cdc223fc8" />


**Question 4**

<img width="837" height="347" alt="image" src="https://github.com/user-attachments/assets/321e383c-1142-467b-be17-0347c3d8323a" />

sql :

<img width="590" height="67" alt="image" src="https://github.com/user-attachments/assets/a6ca0a16-4a8a-4a85-85b6-b332c2d8692e" />

**Output:**

<img width="565" height="632" alt="image" src="https://github.com/user-attachments/assets/aa647b8b-784b-4f43-a6de-efcf57485bbb" />


**Question 5**

<img width="578" height="268" alt="image" src="https://github.com/user-attachments/assets/80a71f11-c0f5-405e-9588-455e8e1ef047" />

sql :

<img width="475" height="55" alt="image" src="https://github.com/user-attachments/assets/bce43999-c2e8-4170-bd74-f484ed53fb84" />


**Output:**

<img width="705" height="290" alt="image" src="https://github.com/user-attachments/assets/f1e8f410-59df-43c7-96c7-4a81f4a27b20" />

**Question 6**

<img width="806" height="337" alt="image" src="https://github.com/user-attachments/assets/adaf499e-c866-487a-8944-f0e4efbe3bb4" />


sql :

<img width="281" height="51" alt="image" src="https://github.com/user-attachments/assets/b3a5684d-4f32-41ae-bc66-61bff05b7f36" />

**Output:**

<img width="797" height="222" alt="image" src="https://github.com/user-attachments/assets/0a024b2d-565a-407b-a8f2-c5c84110a390" />

**Question 7**

<img width="780" height="372" alt="image" src="https://github.com/user-attachments/assets/9c0728e8-9378-4da5-8e4b-135b129bdbd4" />

sql :

<img width="797" height="77" alt="image" src="https://github.com/user-attachments/assets/fb413c4b-c35c-44ef-a74d-df9def3a23c8" />

**Output:**

<img width="786" height="197" alt="image" src="https://github.com/user-attachments/assets/eeb06b6d-f873-43e4-ac93-e71846eaa426" />

**Question 8**

<img width="810" height="153" alt="image" src="https://github.com/user-attachments/assets/ba4c3a7a-86f4-425a-8ced-c8e09e398e80" />

sql :

<img width="456" height="72" alt="image" src="https://github.com/user-attachments/assets/c23c9322-e2a0-45b5-9f41-e7cb271cd3cf" />

**Output:**

<img width="787" height="175" alt="image" src="https://github.com/user-attachments/assets/e6dccecd-7653-425a-b406-cef29fa3124a" />

**Question 9**

<img width="795" height="301" alt="image" src="https://github.com/user-attachments/assets/452272b2-af63-43e1-aaae-985533fd3b09" />

sql :

<img width="670" height="41" alt="image" src="https://github.com/user-attachments/assets/a110c474-f189-44b6-848a-d96d76920380" />

**Output:**

<img width="775" height="357" alt="image" src="https://github.com/user-attachments/assets/354e6f41-0388-41b2-b93e-9bbe244d52a3" />

**Question 10**

<img width="800" height="226" alt="image" src="https://github.com/user-attachments/assets/731fb8f8-2f77-4cb3-9e95-0f7ded82a8a3" />

sql :

<img width="792" height="85" alt="image" src="https://github.com/user-attachments/assets/7cc916bf-13a6-4029-be88-768c79cc4628" />

**Output:**

<img width="800" height="215" alt="image" src="https://github.com/user-attachments/assets/1a513241-1a33-4167-88b2-8c63ac1a0662" />

## RESULT
Thus, the SQL queries to implement DML commands have been executed successfully.
