# Smart Job Application Tracker

A Python-based job application management project designed to help organize job applications, manage user profiles, and track skills in one place.

Built as a hands-on backend development project to strengthen my understanding of Python, SQLite, data validation, and layered application architecture.

## Project Overview

Searching for jobs can involve tracking multiple applications, keeping profile information organized, and managing skills relevant to different opportunities. This project explores a structured way to manage that information through a command-line application.

**Project type:** Command-Line Application (CLI)  
**Status:** In Development  
**Technologies:** Python, SQLite, SQL, Git
## Features

### Job Application Management
- Add and manage job application records.
- Track application statuses.
- Search, filter, and sort application records.

### User Profile Management
- Create, view, update, and delete user profiles.
- Associate skills with specific user profiles.
- View the skills associated with a selected profile.

### Data Integrity
- Validate user inputs.
- Prevent duplicate skills within the same profile.
- Use SQLite foreign key relationships and cascading deletion to maintain data consistency.

## Technical Highlights

- **Python:** Application logic and business rules.
- **SQLite:** Persistent data storage and relational data management.
- **Layered architecture:** Separation of application entry point, services, repositories, and database operations.
- **Testing:** Automated tests for input validation.
## Architecture

The application follows a layered architecture to separate user interaction, business logic, and data access.

```text
User
  |
  v
CLI (main.py)
  |
  v
Service Layer
  |
  v
Repository Layer
  |
  v
SQLite Database
```

### Data Flow

1. The user interacts with the application through the command-line interface.
2. The service layer handles application logic.
3. The repository layer performs database operations.
4. SQLite stores application data and maintains relational integrity.

*Note: The web application version is planned for a future milestone.*
