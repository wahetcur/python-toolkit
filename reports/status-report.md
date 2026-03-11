# Status Report - wahetcur - 2026-03-11

## Open Issues

_No open issues found in the repository._

## Reference Notes

- Python distinguishes **syntax errors** (detected by the parser) from **exceptions** (runtime errors).
- Use `try`/`except` blocks to catch and handle exceptions. Multiple `except` clauses can handle different exception types.
- An `else` clause runs only if no exception occurred in the `try` block, useful for code that should execute when the operation succeeds.
- A `finally` clause (not shown in the fetched snippets but part of the tutorial) executes cleanup code regardless of whether an exception was raised.
- Use `raise` to trigger exceptions manually, either by raising an existing exception instance or by specifying an exception class.
- Exception chaining (`raise NewError from original`) links a new exception to the original cause; `from None` suppresses chaining.
- Custom exceptions should inherit from `Exception` (or a subclass) and are typically named with an `Error` suffix.
- The base class `BaseException` covers system‑level exceptions like `SystemExit` and `KeyboardInterrupt` that usually are not caught.
- Good practice: catch the most specific exceptions possible and avoid catching the generic `Exception` unless re‑raising after logging.
