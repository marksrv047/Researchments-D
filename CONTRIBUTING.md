# Contributing to Researchments & D.

Thank you for contributing to **Researchments & D.**! Whether you are an invited collaborator, team member, or open-source contributor, this document outlines our development workflow and standards.

---

## Getting Started

### 1. Prerequisites and Cloning
Clone the repository locally:
```bash
git clone https://github.com/marksrv047/Researchments-D.git
cd Researchments-D
```

### 2. Proposing a Project or Experiment
Before starting substantial implementation, discuss the initiative with the team:
- Submit an issue using the [Project Proposal](.github/ISSUE_TEMPLATE/project_proposal.md) template.
- Specify objectives, planned deliverables, architecture, and team members involved.

---

## Branching Strategy

To maintain stability on `main`, all contributions must be developed on dedicated branches:

| Branch Prefix | Scope | Example |
| :--- | :--- | :--- |
| `feat/` | New application, utility, or capability | `feat/neural-net-visualizer` |
| `research/` | Analysis, paper reviews, or data exploration | `research/transformer-benchmarks` |
| `exp/` | Exploratory proofs of concept | `exp/websocket-chat-demo` |
| `docs/` | Documentation, guides, or specifications | `docs/update-architecture` |
| `fix/` | Bug fixes or dependency resolutions | `fix/broken-api-route` |

Create and switch to your branch:
```bash
git checkout -b feat/your-project-title
```

---

## Organizing Projects in `projects/`

To prevent dependency conflicts and keep the repository modular:

1. Create an isolated subdirectory under `projects/`:
   ```bash
   mkdir projects/your-project-name
   ```
2. Include a project-level `README.md` containing:
   - **Project Name and Summary:** One-line explanation of the project.
   - **Hypothesis / Features:** Key capabilities or research questions.
   - **Setup Instructions:** How to install dependencies (`pip install -r requirements.txt` or `npm install`).
   - **Execution Instructions:** How to run, test, or evaluate the code.
   - **Authors and Credits:** List of contributors and respective roles.
3. Keep all project-specific assets, configurations, and dependency lists strictly inside your project directory.

---

## Commit Guidelines

Use concise, imperative commit messages:

- `feat(project-name): add initial backend scaffolding`
- `research(nlp): add benchmarking notebook for model evaluation`
- `docs: update projects showcase in main README`
- `fix(auth): correct token validation logic`

---

## Pull Request Process

1. **Commit and Push:**
   ```bash
   git add .
   git commit -m "feat(project-name): implement MVP"
   git push origin feat/your-project-title
   ```
2. **Open a Pull Request:** Navigate to GitHub and submit a Pull Request targeting `main`.
3. **Fill the PR Template:** Complete all sections of the checklist.
4. **Peer Review:** Request a review from Mark (`@marksrv047`) or fellow project collaborators.
5. **Merge:** Once approved, merge into `main` and register the project in the root `README.md` showcase.

---

## Code Quality and Standards

- **Secret Management:** Never commit API keys, `.env` files, passwords, or personal credentials.
- **Dependency Hygiene:** Ensure package files reflect only necessary dependencies with pinned or compatible versions.
- **Reproducibility:** Sub-projects should include clear execution steps so any collaborator can run them in under five minutes.
