
## **1. Basic Database Concepts**  

### **1. What is a database?**  
A **database** is a structured collection of data that allows efficient storage, retrieval, and manipulation of information.  

### **2. What is the difference between SQL and NoSQL databases?**  
- **SQL (Relational Database):** Structured, follows a schema, uses tables (e.g., MySQL, PostgreSQL).  
- **NoSQL (Non-Relational Database):** Schema-less, stores data in key-value, document, column, or graph formats (e.g., MongoDB, Cassandra).  

### **3. What are ACID properties in databases?**  
- **Atomicity:** A transaction is either fully completed or not at all.  
- **Consistency:** Maintains database integrity before and after transactions.  
- **Isolation:** Transactions execute independently without interference.  
- **Durability:** Ensures committed transactions persist even after a system failure.  

### **4. What is normalization, and why is it important?**  
Normalization organizes data to reduce redundancy and improve integrity. It prevents anomalies in data storage and ensures efficient data handling.  

### **5. What are the different normal forms in database normalization?**  
- **1NF:** Eliminates duplicate columns and ensures atomicity.  
- **2NF:** Removes partial dependency (each attribute must depend on the whole primary key).  
- **3NF:** Eliminates transitive dependency (non-key attributes must depend only on the primary key).  
- **BCNF (Boyce-Codd Normal Form):** Stronger version of 3NF, resolving more anomalies.  

---

## **2. Database Keys and Constraints**  

### **6. What is a primary key?**  
A **primary key** uniquely identifies each record in a table and cannot be NULL.  

### **7. What is the difference between a primary key and a unique key?**  
- **Primary Key:** Uniquely identifies records and cannot be NULL.  
- **Unique Key:** Ensures uniqueness but allows NULL values.  

### **8. What is a foreign key?**  
A **foreign key** is a column that establishes a relationship between two tables by referencing the primary key of another table.  

### **9. What are constraints in a database?**  
Constraints enforce rules to maintain data integrity. Examples include:  
- **NOT NULL:** Prevents NULL values.  
- **UNIQUE:** Ensures uniqueness of values.  
- **CHECK:** Validates data against a condition.  
- **DEFAULT:** Assigns default values.  

### **10. What is referential integrity?**  
Referential integrity ensures that foreign key values always reference valid primary keys, preventing orphaned records.  

---

## **3. Indexing and Performance Optimization**  

### **11. What is an index in a database?**  
An **index** is a data structure that improves search performance by allowing faster data retrieval but increases storage requirements.  

### **12. What is the difference between a clustered and non-clustered index?**  
- **Clustered Index:** Determines the physical order of data in a table (one per table).  
- **Non-Clustered Index:** Maintains a separate structure pointing to the actual data (multiple allowed per table).  

### **13. What is a covering index?**  
A covering index contains all the columns needed for a query, reducing the need to access the table itself.  

### **14. What is database fragmentation?**  
Fragmentation occurs when data is stored inefficiently, leading to wasted space and slow performance. It can be **internal (within pages)** or **external (spread across disks)**.  

### **15. What is database partitioning?**  
Partitioning divides large tables into smaller, manageable pieces to improve performance and scalability. Types include:  
- **Horizontal Partitioning:** Splitting rows into multiple tables.  
- **Vertical Partitioning:** Splitting columns into multiple tables.  

---

## **4. Transactions and Concurrency Control**  

### **16. What is a database transaction?**  
A transaction is a sequence of SQL operations executed as a single unit, following **ACID properties**.  

### **17. What is the difference between COMMIT and ROLLBACK?**  
- **COMMIT:** Saves all changes made in a transaction permanently.  
- **ROLLBACK:** Reverts changes if an error occurs or a failure happens.  

### **18. What is a deadlock?**  
A **deadlock** occurs when two transactions wait for each other to release resources, preventing further execution.  

### **19. How do you prevent deadlocks?**  
- Use **consistent locking order**.  
- Keep **transactions short**.  
- Use **lower isolation levels** where possible.  

### **20. What is optimistic vs. pessimistic locking?**  
- **Optimistic Locking:** Assumes conflicts are rare and checks for conflicts before committing changes.  
- **Pessimistic Locking:** Locks records to prevent conflicts during a transaction.  

---

## **5. NoSQL and Distributed Databases**  

### **21. What are the types of NoSQL databases?**  
- **Key-Value Store (e.g., Redis, DynamoDB)**  
- **Document Store (e.g., MongoDB, CouchDB)**  
- **Column-Family Store (e.g., Cassandra, HBase)**  
- **Graph Database (e.g., Neo4j)**  

### **22. What is the CAP theorem?**  
A distributed database can guarantee only two out of three:  
- **Consistency (C):** Every read gets the latest data.  
- **Availability (A):** Every request gets a response.  
- **Partition Tolerance (P):** The system continues working despite network failures.  

### **23. What is database sharding?**  
Sharding splits a large database into smaller, distributed partitions to improve performance and scalability.  

### **24. What is the difference between SQL and NoSQL in scalability?**  
- **SQL:** Scales **vertically** (by adding more resources to a single server).  
- **NoSQL:** Scales **horizontally** (by distributing data across multiple servers).  

### **25. What is database replication?**  
Replication involves copying data across multiple servers to improve availability and reliability. It can be:  
- **Master-Slave Replication:** Writes occur on the master, reads on slaves.  
- **Master-Master Replication:** Multiple nodes handle writes and sync data.  

---

## **6. Advanced Database Concepts**  

### **26. What is denormalization?**  
Denormalization adds redundancy to improve query performance, commonly used in NoSQL and analytics databases.  

### **27. What is a materialized view?**  
A **materialized view** stores query results physically for faster access, unlike regular views, which are computed dynamically.  

### **28. How do you store hierarchical data in SQL?**  
- **Adjacency List Model:** Stores parent-child relationships using a `parent_id` column.  
- **Nested Set Model:** Uses left and right values to represent hierarchy.  

### **29. What is a Common Table Expression (CTE)?**  
A CTE is a temporary result set that simplifies complex queries and recursive operations.  

### **30. What is a stored procedure, and why use it?**  
A **stored procedure** is a reusable block of SQL statements stored in the database. It improves performance and security by reducing query execution time.  

---
