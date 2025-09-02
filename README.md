# Library App

## Description

Library App is a modular C# solution designed to manage library operations such as book loans, patron management, and infrastructure services. The project follows clean architecture principles, separating core logic, infrastructure, and presentation layers for maintainability and scalability.

## Project Structure

- `AccelerateDevGHCopilot/`
  - `README.md`
  - `src/`
    - `Library.ApplicationCore/`
      - `Library.ApplicationCore.csproj`
      - `Entities/`
      - `Enums/`
      - `...`
    - `Library.Console/`
      - `Library.Console.csproj`
      - `...`
    - `Library.Infrastructure/`
      - `Library.Infrastructure.csproj`
      - `...`
  - `tests/`
    - `UnitTests/`
      - `UnitTests.csproj`
      - `...`

## Key Classes and Interfaces

- **Entities (Library.ApplicationCore/Entities/)**
  - Core domain models such as Book, Patron, Loan, etc.
- **Enums (Library.ApplicationCore/Enums/)**
  - Enumerations for domain concepts (e.g., LoanStatus, BookGenre).
- **Infrastructure Services (Library.Infrastructure/)**
  - Implementations for data access, configuration, and external integrations.
- **Console Application (Library.Console/)**
  - Entry point for running the application and interacting via CLI.

## Usage

1. **Build the Solution**
   - Open a terminal in the repository root and run:
     ```
     dotnet build [library_project.sln](http://_vscodecontentref_/0)
     ```
2. **Run the Console Application**
   - Navigate to the `Library.Console` project directory and run:
     ```
     dotnet run --project src/Library.Console/Library.Console.csproj
     ```
3. **Run Unit Tests**
   - Navigate to the `UnitTests` project directory and run:
     ```
     dotnet test src/UnitTests/UnitTests.csproj
     ```

## License

This project is licensed under the MIT License. See the [LICENSE](getting-started-with-github-copilot/LICENSE) file
