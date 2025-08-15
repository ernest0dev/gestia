# Gestia

**Gestia** is an open-source platform currently in development, designed to optimize the internal operations of marketing teams within multi-branch organizations.  
Its primary goal is to streamline workflows, enhance communication between subteams, and centralize access to essential tools (e.g., Events, Design, Digital).  
With built-in automation and optional integrations (Google Drive, Adobe CC, and more), Gestia aims to reduce repetitive manual work while improving overall efficiency.

---

## Project Status

Gestia is in the **early planning and development phase**.  
Core features are being built following a structured roadmap, with public documentation updated as progress continues.

📖 Detailed information is available in the [project Wiki](https://github.com/ernest0dev/gestia/wiki).  
📌 Task tracking and milestones are managed via the [GitHub Project Board](https://github.com/users/ernest0dev/projects/2).

---

## Requirements

- Node.js 18+
- Git
- MySQL
- `.env` file with required API keys and configuration

---

## Installation (Development Setup)
#### Clone repository
```bash
git clone https://github.com/ernest0dev/gestia.git
cd gestia
```
#### Install backend dependencies
```bash
cd backend
npm install
```
#### Install frontend dependencies
```bash
cd ../frontend
npm install
```

## Running the Project (Development Mode)
#### Run backend
```bash
cd backend
npm run dev
```
#### Run frontend
```bash
cd ../frontend
npm run dev
```

## Branching Strategy
- `main` → Stable production-ready code (protected branch)
- `dev` → Integration branch for testing before merging into main
- `feature/*` → New features
- `fix/*` → Bug fixes
- `docs/*` → Documentation changes
- `hotfix/*` → Critical fixes deployed directly to production

## Development Workflow
1. Checkout `dev` branch
```bash
git checkout dev
git pull origin dev
```
3. Create a new branch
```bash
git checkout -b feature/short-description
```

### Semantic branch prefixes:
| Type          | Prefix     | Example                 |
| ------------- | ---------- | ----------------------- |
| Feature       | `feature/` | `feature/auth-login`    |
| Fix           | `fix/`     | `fix/error-login`       |
| Documentation | `docs/`    | `docs/api-integrations` |
| Experiment    | `test/`    | `test/adobe-api-poc`    |

3. Readable commits
```bash
git add .
git commit -m "feat: implements login and user authentication"
```
5. Push branch & create PR
```bash
git push origin feature/auth-login
```
- PR must target dev
- Link the PR to its Issue (Closes #X)
- Add labels and a clear description

## Pull Request Rules
- Clearly explain what the PR does
- Only modify files related to the assigned task
- Include screenshots or examples if relevant
- If UI changes were made, attach visual previews (images/GIFs)

Contributing
We welcome contributions!
- Fork the repository, follow the CONTRIBUTING.md guidelines, and submit your PR to `dev`.
- For suggestions or bug reports, open an Issue with enough detail to reproduce or understand your proposal.
- Maintain code style and documentation standards.

## License
This project is distributed under a customized MIT-style license:
-  Free to view, fork, and contribute
-  Code reuse allowed for educational or personal use
- Commercial use prohibited without explicit permission
- For commercial usage:
  - Request authorization from the maintainer or
  - Fork the project and apply your own license
Full terms available in the LICENSE file.
