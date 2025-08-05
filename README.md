# Gestia

**Gestia** is currently being developed for the internal use of the marketing department of a multi-branch retail company.  
It’s designed to streamline everyday logistics, improve internal communication, and centralize tools across various teams (e.g., Events, Design, Digital).  
This project aims to reduce manual overhead and provide intelligent automation with customizable integrations (Google Drive, Adobe CC, etc.).

---

## 🚀 Project Status

This project is in its early planning and development phase.  
More detailed documentation will be added as features are implemented.

## 📋 Project Management

You can view the active roadmap and tasks on our GitHub Project board:  
👉 [Gestia GitHub Project](https://github.com/users/ernest0dev/projects/2)

Issues are categorized by feature and linked to pull requests for better traceability.

## 🧪 Requirements

- Node.js 18+
- Git
- MySQL
- .env file with appropriate API keys and config

---

## 📦 Installation (for development)

```bash
# Clone the repository
git clone https://github.com/ernest0dev/gestia.git
cd gestia

# Install dependencies
cd backend
npm install

cd ../frontend
npm install
```

## Running the Project (development mode)

```bash
# Run backend
cd backend
npm run dev

# Run frontend
cd ../frontend
npm run dev
```

## General Project Structure

- `main`: Protected branch. Contains stable, production-ready code.
- `dev`: Integration branch. All developments are merged here before going to `main`.
- `feature/*`: New features.
- `fix/*`: Bug fixes.
- `docs/*`: Documentation changes.
- `hotfix/*`: Critical issues that require going directly to production.

## Development Flow

1. Clone the repository and enter the branch `dev`
```bash
git checkout dev
git pull origin dev
```

2. Create a new functional branch
```bash
git checkout -b feature/name
```
Use semantic prefixes:
| Type | Prefix | Example |
| ------------- | ---------- | ----------------------- |
| Function | `feature/` | `feature/auth-login` |
| Fix | `fix/` | `fix/error-login` |
| Documentation | `docs/` | `docs/api-integrations` |
| Experiment | `test/` | `test/adobe-api-poc` |

3. Readable commits
```bash
git add .
git commit -m "feat: implements login and user authentication"
```

4. Upload the branch and create the PR
```bash
git push origin feature/auth-login
```
- Make a Pull Request to `dev`
- Associate the PR with an Issue (`Closes #X`)
- Add tags and a clear description

---

## Rules for Pull Requests

- Clearly describe what the PR does.
- Do not touch files outside of the assigned role.
- Include screenshots or evidence, if applicable.
- If the UI has been modified, add screenshots or GIFs.

---

## Contributing
I appreciate your contributions!
- If you want to contribute, create a fork, follow this README, and submit your PR from dev.
- For suggestions, create an Issue.
- Everything must be documented and follow best practices.
Please fork the repository and submit a pull request with your suggestions.

## License

This project is released under a customized MIT-style license:

- ✅ You may view, fork, and contribute to this project freely.
- ✅ You may reuse parts of the code for educational or personal use.
- ❌ **Commercial use is not allowed** under this license.
- 🔁 To use it commercially, you must either:
  - Request explicit permission from the maintainer, or
  - Fork the project and change the license accordingly.

For full legal terms, please refer to the `LICENSE` file.
