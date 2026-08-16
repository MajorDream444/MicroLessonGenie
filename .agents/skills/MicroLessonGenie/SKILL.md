```markdown
# MicroLessonGenie Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches the key development patterns, coding conventions, and workflows used in the MicroLessonGenie TypeScript codebase. It covers file organization, import/export styles, commit message conventions, and the process for managing production readiness documentation. This guide will help you contribute code and documentation that aligns with the project's established standards.

## Coding Conventions

### File Naming
- Use **snake_case** for all file names.
  - Example: `micro_lesson_generator.ts`

### Import Style
- Use **relative imports** when referencing other modules.
  - Example:
    ```typescript
    import { generateLesson } from './lesson_utils';
    ```

### Export Style
- Use **named exports** for all exported functions, types, or constants.
  - Example:
    ```typescript
    export function generateLesson() { ... }
    ```

### Commit Messages
- Follow the **conventional commit** format.
- Use the `chore` prefix for maintenance or non-feature commits.
  - Example:
    ```
    chore: update production readiness documentation for agents
    ```

## Workflows

### Add Production Readiness Control
**Trigger:** When someone wants to introduce or update production readiness controls or documentation for agents, features, or the repository as a whole.  
**Command:** `/add-production-readiness`

1. Identify the documentation or template file relevant to production readiness:
    - `AGENTS.md`
    - `CLAUDE.md`
    - `.github/PRODUCTION_READINESS.md`
    - `.github/pull_request_template.md`
2. Edit or create the file to include new production readiness controls or guidelines.
3. Commit the changes with a message indicating a production readiness control update, following the conventional commit format.
    - Example:
      ```
      chore: add new checklist to PRODUCTION_READINESS.md
      ```

## Testing Patterns

- Test files use the pattern `*.test.*` (e.g., `lesson_generator.test.ts`).
- The specific testing framework is unknown; check existing test files for structure.
- Place tests alongside or near the modules they test.

## Commands

| Command                   | Purpose                                                         |
|---------------------------|-----------------------------------------------------------------|
| /add-production-readiness | Add or update production readiness documentation and templates.  |
```