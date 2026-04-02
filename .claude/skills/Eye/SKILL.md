```markdown
# Eye Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill provides guidance on the development patterns, coding conventions, and common workflows used in the Eye repository. The project is primarily written in Python, with no major framework detected, and focuses on backend services and APIs. It also includes documentation and static asset management. This guide will help you contribute code, update language support, and maintain documentation in a consistent and effective manner.

## Coding Conventions

### File Naming
- Use **snake_case** for all Python files.
  - Example: `language_service.py`, `api_handler.py`

### Import Style
- Use **relative imports** within the package.
  - Example:
    ```python
    from .models import User
    from ..utils import parse_request
    ```

### Export Style
- Use **named exports** (explicitly listing what is exported).
  - Example:
    ```python
    __all__ = ['UserService', 'LanguageSupport']
    ```

### Commit Messages
- No strict prefix; freeform style.
- Average commit message length: ~25 characters.
  - Example: `Add English language support`

## Workflows

### Language Support Update
**Trigger:** When you want to add or improve language support (e.g., translating prompts, responses, or documentation).  
**Command:** `/add-language-support`

1. Modify backend service files to update language-specific logic or prompts.
    - Edit files in `backend/app/services/*.py`.
    - Example:
      ```python
      # backend/app/services/language_service.py
      def get_greeting(language):
          if language == "en":
              return "Hello!"
          elif language == "es":
              return "¡Hola!"
      ```
2. Update backend API files to support the new or improved language.
    - Edit files in `backend/app/api/*.py`.
    - Example:
      ```python
      # backend/app/api/greet.py
      from ..services.language_service import get_greeting

      def greet_user(request):
          lang = request.get('lang', 'en')
          return get_greeting(lang)
      ```
3. Optionally, update frontend components if user-facing language changes are needed.
    - Edit files in `frontend/src/components/*.vue`.

### Documentation and Assets Refactor
**Trigger:** When you want to update documentation or refresh static images (e.g., logos, screenshots) for the project.  
**Command:** `/update-docs-assets`

1. Update README files and documentation.
    - Edit `README.md` or `README-EN.md` as needed.
    - Example:
      ```markdown
      ## New Feature: Multi-language Support
      Eye now supports English and Spanish prompts.
      ```
2. Add or replace static image assets in the `static/image` directory.
    - Place new images in `static/image/`.
    - Remove or rename outdated images as necessary.

## Testing Patterns

- **Testing Framework:** Unknown (not detected).
- **Test File Pattern:** Files matching `*.test.*` are used for tests.
  - Example: `language_service.test.py`
- **Best Practice:** Place tests alongside the code they test, using the `.test.` naming convention.

## Commands

| Command                | Purpose                                                      |
|------------------------|--------------------------------------------------------------|
| /add-language-support  | Initiate a workflow to add or update language support        |
| /update-docs-assets    | Start a documentation and static asset update workflow       |
```
