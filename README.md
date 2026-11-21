# DevSec Class Project

A project outlining proficiency in configuring security throughout the SDLC.

## Security

- Secrets are never committed. `.env` files, keys and certificates are ignored by `.gitignore`.
- `main` is protected: changes go through pull requests.
- GitHub secret scanning, push protection and Dependabot alerts are enabled.
- AI coding assistants used on this project follow the guardrails in [`CLAUDE.md`](CLAUDE.md):
  least-privilege, read-only cloud access by default, and human approval before any change.
