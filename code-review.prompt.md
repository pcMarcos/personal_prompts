Senior Engineer Code Review Checklist:

1. Risks & Concerns:
- Identify major risks or issues (security, reliability, maintainability, compatibility, scalability). Rate impact (High/Med/Low). For each concern, suggest a concrete fix with reasoning.

2. Tests:
- Is there sufficient unit test coverage? List gaps. Are tests meaningful and well-written? Note brittle/unclear cases. Do tests follow repo test guidelines and best practices (fixtures, teardown, naming, assertions)?

3. Guidelines & Best Practices:
- Does the repo have coding guidelines/docs? Were they followed? Cite clear examples of compliance or issues. If missing, note it. Is code idiomatic and style consistent with repo and language norms?

4. Overengineering & Simplicity:
- Any overengineering, premature optimization, or complexity? Point out specifics and suggest simpler options.

5. Code Smells & Maintainability:
- Note code smells (large funcs, deep nesting, repetition, magic values, unclear responsibility, commented code). Suggest refactors. Highlight any unclear/hard-to-maintain parts and how to clarify.

6. Decision:
- Ship it or Block it? Briefly justify. List blockers if blocking.

Use concise bullet points. No markdown formatting needed.