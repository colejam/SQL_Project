## NFL Scouting Database Design

### Purpose
The purpose of this database design is to implement a secure database environment for an NFL Scouting application. This database allows scouts to evaluate prospects for the upcoming NFL draft by gathering and organizing detailed information about each potential player.

### Description
The database stores comprehensive data on potential prospects, including player information, testing results, measurables, offensive stats, and defensive stats. It is designed to facilitate easy access and evaluation by scouts and coaches, ensuring a seamless recruitment process.

### Structure
- **Entities**:
  - **Strong Entity**: `PlayersInfo`
    - Attributes: player details (e.g., name, position, college)
  - **Weak Entities**:
    - `Measurable`
    - `PlayerTesting`
    - `OffensiveStats`
    - `DefensiveStats`
    - Each weak entity depends on the `PlayersInfo` entity and includes a foreign key to establish the relationship.

### Relations
The relational database schema consists of five relations:
1. `PlayersInfo` (Primary entity with a primary key)
2. `PlayerTesting`
3. `Measurable`
4. `OffensiveStats`
5. `DefensiveStats`

Each weak entity relation includes a foreign key referencing the `PlayersInfo` primary key, maintaining referential integrity.

### Integrity
- **Entity Integrity**: Ensured by primary keys in `PlayersInfo`.
- **Referential Integrity**: Maintained through foreign keys in `PlayerTesting`, `Measurable`, `OffensiveStats`, and `DefensiveStats`.

### Benefits
This database structure provides a robust and secure environment for scouts and coaches to access and evaluate player information efficiently, enhancing the recruitment process for NFL prospects.

### Example Records
The database includes example records to demonstrate its functionality and the relationships between entities.
