# Experiment 6: Joins

## AIM
To study and implement different types of joins.

## THEORY

SQL Joins are used to combine records from two or more tables based on a related column.
JOINS

### 1. INNER JOIN
Returns records with matching values in both tables.

**Syntax:**
```sql
SELECT columns
FROM table1
INNER JOIN table2
ON table1.column = table2.column;
```

### 2. LEFT JOIN
Returns all records from the left table, and matched records from the right.

**Syntax:**

```sql

SELECT columns
FROM table1
LEFT JOIN table2
ON table1.column = table2.column;
```
### 3. RIGHT JOIN
Returns all records from the right table, and matched records from the left.

**Syntax:**

```sql
SELECT columns
FROM table1
RIGHT JOIN table2
ON table1.column = table2.column;
```
### 4. FULL OUTER JOIN
Returns all records when there is a match in either left or right table.

**Syntax:**

```sql
SELECT columns
FROM table1
FULL OUTER JOIN table2
ON table1.column = table2.column;
```

**Question 1**

<img width="828" height="475" alt="image" src="https://github.com/user-attachments/assets/da6498f3-e7a8-439e-90d9-22322b9cafda" />

SQL :

<img width="570" height="107" alt="image" src="https://github.com/user-attachments/assets/f74fccc0-fc00-420d-ad17-34cc9424d77d" />

**Output:**

<img width="826" height="386" alt="image" src="https://github.com/user-attachments/assets/9c3a94e0-1263-4ad9-bbaf-a06af67ad747" />

**Question 2**

<img width="831" height="447" alt="image" src="https://github.com/user-attachments/assets/2e044cb0-5e30-474e-9be0-ac094fc10f0a" />

SQL :

<img width="511" height="110" alt="image" src="https://github.com/user-attachments/assets/3fd46f4c-4981-4dee-b490-1997488fd49e" />

**Output:**

<img width="827" height="198" alt="image" src="https://github.com/user-attachments/assets/10427796-f5fb-4bf5-ad3f-ed616f3f6576" />

**Question 3**

<img width="850" height="566" alt="image" src="https://github.com/user-attachments/assets/2425ae73-1e8d-4738-90b0-549203229455" />

SQL :

<img width="690" height="102" alt="image" src="https://github.com/user-attachments/assets/f40bd308-d8b2-46dd-a1dd-125c11204310" />

**Output:**

<img width="480" height="137" alt="image" src="https://github.com/user-attachments/assets/3855ff12-1110-4342-85e8-39aa6d54ba4e" />

**Question 4**

<img width="851" height="562" alt="image" src="https://github.com/user-attachments/assets/1c717ee1-b8ea-4ed2-a9d7-a6c40c8d37a4" />

SQL :

<img width="597" height="131" alt="image" src="https://github.com/user-attachments/assets/269cb464-3626-4904-b46b-7fd28f5cd776" />

**Output:**

<img width="827" height="315" alt="image" src="https://github.com/user-attachments/assets/fe0568f9-4e01-46fe-bd5b-d35925c98813" />

**Question 5**

<img width="831" height="465" alt="image" src="https://github.com/user-attachments/assets/d79488fc-1e76-4fda-a003-7d9d21c40ad0" />

SQL :

<img width="575" height="116" alt="image" src="https://github.com/user-attachments/assets/74acfc40-2640-474e-8626-ae0affffada0" />

**Output:**

<img width="848" height="386" alt="image" src="https://github.com/user-attachments/assets/a968c220-27d0-441b-b64e-6f71dca5f211" />

**Question 6**

<img width="833" height="551" alt="image" src="https://github.com/user-attachments/assets/831caebf-1a2d-47f0-a116-26e4548b0bf8" />

SQL :

<img width="475" height="127" alt="image" src="https://github.com/user-attachments/assets/18164418-83f4-490a-b1f0-93448b3d3ab6" />

**Output:**

<img width="831" height="372" alt="image" src="https://github.com/user-attachments/assets/ba3774b5-b4c9-4588-a56e-f0e3455053d4" />

**Question 7**

<img width="845" height="642" alt="image" src="https://github.com/user-attachments/assets/6f996b41-674b-42ec-90c8-a2d8d3e7d62e" />

SQL :

<img width="410" height="85" alt="image" src="https://github.com/user-attachments/assets/337bb44f-16c2-47b1-8691-f8f58c52421b" />

**Output:**

<img width="796" height="486" alt="image" src="https://github.com/user-attachments/assets/6e259522-6602-4411-bd50-12322d2b2961" />

**Question 8**

<img width="841" height="527" alt="image" src="https://github.com/user-attachments/assets/337ee1bf-b7c6-4a0f-beb1-5f6ea898879c" />

SQL :

<img width="617" height="125" alt="image" src="https://github.com/user-attachments/assets/61685854-6188-4bc4-b650-d803a053bf5c" />

**Output:**

<img width="850" height="367" alt="image" src="https://github.com/user-attachments/assets/5c4acea2-727e-422c-a0d2-57e4134b6037" />

**Question 9**

<img width="841" height="612" alt="image" src="https://github.com/user-attachments/assets/4fcafee9-25a1-4e36-a7cb-4bb5f9e142d0" />

SQL :

<img width="445" height="87" alt="image" src="https://github.com/user-attachments/assets/6ed42b69-4b65-4675-83be-e6fe6d8f66fc" />

**Output:**

<img width="605" height="272" alt="image" src="https://github.com/user-attachments/assets/124bbbe2-698a-4d47-b1a9-53897314d78c" />

**Question 10**

<img width="845" height="480" alt="image" src="https://github.com/user-attachments/assets/4395039b-451a-4445-8357-424020de6643" />

SQL :

<img width="776" height="117" alt="image" src="https://github.com/user-attachments/assets/d6f190fe-86f3-4023-b425-ab6ca69c516a" />

**Output:**

<img width="832" height="272" alt="image" src="https://github.com/user-attachments/assets/bfa37739-84a5-4ef2-958e-481f3e03279e" />

## RESULT
Thus, the SQL queries to implement different types of joins have been executed successfully.
