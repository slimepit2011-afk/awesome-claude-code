# Python FastAPI Backend Rules (`CLAUDE.md`)

Instructions for Claude Code when building asynchronous backend services with FastAPI and Python.

---

```markdown
# FastAPI Engineering Guidelines

## Technology Stack
- Python 3.11+
- FastAPI with Pydantic v2 data modeling
- SQLAlchemy 2.0 (async engine) or Tortoise ORM
- Pytest with pytest-asyncio for automated test suites

## Code Quality Standards
- Use asynchronous route handlers (`async def`) for any I/O-bound database or external network operations.
- Enforce strict typing with Python type hints and Pydantic models for request and response serialization.
- Isolate domain logic in `services/` and database queries in `repositories/`.
- Handle expected errors using custom HTTP exceptions with descriptive JSON error bodies.

## Test & Execution Commands
- Launch dev server: `uvicorn app.main:app --reload`
- Execute test runner: `pytest`
- Code formatting and linting: `ruff check . && ruff format .`
```
