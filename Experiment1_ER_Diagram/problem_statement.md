## Name   : Gugapriya P 
## Reg No : 212223060075

## Objective
To understand and apply ER modeling concepts by creating ER diagrams for real-world applications.

## Purpose
Gain hands-on experience in designing ER diagrams that represent database structure including entities, relationships, attributes, and constraints.

---

# Scenario A: City Fitness Club Management

**Business Context:**  
FlexiFit Gym wants a database to manage its members, trainers, and fitness programs.

**Requirements:**  
- Members register with name, membership type, and start date.  
- Each member can join multiple programs (Yoga, Zumba, Weight Training).  
- Trainers assigned to programs; a program may have multiple trainers.  
- Members may book personal training sessions with trainers.  
- Attendance recorded for each session.  
- Payments tracked for memberships and sessions.

### ER Diagram:
<img width="884" height="623" alt="image" src="https://github.com/user-attachments/assets/2c12aab7-d6a1-4f52-8ec4-56cd5acc0517" />

### Entities and Attributes

| Entity  | Attributes (PK, FK)                                                     | Notes                             |
| ------- | ----------------------------------------------------------------------- | --------------------------------- |
| Member  | MemberID (PK), MemberName, MembershipType, StartDate                    | Stores member details             |
| Program | ProgramID (PK), ProgramName, ProgramType, Duration                      | Stores fitness program details    |
| Trainer | TrainerID (PK), TrainerName, Specialization, Phone                      | Stores trainer details            |
| Session | SessionID (PK), SessionDate, SessionTime, MemberID (FK), TrainerID (FK) | Stores personal training sessions |
| Payment | PaymentID (PK), MemberID (FK), SessionID (FK), Amount, PaymentDate      | Stores payment details            |


### Relationships and Constraints

| Relationship                | Cardinality | Participation | Notes                                   |
| --------------------------- | ----------- | ------------- | --------------------------------------- |
| Member joins Program        | M:N         | Partial       | A member can join many programs         |
| Trainer assigned to Program | M:N         | Partial       | A program can have many trainers        |
| Member books Session        | 1:N         | Partial       | A member can book many sessions         |
| Trainer conducts Session    | 1:N         | Partial       | A trainer can conduct many sessions     |
| Session has Attendance      | 1:1         | Total         | Attendance is recorded for each session |
| Member makes Payment        | 1:N         | Partial       | A member can make many payments         |


### Assumptions
- Each member, trainer, program, session and payment has a unique ID.
- A member can join more than one fitness program.
- A trainer can handle more than one program and training session.
- Payment is recorded for membership or personal training sessions.

---

# Scenario B: City Library Event & Book Lending System

**Business Context:**  
The Central Library wants to manage book lending and cultural events.

**Requirements:**  
- Members borrow books, with loan and return dates tracked.  
- Each book has title, author, and category.  
- Library organizes events; members can register.  
- Each event has one or more speakers/authors.  
- Rooms are booked for events and study.  
- Overdue fines apply for late returns.

### ER Diagram:
<img width="932" height="619" alt="image" src="https://github.com/user-attachments/assets/a4e361aa-d119-46ac-9f4b-6ac8dfee9ede" />

### Entities and Attributes

| Entity       | Attributes (PK, FK)                                           | Notes                         |
| ------------ | ------------------------------------------------------------- | ----------------------------- |
| Member       | MemberID (PK), MemberName, Email, Phone                       | Stores library member details |
| Book         | BookID (PK), Title, Author, Category                          | Stores book details           |
| Loan         | LoanID (PK), MemberID (FK), BookID (FK), LoanDate, ReturnDate | Keeps track of borrowed books |
| Event        | EventID (PK), EventName, EventDate, Description               | Stores library event details  |
| Room         | RoomID (PK), RoomName, Capacity                               | Stores room details           |
| Speaker      | SpeakerID (PK), SpeakerName, AuthorName, Contact              | Stores speaker details        |
| Fine         | FineID (PK), LoanID (FK), Amount, FineDate                    | Stores overdue fine details   |
| EventSpeaker | EventID (FK), SpeakerID (FK)                                  | Connects events with speakers |


### Relationships and Constraints

| Relationship               | Cardinality | Participation | Notes                                  |
| -------------------------- | ----------- | ------------- | -------------------------------------- |
| Member borrows Book        | M:N         | Partial       | A member can borrow many books         |
| Member registers for Event | M:N         | Partial       | A member can register for many events  |
| Event uses Room            | N:1         | Total         | An event is held in one room           |
| Event has Speaker          | M:N         | Total         | An event can have one or more speakers |
| Book has Loan              | 1:N         | Partial       | A book can be borrowed many times      |
| Loan generates Fine        | 1:0..1      | Partial       | Fine is given only for late returns    |

### Assumptions

- A member can borrow more than one book at a time.
- A room can be used for different events at different times.
- A fine is given only when a book is returned late.

---

# Scenario C: Restaurant Table Reservation & Ordering

**Business Context:**  
A popular restaurant wants to manage reservations, orders, and billing.

**Requirements:**  
- Customers can reserve tables or walk in.  
- Each reservation includes date, time, and number of guests.  
- Customers place food orders linked to reservations.  
- Each order contains multiple dishes; dishes belong to categories (starter, main, dessert).  
- Bills generated per reservation, including food and service charges.  
- Waiters assigned to serve reservations.

### ER Diagram:
<img width="870" height="623" alt="image" src="https://github.com/user-attachments/assets/97725227-69bc-4203-abcf-41b525b4e9ea" />

### Entities and Attributes

| Entity      | Attributes (PK, FK)                                                                         | Notes                            |
| ----------- | ------------------------------------------------------------------------------------------- | -------------------------------- |
| Customer    | CustomerID (PK), CustomerName, Phone, Email                                                 | Stores customer details          |
| Reservation | ReservationID (PK), CustomerID (FK), TableID (FK), ReservationDate, ReservationTime, Guests | Stores table reservation details |
| Table       | TableID (PK), TableNumber, Capacity, Status                                                 | Stores restaurant table details  |
| Order       | OrderID (PK), ReservationID (FK), OrderDate, TotalAmount                                    | Stores food order details        |
| Dish        | DishID (PK), DishName, Price, CategoryID (FK)                                               | Stores food item details         |
| Category    | CategoryID (PK), CategoryName                                                               | Stores dish categories           |
| OrderItem   | OrderID (PK, FK), DishID (PK, FK), Quantity                                                 | Stores dishes in each order      |
| Bill        | BillID (PK), ReservationID (FK), FoodCharge, ServiceCharge, TotalAmount                     | Stores billing details           |
| Waiter      | WaiterID (PK), WaiterName, Phone, Shift                                                     | Stores waiter details            |


### Relationships and Constraints

| Relationship               | Cardinality | Participation | Notes                                     |
| -------------------------- | ----------- | ------------- | ----------------------------------------- |
| Customer makes Reservation | 1:N         | Partial       | A customer can make many reservations     |
| Reservation has Order      | 1:N         | Partial       | A reservation can have multiple orders    |
| Order contains Dish        | M:N         | Total         | An order can contain many dishes          |
| Category has Dish          | 1:N         | Total         | A category can have many dishes           |
| Reservation uses Table     | N:1         | Total         | Each reservation is assigned to one table |
| Reservation generates Bill | 1:1         | Total         | Each reservation has one bill             |
| Waiter serves Reservation  | 1:N         | Partial       | A waiter can serve many reservations      |


### Assumptions
- Each customer has a unique CustomerID.
- A customer can make multiple reservations.
- Each reservation is assigned to one table.
- An order can contain multiple dishes.
- A bill is generated for each reservation. 
  
---

## Instructions for Students

1. Complete **all three scenarios** (A, B, C).  
2. Identify entities, relationships, and attributes for each.  
3. Draw ER diagrams using **draw.io / diagrams.net** or hand-drawn & scanned.  
4. Fill in all tables and assumptions for each scenario.  
5. Export the completed Markdown (with diagrams) as **a single PDF**
