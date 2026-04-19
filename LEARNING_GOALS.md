# Mandatory II – Learning Goals

Dette dokument gennemgår samtlige learning goals fra semesterplanen.

- For **"can"-punkter**: kort snippet/eksempel + "I can do it!"
- For **"understands"/"knows"-punkter**: et par sætninger eller nøgleord der viser jeg kan forklare det.

---

## 1. Terminal og filhåndtering

### Can navigate the terminal: `ls`, `cd`, `whoami`, `pwd`.

```bash
# TODO: indsæt dit eget eksempel
```

**I can do it!**

---

### Can create, delete files / folders: `mkdir`, `rm`, `cp`, `mv`, `touch`, `nano`.

```bash
# TODO
```

**I can do it!**

---

### Can use the following basic terminal commands: `cat`, `wc`, `uniq`, `sort`.

```bash
# TODO
```

**I can do it!**

---

## 2. Git og GitHub

### Can create a new repository in your preferred Git provider.

```bash
# TODO: hvordan du opretter et nyt repo (fx på GitHub + git init / remote add)
```

**I can do it!**

---

### Can perform basic Git operations: `clone`, `add`, `commit`, `push`, `pull`.

```bash
# TODO
```

**I can do it!**

---

### Can create a pull request.

<!-- TODO: Beskriv workflow – branch, push, åbn PR på GitHub, review, merge -->

**I can do it!**

---

### Understands different Git workflows such as GitHub Flow.

<!--
TODO: Forklar kort.
Nøgleord: main altid deployable, feature branches, pull request, review, merge, deploy.
Evt. sammenlign kort med Git Flow.
-->

---

### Can solve a merge conflict.

<!-- TODO: Vis eksempel på conflict markers (<<<<<<<, =======, >>>>>>>) og hvordan du løser den -->

```
// TODO: eksempel på conflict markers
```

**I can do it!**

---

## 3. Hardware, software og operativsystemer

### Can list the main hardware components of a computer, their functions and the Von Neumann architecture.

<!--
TODO:
- Komponenter: CPU, RAM, storage, bus, I/O
- Von Neumann: data og instruktioner i samme hukommelse
- Fetch-decode-execute cyklus
-->

**I can do it!**

---

### Can explain how computers work, starting from hardware all the way to software.

<!--
TODO: Lagene – transistorer → logic gates → maskinkode → assembly → højniveau-sprog → OS → applikationer
-->

**I can do it!**

---

### Can talk about processes in operating systems.

<!--
TODO: Nøgleord – proces vs. program, PID, tråde, scheduling, process states (ready/running/waiting), context switch
-->

---

## 4. Talrepræsentation og tegnsæt

### Can talk about different number representations: Binary, Hexadecimal, Decimal.

<!--
TODO:
- Binær: base 2, bruges internt i computere
- Hex: base 16, kompakt repræsentation af binær
- Decimal: base 10, menneske-venlig
- Omregningseksempler
-->

**I can do it!**

---

### Can bring up real-world use cases for different number representations.

<!--
TODO: Eksempler
- Binær: bit-flag, low-level protokoller
- Hex: farver (#FF5733), memory addresses, MAC-adresser
- Decimal: brugervendt UI, beløb
-->

**I can do it!**

---

### Can explain different charsets like ASCII and Unicode and how they differ.

<!--
TODO:
- ASCII: 7-bit, 128 tegn, engelsk alfabet
- Unicode: standard for ALLE sprog, tildeler code points (U+XXXX)
- UTF-8: encoding af Unicode, variabel længde (1-4 bytes), bagudkompatibel med ASCII
- Hvorfor vigtigt: æøå kræver Unicode
-->

**I can do it!**

---

## 5. Databaser – grundlæggende

### Knows about different types of databases and their use cases.

<!--
TODO:
- Relationelle (SQL): MySQL, PostgreSQL – strukturerede data, ACID, relationer
- NoSQL document: MongoDB – fleksibelt skema, JSON-lignende
- Key-value: Redis – caching, sessions
- Graph: Neo4j – relationer (fx sociale netværk)
-->

---

### Can setup a new MySQL database and connect to it.

```sql
-- TODO: CREATE DATABASE + forbindelse (via terminal, Workbench eller JDBC)
```

**I can do it!**

---

### Can create DDL statements to create tables.

```sql
-- TODO: eksempel på CREATE TABLE
```

**I can do it!**

---

### Can create DML (`SELECT`, `INSERT`) statements.

```sql
-- TODO: eksempel på SELECT og INSERT
```

**I can do it!**

---

### Can use `WHERE` clause to filter results.

```sql
-- TODO
```

**I can do it!**

---

### Can define Primary Keys.

```sql
-- TODO: CREATE TABLE med PRIMARY KEY
```

**I can do it!**

---

### Understands how Foreign Keys work.

<!--
TODO:
- FK peger på en PK i en anden tabel
- Sikrer referentiel integritet
- Kan ikke indsætte række med FK der ikke findes i moder-tabellen
- ON DELETE CASCADE / SET NULL
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
