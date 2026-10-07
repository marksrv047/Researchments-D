# Projects Directory 🛠️

This folder contains all independent software projects, prototypes, and research code developed by our team.

---

## 📂 How It Works

Each project is self-contained in its own folder to ensure modularity and clean dependency isolation:

```text
projects/
├── _template/            # Starter README template for new projects
├── project-alpha/        # Standalone project
│   ├── src/
│   ├── requirements.txt  # (or package.json, Cargo.toml, etc.)
│   └── README.md         # Documentation specific to project-alpha
└── project-beta/
    └── ...
```

---

## 🚀 Adding a New Project

1. Duplicate `projects/_template` or create a new folder:
   ```bash
   mkdir projects/my-project-name
   ```
2. Copy `projects/_template/README.md` into your new folder and fill in your project's details.
3. Add your source code, configuration files, and dependencies list.
4. Update the [Project Showcase](../README.md#-projects-showcase) in the root `README.md`.
