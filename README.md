# ChillTrace

ChillTrace is a **fictional** London company that monitors café-chain fridges with IoT
sensors. Each sensor proves its identity with its own certificate through AWS IoT Core.
It's a portfolio project showing security across the whole SDLC. All data is fake.



## Security

- Secrets are never committed. `.env` files, keys and certificates are ignored by `.gitignore`.
- `main` is protected: changes go through pull requests.
- GitHub secret scanning, push protection and Dependabot alerts are enabled.
- Secrets are also scanned with [gitleaks](https://github.com/gitleaks/gitleaks), locally before each
  commit and in CI on every pull request. After cloning, run once: `pre-commit install`.
- AI coding assistants used on this project follow the guardrails in [`CLAUDE.md`](CLAUDE.md):
  least-privilege, read-only cloud access by default, and human approval before any change.
