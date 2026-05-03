# Mandatory II – Learning Goals

Dette dokument gennemgår samtlige learning goals fra semesterplanen.

- For **"can"-punkter**: kort snippet/eksempel + "I can do it!"
- For **"understands"/"knows"-punkter**: et par sætninger eller nøgleord der viser jeg kan forklare det.

---

## 1. Terminal og filhåndtering

### Can navigate the terminal: `ls`, `cd`, `whoami`, `pwd`.

```bash
# whoami -> cassandramichaelsen
# ls -> shows what's on my Desktop
# cd Ideaprojects -> goes to the folder
# pwd -> /Users/cassandramichaelsen/IdeaProjects
```

**I can do it!**

---

### Can create, delete files / folders: `mkdir`, `rm`, `cp`, `mv`, `touch`, `nano`.

```bash
# mkdir "hi" -> creates folder called "hi"
# touch "hey" - creates empty file called "hey"
# cp "hey" IdeaProjects -> copies "hey" to IdeaProjects
# mv "hey" "heyy" -> renames the file (can also be used for moving the file)
# rm "hey" -> deletes file called "hey"

```

**I can do it!**

---

### Can use the following basic terminal commands: `cat`, `wc`, `uniq`, `sort`.

```bash
# cat "hey" -> shows the whole file
# wc "hey" -> counts lines, words and tegn
# uniq "hey" -> removes dublicates
# sort "hey" -> sorts lines
```

**I can do it!**

---

## 2. Git og GitHub

### Can create a new repository in your preferred Git provider.

```bash
# I usually create a repo on GitHub, and from there copy the http code and clone it to IntelliJ
```

**I can do it!**

---

### Can perform basic Git operations: `clone`, `add`, `commit`, `push`, `pull`.

```bash
# git clone "url" -> clones repo 
# git add . -> adds all changed files
# git add Main.java -> adds one specific file
# git commit -m "commit-message" -> commits with a message
# git push -u origin main -> coomits to GitHub
# git pull -> opdates from remote to local branch

# Usually it goes like this:
# - git add .
# - git commit -m "adds new function"
# - git push

# And on another device
# - git pull
```

**I can do it!**

---

### Can create a pull request.

<!--
  Make branch
  Do some stuff on that branch
  commit and push your stuff to GitHub with a message
  make a pull request on GitHub
  go over any changes and possible merge conflicts
  code review with the team and lastly merge to main branch -->

**I can do it!**

---

### Understands different Git workflows such as GitHub Flow.

<!--
Make a branch out from Main, that you work on.
When the wokr is finished, you commmit and push to GitHub.
On GitHub you create a pull request, where merge conflicts may occur and make code reviewwith the team.
When thats finished, you merge to main and deploy to Azure via GitHub Actions.
-->

---

### Can solve a merge conflict.

<!--
Merge conflict occurs when there is a line in main that is different from the line you are trying to merge.

Git shows conflicts like this:
<<<<<HEAD -> start of own version
========= -> dividing line
>>>>>main -> the other versions ending

-->

```
// You solve it by deciding which version to keep - or maybe a combination.
// Delete the markers and the version you don't need.
// Save file, git add file and git commmit - and the conflict is solved
```

**I can do it!**

---

## 3. Hardware, software og operativsystemer

### Can list the main hardware components of a computer, their functions and the Von Neumann architecture.

<!--
CPU -> Central Processing Unit 
- Its the CPu that does all the work - the brain.
- It reads instruction one at a time and executes them quickly

RAM -> Random Access Memory
- Fast and temporary memory
- Gottra save all the files, cause when the computer turns off, its gone.

Storage -> HDD/SSD
- Permanent storage of files.
- Slower than RAM, but has a bigger capacity

Von Neuman -> Data and instructions in the same memory (RAM)
Descibes how computers are build - almost every computer today follows this structure.
In the early days, we reprogrammed by moving wires around. But the Neumann way, you could just load a new program into the memory - thereby came Software.
-->

**I can do it!**

---

### Can explain how computers work, starting from hardware all the way to software.

<!--
Layer 1: Transistors - the bottom of it all
- Small electric switch. it can either be on (1) or off (0)
- The whole computer is build with the whole concept of on and off - therefore binary.

Layer 2: logic gates - transistors working together
- logic ports does simple decisions
  - AND-gate -> output is 1, but only if both outputs are 1
  - OR-gate -> output is 1 if at least one output is 1
  - NOT-gate -> tunrs the outputs (0=1,1=0)

Layer 3: Machione code - CPU
- the CPU does a limited set of instructions - binary code
- the CPU loads, decodes and executes instructions

Layer 4: Assembly - machine code with readable names
- Machine code made readable to humans

Layer 5: high-level language - programming
- Java, Python, C++, JavaScript and so on
- All the different languages have different ways of translating to machine code

Layer 6: Operative system (OS) - The manager
- Windows, macOS, Linux
- It's a big program controlling the computer.
  - Administrate processes
  - Controls memeory
  - Handle files
  - Communicates with the hardware via drivers
  - Offers a user interface

  Layer 7: Applications
  - programs we interact with, such as IntelliJ, Chrome, Spotufy and so on
  - they don't communicate directly wiht the hardware.
  - The apps calls for the OS when a file is needed to be read og opening a network connection
-->

**I can do it!**

---

### Can talk about processes in operating systems.

<!--
A program is a passiv file on a disk, where a process is a runnign program in RAM
PID (Process ID) -> unique number the OS gives every proess, so it can keep a tab on them
Threads -> a process can have multiple threads going on at the same time and share memory.
Process states:
  - READY - ready to run, waiting on the CPU
  - RUNNING - using the CPU
  - WAITING - waiting on disk or netword or user-input
Scheduling -> the OS has a scheduler who decides which process that gets time from the CPU. It goes so fast, it looks like it runs simultanoulsy
Context switch -> when the CPU switches from one process to another
-->

---

## 4. Talrepræsentation og tegnsæt

### Can talk about different number representations: Binary, Hexadecimal, Decimal.

<!--
Binary code:
  - only 0 and 1
Hexadecimal:
  - 0-9 and A-F
Decimal:
  - 0-9
  - What we use in our every day life

Example - the numberer 255
  - Decimal - 255
  - Binary - 1111 1111
  - Hex - FF
-->

**I can do it!**

---

### Can bring up real-world use cases for different number representations.

<!--
Binary:
  - Bit-flags (Linux rwx)
  - low-level network protocol
  - Image format
Hex:
  - colours in CSS
  - MAC adresses
  - memeory adresses
Decimal:
  - amounts
  - price
  - everything we have to read directly
-->

**I can do it!**

---

### Can explain different charsets like ASCII and Unicode and how they differ.

<!--
ASCII:
  - Only have english letters, numbers and ordinary characters
  - cant handle æ,ø and å or other languages characters
  - 7 bits and 128 characters
Unicode:
  - internation standard that gives every character a uinique number (æ=U+00E6)
  - Covers all languages, emojis, math symbols and so on
UFT-8:
  - the most used encoding by Unicode
  - Variable length (1-4 bytes) and backward compatible with ASCII
  - English characters still only take up 1 byte, while æ takes up 2 bytes
  
Sometimes the database or file doesnt use UFT-8, so æ,ø and å is shown as a ? or a weird character
-->

**I can do it!**

---

## 5. Databaser – grundlæggende

### Knows about different types of databases and their use cases.

<!--
Relational (SQL)
  - structured tabels with realtions, ACID-garanties.
  - used for most businuess applications
NoSQL document (fx MongoDB)
  - Saves JSON-like documents.
  - Is used when the data doesnt have a fixed structure
Key-values (fx Redis)
  - very quick
  - saves simple pairs
  - used for caching and sessions
Graph (fx Neo4j)
  - Optimized for relationships between things
  - used for social networks and recommendation
-->

---

### Can setup a new MySQL database and connect to it.

```sql
-- MySQL
  -- CREATE DATABASE oenskeskyen;
  -- USE oenskeskyen;

-- Connection thorugh terminal
  -- mysql -u root -p

--JDBC in Spring Boot
  -- spring.datasource.url=jdbc:mysql://localhost:3306/oenskeskyen
  -- spring.datasource.username=root
  -- spring.datasource.password=password
```

**I can do it!**

---

### Can create DDL statements to create tables.

```sql
-- CREATE TABLE users (
    id INT PRIMARY KEY,
    username VARCHAR(50),
    email VARCHAR(100)
);
```

**I can do it!**

---

### Can create DML (`SELECT`, `INSERT`) statements.

```sql
-- INSERT INTO users (id, username, email)
VALUES (1, 'cassandra', 'cassandra@example.com');

SELECT * FROM users;
```

**I can do it!**

---

### Can use `WHERE` clause to filter results.

```sql
-- SELECT * FROM users WHERE username = 'cassandra';

SELECT * FROM wishes WHERE price < 500;
```

**I can do it!**

---

### Can define Primary Keys.

```sql
-- A primary key ensures that every row is unique and cant be NULL

-- CREATE TABLE users (
    id INT PRIMARY KEY,
    username VARCHAR(50)
);
```

**I can do it!**

---

### Understands how Foreign Keys work.

<!--
TODO:
A FK is a column which points to a PK in another tabel
Ensures referential integrity.
You cannot insert an FK value that does not exist in the other table.
-->

---

## 6. Databaser – viderekommende SQL

### In `SELECT` statements, can use (with moderate help):

#### `LIMIT`, `ORDER BY`, `GROUP BY`

```sql
-- LIMIT, ORDER BY, GROUP BY
-- sqlSELECT * FROM wishes
-- ORDER BY price DESC
-- LIMIT 10;

-- SELECT user_id, CO
```

#### Aggregate functions: `COUNT`, `SUM`, `AVG`, `MIN`, `MAX`

```sql
SELECT COUNT(*) FROM wishes;
SELECT AVG(price) FROM wishes;
SELECT MIN(price), MAX(price) FROM wishes;
```

#### Pattern matching med `LIKE` og wildcards

```sql
-- All uasers whose names starts with 'C'
SELECT * FROM users WHERE username LIKE 'C%';

-- All wishes that contatins 'bog'
SELECT * FROM wishes WHERE name LIKE '%bog%';

--  Macthes exactly with one character
SELECT * FROM users WHERE username LIKE 'C_ssandra';
```

#### `JOIN` to combine data from multiple tables

```sql
SELECT users.username, wishes.name
FROM users
JOIN wishes ON users.id = wishes.user_id;
```

**I can do it!**

---

### Can create inner, left and right joins after looking up the syntax.

```sql
-- INNER JOIN: only users with wishes
SELECT users.username, wishes.name
FROM users
INNER JOIN wishes ON users.id = wishes.user_id;

-- LEFT JOIN: all users, also those without wishes (NULL in wishes-columns)
SELECT users.username, wishes.name
FROM users
LEFT JOIN wishes ON users.id = wishes.user_id;

-- RIGHT JOIN: all wishes, alos those without a user
SELECT users.username, wishes.name
FROM users
RIGHT JOIN wishes ON users.id = wishes.user_id;
```

**I can do it!**

---

### Can create DDL statements to create tables with constraints: `PRIMARY KEY`, `AUTO_INCREMENT`, `FOREIGN KEY`, `UNIQUE`, `NOT NULL`.

```sql
-- CREATE TABLE users (
    id INT PRIMARY KEY AUTO_INCREMENT,
    username VARCHAR(50) UNIQUE NOT NULL,
    email VARCHAR(100) UNIQUE NOT NULL
);

CREATE TABLE wishes (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100) NOT NULL,
    price DECIMAL(10,2),
    user_id INT,
    FOREIGN KEY (user_id) REFERENCES users(id)
);
```

**I can do it!**

---

### Can create DML (`UPDATE`, `DELETE`) statements.

```sql
-- UPDATE users
SET email = 'new@example.com'
WHERE id = 1;

DELETE FROM wishes
WHERE id = 5;

-- Always remember WHERE or else all the rows will be opdated/deleted
```

**I can do it!**

---

## 7. YAML og GitHub Actions

### Can write YAML.

```yaml
# name: Cassandra
age: 24
hobbies:
  - pilates
  - kaniner
  - kodning
adresse:
  by: København
  postnummer: 2100
```

**I can do it!**

---

### Understands what GitHub Actions are and can break down workflows into runners, jobs, and steps.

<!--
GitHub Actions
  - CI/CD-platofrm build within GitHub
  - Automates tests, builds and deployments
Workflow
  - YAML-files placed in .github/workflows/ whioch defines what will happen
Trigger
  - what starts the workflow
  - could be on: puhs, on: pull_request or on: schedule
Job
  - a group of steps that runs on one runner
  - more jobs can run parallel
Runner
  - the machine that the workflow runs on
  - could be ubuntu-latest or windows-latest
Step
  - A single command opr action
  - Checkout code, run tests, deploy
-->

---

### Can give use cases for GitHub Actions.

<!--
 Run automatic test with every push or pull request
 Build and deploy to Azure by merge to main
 Format code automatic
 Send notification to email if theres a mistake
-->

**I can do it!**

---

## 8. Cloud og deployment

### Understands different cloud service models: IaaS, PaaS, SaaS.

<!--
IaaS (infrastructure as a Service)
  - virtuel machines, network, storage
  - running your own OS, runtime and app
PaaS (PLatform as a Service)
  - uploading your app
  - the provider controls OS and runtime
SaaS (Software as a Service)
  - A finished product you can use
-->

---

### Can deploy a web application to Azure App Service.

<!--
create an App Service in Azure (Java 17)
Configure runtime (Spring Boot)
Set app settings (database url, username, password as environment variables)
Conncet GitHub Actions via Deployment Center
The app will be available on https://<app-navn>.azurewebsites.net
-->

**I can do it!**

---

### Understands the flow from pushing, GitHub Actions running, building the project and deployment to Azure.

<!--
push code to main on GitHub
GitHub Actions is triggered by the push
Runner checks the code
Runner builds the project with mvn package
Output is a .jar-file
Aritfact uploads
Deploy-step sends the jar file to Azure via publish profile
Azure app restarts with the new version
-->

---

## 9. Database i Spring og Azure

### Adding a database to a Spring project.

<!--
Add dependencies in pom.xml

<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-jdbc</artifactId>
</dependency>
<dependency>
    <groupId>com.mysql</groupId>
    <artifactId>mysql-connector-j</artifactId>
</dependency>

onmfigure application.properties:

propertiesspring.datasource.url=jdbc:mysql://localhost:3306/oenskeskyen
spring.datasource.username=root
spring.datasource.password=password
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

Use JdbcTemplate in a repository-class to make queries.
-->

**I can do it!**

---

### Setting up a database in Azure.

<!--
Create an Azure databse for MySql
Configure firewall - allow Azure and own IP
Create database and user via Azure CLI or MySQL Workbench
Note: Azure typically requires a SSL-connection
-->

**I can do it!**

---

### Can set up a database in Azure and connect it to an Azure App Service project with a guide.

<!--
In App Service -> Configuration -> Application setting: add
  - Spring_DATASOURCE_URL
  - SPRING_DATASOURCE_USERNAME
  - SPRING_DATASOURCE_PASSWORD
Maybe add ?useSSL=true&requireSSL=true to the connection-string
Restart App Service and test connection
-->

**I can do it!**

---

## 10. Concurrency og transaktioner

### Is able to go through scenarios that can cause concurrency problems in databases.

<!--
Classic problems when multiple users/processes access the database simultaneously:
  - lost update -> two users updates the same row. One overwrites the other without knowing it
  - Dirty read -> User A reads data that user B have changed but haven't committed. if B rollws back, A has read data that technically never existed
  - Non-repeatable read -> SELECT gives different results within the same transaction because another transaction has changed data in the meantime.
  - Phantom read -> new rows shows up (or disappers) between two SELECTs in the same transaction
-->

---

### Can explain what ACID is and why it solves concurrency problems for databases.

<!--
TODO:
- A – Atomicity: All or nothing. A transaction is either fully committed or fully rolled back. No half-updates.
- C – Consistency: the database goes from one valid state to another. All constraints (FK, NOT NULL, etc.) are respected.
- I – Isolation: Transactions do not affect each other while they are running. This prevents dirty reads and non-repeatable reads.
- D – Durability: Once a transaction is committed, it is permanent — even if the server crashes.

How it solves concurrency:
Isolation prevents two users from seeing half of each other's work. Atomicity ensures that money doesn't "disappear" between two accounts if a transfer fails halfway through.
-->

---

### Is aware of the possibility to define transactions in SQL and JDBC.

```sql
-- START TRANSACTION;
UPDATE accounts SET balance = balance - 100 WHERE id = 1;
UPDATE accounts SET balance = balance + 100 WHERE id = 2;
COMMIT;
-- If anything goes worng: ROLLBACK;
```

```java
Connection conn = dataSource.getConnection();
try {
    conn.setAutoCommit(false);

    // Træk 100 fra konto 1
    PreparedStatement stmt1 = conn.prepareStatement(
        "UPDATE accounts SET balance = balance - 100 WHERE id = 1");
    stmt1.executeUpdate();

    // Tilføj 100 til konto 2
    PreparedStatement stmt2 = conn.prepareStatement(
        "UPDATE accounts SET balance = balance + 100 WHERE id = 2");
    stmt2.executeUpdate();

    conn.commit();
} catch (SQLException e) {
    conn.rollback();
}
```

**I can do it!**
