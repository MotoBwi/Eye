```markdown
# Eye Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill introduces the core development patterns and workflows used in the Eye Python codebase. It covers coding conventions, file organization, import/export styles, and documents the main workflow for maintaining project documentation. This guide is useful for contributors aiming for consistency and efficiency in Eye's development process.

## Coding Conventions

### File Naming
- Use **snake_case** for all Python file names.
  - Example: `image_processor.py`, `data_loader.py`

### Import Style
- Use **relative imports** within the package.
  - Example:
    ```python
    from .utils import helper_function
    ```

### Export Style
- Use **named exports** (explicitly listing what is exported from a module).
  - Example:
    ```python
    __all__ = ['process_image', 'ImageAnalyzer']
    ```

### Commit Patterns
- Commit messages are freeform, typically short (~20 characters).
  - Example: `fix image loader bug`

## Workflows

### Update README Documentation
**Trigger:** When you need to add, update, or clean up the project documentation in `README.md`.  
**Command:** `/update-readme`

1. Open the `README.md` file in your editor.
2. Edit the content as needed (add, update, or remove sections, badges, links, etc.).
3. Save your changes.
4. Commit the changes with a descriptive message.
   - Example: `update usage section in README`
5. Push your changes to the repository or open a pull request.

## Testing Patterns

- **Framework:** Not explicitly defined; testing framework is unknown.
- **Test File Naming:** Test files follow the pattern `*.test.*`.
  - Example: `image_processor.test.py`
- **Writing Tests:** Place test cases in files matching the above pattern to ensure discoverability.

## Commands

| Command         | Purpose                                             |
|-----------------|-----------------------------------------------------|
| /update-readme  | Update or clean up project documentation in README. |

```