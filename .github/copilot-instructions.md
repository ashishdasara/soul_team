# Repository context for GitHub Copilot

- This is a Ruby 3.4 / Rails 8 application using Rails conventions and Minitest.
- Use the repository's existing patterns before introducing a new abstraction.
- When implementation guidance depends on repository behavior, ground the answer in relevant source files.
- Cite file paths and include a brief source summary.
- Prefer `bin/rails` and the existing `bin/rubocop` / `bin/brakeman` commands.
- Do not commit generated `rag/index.json` files or secrets.
- For RAG-related work, use `Rag::Pipeline` and `Rag::IndexBuilder`.
- Keep issue workflow answers grounded in retrieved repository context and say when evidence is insufficient.
- For implementation tasks from GitHub Issues, make the smallest complete code change, add or update focused tests, and open a pull request.
- Verify changes with the focused test command, `bin/rubocop`, and `bin/brakeman` when relevant.
- Do not commit generated `rag/index.json` files or expand the change beyond the issue requirements.
