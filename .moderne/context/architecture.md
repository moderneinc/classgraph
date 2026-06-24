# Architecture

## FINOS CALM architecture diagram

FINOS CALM (Common Architecture Language Model) architecture diagram showing services, databases, external integrations, and messaging connections. Use this to understand the high-level system architecture and component relationships.

## Data Tables

### Project metadata

**File:** [`project-metadata.csv`](project-metadata.csv)

Project identification including artifact ID, group ID, and name.

| Column | Description |
|--------|-------------|
| Source path | The path to the build file (pom.xml or build.gradle). |
| Artifact ID | The project's artifact ID (Maven) or project name (Gradle). |
| Group ID | The project's group ID. |
| Name | The project's display name. |
| Description | The project's description. |
| Version | The project's version. |

### Database connections

**File:** [`database-connections.csv`](database-connections.csv)

Database connections and data access patterns in the application.

| Column | Description |
|--------|-------------|
| Entity ID | Unique identifier for this database entity (format: repository:{className} or entity:{className}). |
| Source path | The path to the source file containing the database access. |
| Entity/Table name | The name of the entity or table being accessed. |
| Entity class | The fully qualified name of the entity class (if applicable). |
| Repository class | The fully qualified name of the repository or DAO class (if applicable). |
| Connection type | The type of database connection (JPA, JDBC, Spring Data, MyBatis). |
| Database type | The type of database if detectable (PostgreSQL, MySQL, MongoDB, etc.). |

### Data assets

**File:** [`data-assets.csv`](data-assets.csv)

Data entities, DTOs, and records that represent the application's data model.

| Column | Description |
|--------|-------------|
| Source path | The path to the source file containing the data asset. |
| Class name | The fully qualified name of the data asset class. |
| Simple name | The simple class name for display. |
| Asset type | The type of data asset (Entity, Record, DTO, Document, etc.). |
| Description | A description of the data asset based on its fields. |
| Fields | Comma-separated list of field names. |

