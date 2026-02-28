```markdown
# AGENTS.md - Guidelines for AI Coding Agents

These guidelines are designed to ensure the creation and maintenance of high-quality, maintainable, and effective AI coding agents.  Adherence to these principles is crucial for successful development and long-term stability.

## 1. DRY (Don't Repeat Yourself)

*   **Code Reuse:**  Strive to create reusable components and functions across multiple agents. Avoid duplicating logic and data structures.
*   **Modular Design:** Each agent should have a clearly defined module with a single, specific responsibility.
*   **Parameterization:**  Parameters should be defined once and reused throughout the agent's logic, reducing redundancy.

## 2. KISS (Keep It Simple, Stupid)

*   **Minimal Code:**  Each function and module should accomplish a single, well-defined task.
*   **Avoid Complexity:**  Keep algorithms and data structures as simple as possible.  Favor readability over cleverness.
*   **Clear Naming:** Use descriptive names for functions, variables, and modules.

## 3. SOLID Principles

*   **Single Responsibility Principle:**  Each class/module should have one, and only one, reason to change.
*   **Open/Closed Principle:**  The system should be extensible without modifying the existing code.  Add new features without altering core logic.
*   **Liskov Substitution Principle:**  Subclasses should be substitutable for their base classes without altering the correctness of the program.
*   **Interface Segregation Principle:**  Clients should not be forced to implement interfaces they do not use.
*   **Dependency Inversion Principle:**  High-level modules should be dependent on low-level modules, not vice versa.

## 4. YAGNI (You Aren't Gonna Need It)

*   **Avoid Unnecessary Code:**  Do not implement functionality that is not currently required. Focus on what *is* needed.
*   **Refactor Only When Necessary:**  Refactoring should be a last resort after thorough testing.  Don't introduce new functionality just to improve existing code.

## 5. Development Workflow & Best Practices

*   **Unit Tests:** All code must be thoroughly tested with unit tests covering all functionality.  Each function/module should have at least 80% test coverage.
*   **Code Reviews:**  All changes must be reviewed by at least two developers before being merged.
*   **Static Analysis:**  Utilize static analysis tools (e.g., linters, code quality checkers) to identify potential issues early.
*   **Documentation:**  Clear and concise documentation is required for all functions, classes, and modules.
*   **Versioning:**  Use a version control system (e.g., Git) with clear commit messages.
*   **Configuration:**  Use configuration files to manage settings and parameters, avoiding hardcoded values.

## 6. File Size Limit (180 lines)

*   Each file must be no more than 180 lines of code.  All code must be clearly delineated with consistent indentation.

## 7.  Testing Requirements

*   **Comprehensive Test Suite:**  All modules must have dedicated test cases covering various scenarios.
*   **Test Driven Development (TDD):**  Implement tests before code.
*   **Regression Tests:**  Ensure that changes do not break existing functionality.
*   **Edge Case Testing:**  Specifically test boundary conditions and unusual inputs.

## 8.  Specific Considerations for AI Agents

*   **State Management:** Clearly define the agent's state and how it is updated.
*   **Decision Logic:**  Document the decision-making process clearly.
*   **Error Handling:**  Implement robust error handling to prevent unexpected behavior.
*   **Logging:**  Include logging statements to track agent actions and errors.

## 9.  Data Handling (Mocking Emphasis)

*   **Only Mocking for Tests:**  All data, algorithms, and state updates must be mocked or simulated for testing.  No real data should be used in production.
*   **Testable Data:** Ensure data inputs for unit tests are testable and predictable.
*   **Data Validation:** Implement data validation mechanisms to ensure data quality.


These guidelines are subject to change as the project evolves.  Any modifications must be communicated to the team.
```