# System Requirements Specification (SRS)

**Project:** EliteAthlete Academy Management System (EAAMS)  
**Company:** NovaSport Tech Sdn. Bhd.  
**Course:** BTS4493 Software Engineering, 2025/26 SEM II  
**Members:** TG23091 Steewart Aaron A/L Silvester | TG23088 Bavindran A/L Muthuraju  

---

## Functional Requirements (FR)

| No. | Category | Description |
|-----|----------|-------------|
| FR01 | Account Management | The system shall allow Administrators to create, update, and delete user accounts (Coaches and Players) and assign appropriate role-based permissions. |
| FR02 | Account Management | The system shall require all users to authenticate using a secure login (username and password) before accessing their respective dashboards. |
| FR03 | Performance Management | The system shall allow Coaches to input, edit, and delete daily numerical performance metrics (e.g., speed, agility, stamina) and qualitative feedback for their assigned players. |
| FR04 | Performance Management | The system shall allow Coaches to set specific, measurable training goals for individual players and track their progress over time. |
| FR05 | Performance Management | The system shall automatically process historical data to generate visual performance growth charts for individual players over a selected date range. |
| FR06 | Performance Management | The system shall allow Players to view their personal performance dashboards, including metrics, charts, and coach feedback. |
| FR07 | Tournament Management | The system shall allow Administrators to create new tournament events, detailing the event name, date, location, and maximum participant limits. |
| FR08 | Tournament Management | The system shall allow Coaches to view upcoming tournaments and register their assigned players into specific tournament rosters. |
| FR09 | Tournament Management | The system shall allow Administrators to generate tournament brackets and manually input match results as the tournament progresses. |
| FR10 | Tournament Management | The system shall send automated system notifications or emails to Players when they are successfully registered for a tournament or when a match time changes. |

---

## Non-Functional Requirements (NFR)

| No. | Category | Description |
|-----|----------|-------------|
| NFR01 | Security | The system shall implement strict Role-Based Access Control (RBAC). Players must be strictly restricted from viewing the performance records of other players or altering their own data. |
| NFR02 | Usability | The user interface shall be fully mobile-responsive, ensuring that Coaches can easily navigate and input data using tablets or smartphones directly from the training field. |
| NFR03 | Reliability | The system shall ensure data integrity by performing automated daily database backups of all performance logs and tournament records to an off-site server to prevent data loss. |
| NFR04 | Performance | The system shall process queries and load the interactive player performance dashboard (including charts) in under 3 seconds under standard internet conditions. |
| NFR05 | Scalability | The system database and application architecture shall be designed to handle at least 1,000 concurrent active users without experiencing noticeable performance degradation, especially during peak tournament registration periods. |

---

## Actors & Roles

| Actor | Access Level |
|-------|-------------|
| Administrator | Full system access – manage users, tournaments, and view all data |
| Coach | Can log/edit performance records and register players for tournaments |
| Player | Read-only access to their own performance dashboard only |
