# AddressBookJDBC
An address book application that enables you to browse existing entries, add new entries and search for entries with a specific last name.

# Description
The AddressBook Java DB database contains an Addresses table with columns `AddressID`, `FirstName`, `LastName`, `Email` and `PhoneNumber`.

Class `Person` represents one person in the address book. Class `PersonQueries` manages the address book application's db connection and creates `PreparedStatements` to interact with the database. `AddressBookController` uses a `PersonQueries` object to interact with the database. `AddressBook` loads and displays the AddressBook's GUI.

The java program communicates with the Java DB and manages their data using JDBC which uses a low-level vendor driver to talk to the database.

# Getting Started
## Prerequisites
- JDK 1.8
- Java DB - Apache Derby
- JDBC

## Installing
- Create a local respository.
```
git clone git@github.com:lnpeng/AddressBookJDBC.git
cd AddressBookJDBC
```

- Setting up the Database
  - Open the NetBeans IDE.
  - On the **Services** tab, expand the **Databases** node then right click **Java DB**. Select **Start** server to launch the Java DB server.
  
- Creating the Database
  - On the **Services** tab, expand the **Databases** node, right click **Java DB** and select **Create Database...**.
  - Specify **Database Name**, **User Name**, **Password**.
  - Click **OK** to create the database.
  
- Populating the Database with sample data.
  - Expand the jdbc:derby://localhost:1527/addressperson node.
  - Right click the **Tables** node and select **Execute Command...** to open a **SQL** editor tab in NetBeans. Add the SQL statements. Right click in the **SQL Command** editor and select **Run File**.
  
## Running the tests
### Test the address book application
- Launch the application
- Browse all entries
- ![Screenshot](https://github.com/lnpeng/AddressBookJDBC/blob/master/Screen%20Shot%202018-12-01%20at%2010.05.31%20AM.png)

# Build
- [Ant](https://ant.apache.org/) - Automating software build process.
