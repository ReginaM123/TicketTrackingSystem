
 Ticket Tracking System

 Overview

This project is a Ticket Tracking System built with ASP.NET Core MVC (Phase I) and expanded with additional functionalities in Phase II. The system allows different types of users (QA, RD, PM, Administrator) to manage and track various tickets, including bugs, feature requests, and test cases.

### Features
 Phase I Features:
- **User Roles**:
  - **QA (Quality Assurance)**:
    - Create, edit, and delete bug tickets.
  - **RD (Research and Development)**:
    - Resolve bug tickets.
- **Bug Management**:
  - **Bug Creation**: QA can create a bug ticket with required fields: Summary and Description.
  - **Bug Editing**: QA can edit an existing bug ticket.
  - **Bug Deletion**: QA can delete an existing bug ticket.
  - **Bug Resolution**: RD can mark a bug ticket as resolved.

#### Phase II Features:
- **Enhanced Ticket Attributes**:
  - Added Severity and Priority fields to bug tickets.
- **Additional Ticket Types**:
  - **Feature Request**:
    - Created by PM (Project Manager).
    - Resolved by RD.
  - **Test Case**:
    - Created and resolved by QA.
    - Read-only for other user types.
- **User Management**:
  - **Administrator**:
    - Manage (add, edit, delete) users including QA, RD, and PM.
    - 

1. Clone the repository
   ```sh
   git clone https://github.com/yourusername/ticket-tracking-system.git
   cd ticket-tracking-system
   ```

2. Setup the database
   - Update the connection string in `appsettings.json` to point to your SQL Server instance.
   - Run migrations to create the database schema:
     ```sh
     dotnet ef migrations add InitialCreate
     dotnet ef database update
     ```

3. Run the application
   ```sh
   dotnet run
   ```

4. Access the application
   - Open your browser and navigate to `http://localhost:5000`.

### Technologies Used

- **Backend**: ASP.NET Core MVC
- **Frontend**: HTML, CSS, JavaScript (you can mention any specific framework if used)
- **Database**: Entity Framework Core with SQL Server

### Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes. Ensure that your code adheres to the project's coding standards and includes appropriate tests.

### License
