### 💻 Data Engineering Skills Demonstrated
<hr>

#### Data Transformation
- String Parsing: Converting Python list format ['skill1', 'skill2'] to normalized rows via UNNEST and string functions
- Type Casting: DuckDB data types (VARCHAR, INTEGER, DOUBLE, etc.) for schema integrity
- Deduplication: Extracting unique companies and skills with proper surrogate key generation

#### Dimensional Modeling
- Star Schema Design: Fact table with dimension and bridge tables
- Surrogate Keys: ROW_NUMBER() for generating sequential IDs
- Bridge Table: Many-to-many relationship handling for job–skill mappings
- Referential Integrity: Foreign key constraints between fact, dimensions, and bridge

#### SQL Techniques
- DDL: CREATE TABLE, DROP TABLE IF EXISTS for idempotent schema creation
- DML: INSERT INTO ... SELECT with explicit column mapping
- CTEs: Common Table Expressions for complex transformations
- Window Functions: ROW_NUMBER() for surrogate key generation
- UNNEST: Flattening array-like skill data into relational rows

#### Production Practices
- Idempotency: Scripts safely rerunnable without side effects
- Verification: 06_verify_schema.sql for record count validation
- Orchestration: Master script for automated end-to-end execution
- Error Handling: Shell script with structured execution flow