# RoomExample - Room Example App
- This app shows the use of Room - Jetpack Component
- Why need Room
  - Abstraction over SQLite
  - Less Boilerplate
  - Compile Time Verification of SQL Queries
- The Room Database topics cover in this app 
  - Entities (Tables)
  - DAO (Data Access Object) Singleton
  - Type Convertors
  - Migrations
- Room Database - DAO
  - Data Access Objects
  - Interface containing methods to access database - CRUD Operations
  - We can define multiple DAOs
- SQLite Only Supports - We use type convertors if we use another type instead of belows:
  1. NULL
  2. INTEGER
  3. REAL
  4. TEXT
  5. BLOB
- synchronized lock is used to safe from multi threading
- Volatile annotation is used for immediately made visible to other threads that this is initialized.

## APP Structure
- Contact - Table Data Model Class
- ContactDao - Database Access Object Interface which have interface for CRUD Operations
- ContactDatabase - Use Singleton Pattern to initialize Database object
- Convertors - is used to convert types
- MainActivity - is activity where database create request and insert data and get all data by clicking hello world textview.
