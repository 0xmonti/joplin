# MONTIAI Guidelines

## Quick Reference

- Tabs for indentation (4 spaces in Python, follow PEP 8)
- Single quotes for strings
- Proper type hints (use `typing` module, avoid `Any` where possible)
- Don't annotate return types when Python can infer them. Annotate when return type is non-obvious or `Any` would otherwise be inferred.
- Comments should be only with `#` and should not contain docstring syntax unless defining module/class/function documentation.
- If you duplicate a substantial block of code, add a comment above it noting the duplication and referencing the original location.
- When creating pytest tests, organize tests logically with `class` grouping or parametrized tests.
- Focus on testing essential behavior and edge cases — avoid adding tests for every minor detail.
- Avoid duplicating code in tests; use `pytest.mark.parametrize` or shared fixtures instead of repeating similar test blocks.
- Do not make white space changes - do not add unnecessary new lines, or spaces to existing code, or wrap existing code.
- If you add a new Python file, ensure it follows the module structure and update `__init__.py` files as needed.
- When an unknown word is detected by spell checker, handle it as per project specification.
- To type-check, use `mypy` or `pyright`. For linting, use `pylint` or `flake8`.
- Default to no comments. Only add one when the why is non-obvious (workaround, hidden constraint, subtle invariant). Never explain what the code does — names handle that. Keep necessary comments to a minimum.
- Database queries should be abstracted into data access layers or ORM models.
- Follow PEP 8 style guide for Python code.

## Performance Optimization

MONTIAI prioritizes performance:
- Use type hints for better performance and IDE support
- Leverage async/await for I/O-bound operations
- Profile code bottlenecks before optimizing
- Document performance-critical sections
- Use appropriate data structures (dict for lookups, list for sequences)

## Full Documentation

- Coding style: [readme/dev/coding_style.md](readme/dev/coding_style.md)
- Contributing: [CONTRIBUTING.md](CONTRIBUTING.md)
