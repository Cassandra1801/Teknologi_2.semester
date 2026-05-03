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
-- TODO
```

#### Aggregate functions: `COUNT`, `SUM`, `AVG`, `MIN`, `MAX`

```sql
-- TODO
```

#### Pattern matching med `LIKE` og wildcards

```sql
-- TODO: eksempel med % og _
```

#### `JOIN` to combine data from multiple tables

```sql
-- TODO
```

**I can do it!**

---

### Can create inner, left and right joins after looking up the syntax.

```sql
-- TODO: INNER JOIN
-- TODO: LEFT JOIN
-- TODO: RIGHT JOIN
```

**I can do it!**

---

### Can create DDL statements to create tables with constraints: `PRIMARY KEY`, `AUTO_INCREMENT`, `FOREIGN KEY`, `UNIQUE`, `NOT NULL`.

```sql
-- TODO: CREATE TABLE der bruger alle constraints
```

**I can do it!**

---

### Can create DML (`UPDATE`, `DELETE`) statements.

```sql
-- TODO
```

**I can do it!**

---

## 7. YAML og GitHub Actions

### Can write YAML.

```yaml
# TODO: lille YAML-eksempel (fx key-value, liste, nested)
```

**I can do it!**

---

### Understands what GitHub Actions are and can break down workflows into runners, jobs, and steps.

<!--
TODO:
- GitHub Actions = CI/CD platform indbygget i GitHub
- Workflow: YAML-fil i .github/workflows/
- Runner: maskinen workflow kører på (ubuntu-latest, windows-latest…)
- Job: gruppe af steps, kører på én runner
- Step: enkelt kommando eller action
- Triggers: on push, pull_request, schedule…
-->

---

### Can give use cases for GitHub Actions.

<!--
TODO: Eksempler
- Kør tests automatisk ved push
- Byg og deploy til Azure ved merge til main
- Lint / formater kode
- Publish package / Docker image
-->

**I can do it!**

---

## 8. Cloud og deployment

### Understands different cloud service models: IaaS, PaaS, SaaS.

<!--
TODO:
- IaaS (Infrastructure): virtuelle maskiner, netværk, lagerplads (fx Azure VM, AWS EC2) – du styrer OS og opefter
- PaaS (Platform): kør din app uden at tænke på OS/server (fx Azure App Service, Heroku)
- SaaS (Software): færdigt produkt brugeren bruger direkte (fx Gmail, Office 365)
- Tegn evt. "pizza as a service"-analogien
-->

---

### Can deploy a web application to Azure App Service.

<!--
TODO: Beskriv dine trin fra Ønskeskyen-deployment:
- Opret App Service i Azure Portal
- Konfigurer runtime (Java 17 / Spring Boot)
- Connect via GitHub Actions eller deployment center
- Sæt environment variables
-->

**I can do it!**

---

### Understands the flow from pushing, GitHub Actions running, building the project and deployment to Azure.

<!--
TODO:
- git push → GitHub
- Workflow triggeres
- Runner tjekker koden ud, bygger (mvn package)
- Artifact uploades
- Deploy-step sender .jar til Azure App Service via publish profile / service principal
- Azure genstarter app
-->

---

## 9. Database i Spring og Azure

### Adding a database to a Spring project.

<!--
TODO:
- Tilføj dependency: spring-boot-starter-jdbc (eller data-jpa) + mysql-connector-j
- Konfigurer application.properties (url, username, password)
- Opret JdbcTemplate / Repository
-->

```properties
# TODO: application.properties eksempel
```

**I can do it!**

---

### Setting up a database in Azure.

<!--
TODO:
- Opret Azure Database for MySQL
- Konfigurer firewall (tillad Azure services + egen IP)
- Opret database og bruger
- Note SSL-krav
-->

**I can do it!**

---

### Can set up a database in Azure and connect it to an Azure App Service project with a guide.

<!--
TODO:
- Connection string i App Service "Configuration" (eller application.properties)
- SSL-certifikat ved behov
- Test forbindelse
-->

**I can do it!**

---

## 10. Concurrency og transaktioner

### Is able to go through scenarios that can cause concurrency problems in databases.

<!--
TODO: Klassiske problemer
- Lost update: to brugere opdaterer samme række, den ene overskriver den anden
- Dirty read: læser ikke-committet data
- Non-repeatable read: samme SELECT giver forskellige resultater i samme transaktion
- Phantom read: nye rækker dukker op mellem to SELECTs
-->

---

### Can explain what ACID is and why it solves concurrency problems for databases.

<!--
TODO:
- A – Atomicity: alt eller intet
- C – Consistency: databasen går fra én gyldig tilstand til en anden
- I – Isolation: transaktioner påvirker ikke hinanden
- D – Durability: committed data er permanent (overlever crash)
- Hvordan løser det: isolation hindrer dirty/non-repeatable reads, atomicity hindrer halve updates osv.
-->

---

### Is aware of the possibility to define transactions in SQL and JDBC.

<!--
TODO: Nøgleord
- SQL: START TRANSACTION / BEGIN, COMMIT, ROLLBACK
- JDBC: connection.setAutoCommit(false), connection.commit(), connection.rollback()
- Spring: @Transactional
- Atomic structures: updates enten sker fuldt ud eller slet ikke
-->

```sql
-- TODO: SQL transaktion-eksempel
```

```java
// TODO: JDBC transaktion-eksempel
```

**I can do it!**

---

## Kilder

<!-- TODO: Evt. referencer til slides, docs, tutorials -->
