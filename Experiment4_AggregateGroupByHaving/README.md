# Experiment 4: Aggregate Functions, Group By and Having Clause

## AIM
To study and implement aggregate functions, GROUP BY, and HAVING clause with suitable examples.

## THEORY
### Aggregate Functions
These perform calculations on a set of values and return a single value.

- **MIN()** – Smallest value  
- **MAX()** – Largest value  
- **COUNT()** – Number of rows  
- **SUM()** – Total of values  
- **AVG()** – Average of values

**Syntax:**
```sql
SELECT AGG_FUNC(column_name) FROM table_name WHERE condition;
```
### GROUP BY
Groups records with the same values in specified columns.
**Syntax:**
```sql
SELECT column_name, AGG_FUNC(column_name)
FROM table_name
GROUP BY column_name;
```
### HAVING
Filters the grouped records based on aggregate conditions.
**Syntax:**
```sql
SELECT column_name, AGG_FUNC(column_name)
FROM table_name
GROUP BY column_name
HAVING condition;
```

**Question 1**

<img width="797" height="355" alt="image" src="https://github.com/user-attachments/assets/f8da83db-de54-4748-9721-357df12129d0" />

SQL :

<img width="468" height="37" alt="image" src="https://github.com/user-attachments/assets/fc1de898-9c87-4ac4-86fa-23b98bf9d77a" />

**Output:**

<img width="535" height="215" alt="image" src="https://github.com/user-attachments/assets/0a467559-076d-40f1-84f7-c6a0d208e00b" />

**Question 2**

<img width="745" height="358" alt="image" src="https://github.com/user-attachments/assets/70badc3d-e2c5-4ee5-8ead-1005ddeececd" />

SQL :

<img width="478" height="30" alt="image" src="https://github.com/user-attachments/assets/cf61c1c9-0700-458a-9024-f996f8cbbce0" />

**Output:**

<img width="762" height="210" alt="image" src="https://github.com/user-attachments/assets/a98ab8ed-495f-41d0-a878-92c512d7f2b8" />

**Question 3**

<img width="873" height="340" alt="image" src="https://github.com/user-attachments/assets/49379807-a816-41c5-818c-863b7850ec1e" />

SQL :

<img width="576" height="30" alt="image" src="https://github.com/user-attachments/assets/83a27311-f8ee-49c6-b216-d64155995d2d" />

**Output:**

<img width="671" height="215" alt="image" src="https://github.com/user-attachments/assets/ff559b38-4e0a-4fd2-8ab4-6f8255550d04" />

**Question 4**

<img width="850" height="235" alt="image" src="https://github.com/user-attachments/assets/0d49e8ea-c4f7-4e08-8a45-ac1d17922bac" />

SQL :

<img width="701" height="56" alt="image" src="https://github.com/user-attachments/assets/fa25b6c8-5c73-42bf-8e3a-1c3258c348fd" />

**Output:**

<img width="742" height="300" alt="image" src="https://github.com/user-attachments/assets/42312484-e383-4b10-9c72-cb7350008df9" />

**Question 5**

<img width="782" height="420" alt="image" src="https://github.com/user-attachments/assets/8e44decf-a1ce-49d1-bff3-d4023f176dc5" />

SQL :

<img width="442" height="50" alt="image" src="https://github.com/user-attachments/assets/32fad8cb-5476-4b7a-93ee-2e0eca75f745" />

**Output:**

<img width="662" height="302" alt="image" src="https://github.com/user-attachments/assets/677ef21d-81ff-4f7b-98a7-09e1d963adec" />

**Question 6**

<img width="827" height="351" alt="image" src="https://github.com/user-attachments/assets/a0af661c-c069-4bac-8896-58e96ec755ce" />

SQL :

<img width="668" height="76" alt="image" src="https://github.com/user-attachments/assets/e38509b5-b215-4d2d-b01b-65ff93d0ffab" />

**Output:**

<img width="722" height="286" alt="image" src="https://github.com/user-attachments/assets/159ade5e-5129-4310-b9b8-6d4418a0319b" />

**Question 7**

<img width="766" height="411" alt="image" src="https://github.com/user-attachments/assets/2a540455-c25f-42fc-9313-45c8f07ccf86" />

SQL :

<img width="563" height="75" alt="image" src="https://github.com/user-attachments/assets/4e813a4d-d600-42b7-a0ad-b1c401314b7c" />

**Output:**

<img width="567" height="243" alt="image" src="https://github.com/user-attachments/assets/023ff415-5da9-46fc-9169-a7cd40d23780" />

**Question 8**

<img width="840" height="385" alt="image" src="https://github.com/user-attachments/assets/7e85dc12-4818-4e83-84de-bb9cadc52b66" />

SQL :

<img width="582" height="91" alt="image" src="https://github.com/user-attachments/assets/944b25aa-d50d-46fa-8d13-01e921f57b03" />

**Output:**

<img width="706" height="328" alt="image" src="https://github.com/user-attachments/assets/a2d60e52-a741-4594-80bb-c08b4f0af7eb" />

**Question 9**

<img width="836" height="420" alt="image" src="https://github.com/user-attachments/assets/a4d5946c-51db-460f-b862-8283121dd6f3" />

SQL :

<img width="575" height="71" alt="image" src="https://github.com/user-attachments/assets/d61aa7f6-6f0c-465a-b896-7b18019c06cf" />

**Output:**

<img width="727" height="233" alt="image" src="https://github.com/user-attachments/assets/76a329a2-3ae3-4430-a3d7-dee3da93a674" />

**Question 10**

<img width="831" height="315" alt="image" src="https://github.com/user-attachments/assets/4fe37d3c-35bf-45d2-81a0-45fc2dbe0aa4" />

SQL :

<img width="643" height="67" alt="image" src="https://github.com/user-attachments/assets/f6c0a5dd-3b08-4e6e-8a2f-f0bd6c9cfe91" />

**Output:**

<img width="665" height="220" alt="image" src="https://github.com/user-attachments/assets/3e460ca6-a33d-4dc9-8ec2-eeb6e12dea13" />


## RESULT
Thus, the SQL queries to implement aggregate functions, GROUP BY, and HAVING clause have been executed successfully.
