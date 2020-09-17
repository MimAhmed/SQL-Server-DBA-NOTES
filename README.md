
# How To Begin Your Career As a SQL Server DBA Notes
## Main Topics

 **1. Roles  Installation 
 2. The Table Object 
 3. Transact-SQL 
 4. Security 
 5. Backing Up DataBases**
 

# Roles
## Production DBA
Responsible for backing up, securing, monitoring and the overall health of the SQL Server boxes under your management. You'll troubleshoot outages and be the front person when that box is down. This can be very stressful if you aren't proficient with SQL Server. The learning curve to senior level is steep. The opportunities for skilled production DBAs are many. You'll be well compensated. Many production DBAs come from the windows administration side of the house.
### Example :
Performance Tuners
Datawarehouse Administrators
Database Cloud Architects
Database Architects
High Avaiability

**The role might be right**  **for you if:**

-   You like constantly learning
-   You handle stressful situations well
-   You don't mind being on call
-   You like high visibility
-   You have solid communication skills

## Development DBA
Ensure that new database code meets company standards for readability, reliability, and performance. In this role you'll be an integral part of the development team and their life cycles. You'll work as a mentor to fill the gap for developers who aren't strong with relational design. You'll be well compensated. Like the skilled production DBA there are lots of opportunies for skilled SQL developers and development DBAs. Many development DBAs come from the developer realm.

### Example:
BI Developers
SSRS Developers (Report Writers)
SSIS Developers

**The role might be right for you if:**

-   You like developing SQL code (Transact-SQL)
-   You like working in highly collaborative environments.
-   You don' want to be on-call around the clock.
-   You like authoring code over administration.
-   You come from a development background (C, C++, C#, Java)
## A Look Into The Daily Routine. A Day In The Life Of A  Production DBA.


# What is Database?


# What is a Relational DataBase?
A database is a collection of objects tables stored procedures fuse triggers. Constraints are all objects within a database. SQL Server is a RDB.

# How Table Relate to one another?
# The ACID Properties
#### Atomicity

The atomicity property identifies that the transaction is atomic.  **An atomic transaction is either fully completed**, or is not begun at all. Any updates that a transaction might affect on a system are completed in their entirety. If for any reason an error occurs and the transaction is unable to complete all of its steps, the then system is returned to the state it was in before the transaction was started.

#### Consistency

A transaction enforces  **consistency**  in the system state by ensuring that at  **the end of any transaction the system is in a valid state.**  If the transaction completes successfully, then all changes to the system will have been properly made, and the system will be in a valid state. If any error occurs in a transaction, then any changes already made will be automatically rolled back. This will return the system to its state before the transaction was started. Since the system was in a consistent state when the transaction was started, it will once again be in a consistent state.

#### Isolation

When a transaction runs in  **isolation**,  **it appears to be the only action that the system is carrying out at one time.**  If there are two transactions that are both performing the same function and are running at the same time, transaction isolation will ensure that each transaction thinks it has exclusive use of the system. This is important in that as the transaction is being executed, the state of the system may not be consistent. The transaction ensures that the system remains consistent after the transaction ends, but during an individual transaction, this may not be the case. If a transaction was not running in isolation, it could access data from the system that may not be consistent. By providing transaction isolation, this is prevented from happening.

#### Durability

**A transaction is durable in that once it has been successfully completed, all of the changes it made to the system are permanent.**  There are safeguards that will prevent the loss of information, even in the case of system failure. By logging the steps that the transaction performs, the state of the system can be recreated even if the hardware itself has failed. The concept of durability allows the developer to know that a completed transaction is a permanent part of the system, regardless of what happens to the system later on.
