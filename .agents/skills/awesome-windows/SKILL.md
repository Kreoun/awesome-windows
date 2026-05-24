```markdown
# awesome-windows Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches you how to contribute to the `awesome-windows` repository, a curated list of awesome applications, tools, and software for Windows. You'll learn the project's coding conventions, how to add or update entries, manage pull requests, and update contributors, all while following established workflows and best practices.

## Coding Conventions

### File Naming
- Use **PascalCase** for file names.
  - Example: `SoftwareEntry.ts`, `ReadmeParser.ts`

### Import Style
- Use **relative imports** for modules within the project.
  - Example:
    ```typescript
    import { parseReadme } from './ReadmeParser';
    ```

### Export Style
- Use **named exports** for all modules.
  - Example:
    ```typescript
    export function addSoftwareEntry(entry: SoftwareEntry) { ... }
    ```

### Commit Messages
- Common prefixes: `docs`, `feat`, `fix`
- Messages are concise (~39 characters on average).
  - Example: `feat: add new backup tool to utilities`

## Workflows

### Add New Software Entry
**Trigger:** When you want to add a new application, tool, or software to the awesome-windows list.  
**Command:** `/add-software-entry`

1. Open `README.md`.
2. Add the new software entry under the relevant category.
   - Example:
     ```markdown
     - [SuperApp](https://superapp.example.com) - Powerful productivity tool.
     ```
3. Commit your change with a message like:  
   `feat: add SuperApp to productivity`
4. Optionally, submit a pull request if you don't have direct commit access.

---

### Fix or Update Existing Entry
**Trigger:** When you need to correct, clarify, or update an existing entry in the list.  
**Command:** `/fix-entry`

1. Open `README.md`.
2. Locate the entry to fix or update.
3. Make the necessary changes (e.g., fix formatting, update description, correct link).
4. Commit your change with a message like:  
   `fix: update description for SuperApp`
5. Optionally, submit a pull request if you don't have direct commit access.

---

### Merge Pull Request for README Change
**Trigger:** When a contributor submits a pull request to update the `README.md` file.  
**Command:** `/merge-readme-pr`

1. Review the pull request for correctness and formatting.
2. If everything looks good, merge the pull request into the main branch.

---

### Update Contributors List
**Trigger:** When you want to acknowledge new contributors in the README.  
**Command:** `/update-contributors`

1. Open `README.md`.
2. Update the contributors section to reflect recent contributions.
   - Example:
     ```markdown
     ## Contributors
     - @alice
     - @bob
     ```
3. Commit your change with a message like:  
   `docs: update contributors list`

## Testing Patterns

- **Testing framework:** Unknown (not detected).
- **Test file pattern:** Files named with `*.test.*`
  - Example: `SoftwareEntry.test.ts`
- To write a test, create a file following the pattern and include relevant test cases for your module.

## Commands

| Command               | Purpose                                                      |
|-----------------------|--------------------------------------------------------------|
| /add-software-entry   | Add a new software/tool entry to the list                    |
| /fix-entry            | Fix or update an existing software entry                     |
| /merge-readme-pr      | Merge a pull request that modifies the README.md             |
| /update-contributors  | Update the contributors section in README.md                 |
```