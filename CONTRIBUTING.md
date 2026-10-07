# Contributing to Researchments & D. 🤝

Thank you for contributing to **Researchments & D.**! Whether you're Mark's friend, an invited collaborator, or an open-source contributor, we are excited to build and experiment together.

---

## 🎯 Getting Started

### 1. Prerequisites & Cloning
Clone the repository locally:
```bash
git clone https://github.com/marksrv047/Researchments-D.git
cd Researchments-D
```

### 2. Proposing a Project or Experiment
Before diving into major code writing, it is recommended to open an issue or message the team:
- Use the **[Project Proposal](.github/ISSUE_TEMPLATE/project_proposal.md)** issue template.
- Outline the concept, goals, tech stack, and members collaborating on it.

---

## 🌳 Branching Strategy

To keep the `main` branch stable, please work in isolated feature or topic branches:

| Branch Prefix | Purpose | Example |
| :--- | :--- | :--- |
| `feat/` | A new tool, app, or major feature | `feat/neural-net-visualizer` |
| `research/` | Analysis, paper reviews, or data exploration | `research/transformer-benchmarks` |
| `exp/` | Quick experimental prototypes | `exp/websocket-chat-demo` |
| `docs/` | Documentation, guides, or README updates | `docs/update-contributing` |
| `fix/` | Bug fixes or dependency updates | `fix/broken-api-route` |

Create and switch to your branch:
```bash
git checkout -b feat/your-project-title
```

---

## 📁 Organizing Your Project in `projects/`

To prevent dependency clashes and keep the repo organized:

1. Create a dedicated subdirectory under `projects/`:
   ```bash
   mkdir projects/your-project-name
   ```
2. Include a project-specific `README.md` following this structure:
   - **Project Name & Description**
   - **Key Features / Research Hypothesis**
   - **Setup & Installation** (e.g. `pip install -r requirements.txt` or `npm install`)
   - **How to Run / Demo**
   - **Team Members & Credits**
3. Keep all project-specific assets, dependencies (`requirements.txt`, `package.json`, etc.), and code contained within that folder.

---

## 📝 Commit Guidelines

Keep commit messages concise and descriptive:

- `feat(project-name): add initial backend scaffolding`
- `research(nlp): add benchmarking notebook for model eval`
- `docs: update projects showcase in main README`
- `fix(auth): correct token validation logic`

---

## 🚀 Submitting a Pull Request (PR)

1. **Commit and Push:**
   ```bash
   git add .
   git commit -m "feat(project-name): implement MVP"
   git push origin feat/your-project-title
   ```
2. **Open a PR:** Go to GitHub and open a Pull Request targeting `main`.
3. **Fill the PR Template:** Complete the checklist and describe what you built or changed.
4. **Peer Review:** Request a review from Mark (`@marksrv047`) or fellow project collaborators.
5. **Merge:** Once approved, your work is merged into `main`! Don't forget to update the project table in `README.md`.

---

## 💡 Code Quality & Best Practices
- **Do not commit secrets:** Never commit API keys, `.env` files, passwords, or personal credentials.
- **Clean dependencies:** Ensure package files (`requirements.txt`, `package.json`) reflect only what is needed.
- **Documentation:** Every sub-project should be reproducible by another teammate within 5 minutes.
