---
name: code-review-pro
description: >-
  Conducts high-standard code reviews focusing on Clean Code, SOLID principles,
  architectural clarity, performance, error resilience, and maintainability.
---

# Code Review Pro & Quality Assurance

Comprehensive framework for evaluating and refactoring code to ensure exceptional readability, reliability, and modularity.

## Quality Standards

### 1. Clean Code & Architecture
- **Single Responsibility Principle (SRP)**: Each function, module, or component must do exactly one thing well.
- **Meaningful Naming**: Use descriptive, intention-revealing names for variables, functions, and files (avoid abbreviations like `d`, `temp`, `fn1`).
- **DRY (Don't Repeat Yourself)**: Extract reusable helper functions, hooks, and UI components.

### 2. Error Handling & Resilience
- Always handle asynchronous operations with `try/catch` or `.catch()` blocks.
- Never swallow errors silently; provide informative error messages or fallback states.
- Return standardized JSON response formats in APIs (`{ success: boolean, data?: any, error?: string }`).

### 3. Performance & Resource Efficiency
- Optimize loops, avoid unnecessary re-renders in UI components.
- Use efficient data structures and database indexes.
- Paginate large data sets rather than dumping thousands of records at once.

### 4. Documentation & Verification
- Include concise JSDoc / Docstrings for public functions and API endpoints.
- Provide a clear, well-structured `README.md` for every project with setup instructions, prerequisites, features, and screenshots.
