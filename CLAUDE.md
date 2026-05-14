# VERY IMPORTANT
- Be simple. Approach tasks in a simple, incremental way.
- Work incrementally ALWAYS. Small, simple steps. Validate and check each increment before moving on.
- Use LATEST apis as of NOW
- Assume the environment is air-gapped or restricted by default. Confirm connectivity requirements before coding.

# MANDATORY Code Style
- Do not overengineer. Do not program defensively. Use exception managers only when needed.
- Identify root cause before fixing issues. Prove with evidence, then fix.
- Work incrementally with small steps. Validate each increment.
- Use latest library APIs.
- Use `uv` as Python package manager. Always `uv run xxx` never `python3 xxx`, always `uv add xxx` never `pip install xxx`
- Favor clear, concise docstring comments. Be sparing with comments outside docstrings.
- Favor small modules, short methods and functions. Name things clearly.
- Never use emojis in code or in print statements or logging.
- Keep README.MD concise.

# Security & Sensitive Data Handling
- Never hardcode credentials, API keys, tokens, or secrets. Always use environment variables or a secrets manager.
- Never log sensitive data (passwords, tokens, PII, IOCs in raw form).
- Treat all external input as untrusted. Sanitize before processing.
- When handling malware samples, IOCs, or raw threat data, isolate in dedicated functions/modules — never mix with business logic.
- No external network calls without explicit justification in a comment.
- Any script that modifies, deletes, or exports data must require explicit confirmation (`--confirm` flag or equivalent).


# Important - debugging and fixing
- When troubleshooting problems, ALWAYS identify root cause BEFORE fixing
- Reproduce consistently.
- PROVE THE PROBLEM FIRST - don't guess.
- Try one test at a time. Be methodical.
- Don't jump to conclusions. Don't apply workarounds.
- Never run untested scripts against production data or live security systems.
- Log what you do. Forensic auditability matters.