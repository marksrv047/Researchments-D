# Projects Directory

This directory contains all independent software projects, prototypes, and research code developed by our collective.

---

## Structure and Organization

Each project is isolated in its own folder to ensure modularity and clean dependency isolation:

```text
projects/
├── _template/            # Starter README template for new projects
├── project-alpha/        # Standalone sub-project
│   ├── src/
│   ├── requirements.txt  # (or package.json, Cargo.toml, etc.)
│   └── README.md         # Documentation specific to project-alpha
└── project-beta/
    └── ...
```

---

## Adding a New Project

1. Copy `projects/_template` into a new folder:
   ```bash
   mkdir projects/my-project-name
   ```
2. Copy `projects/_template/README.md` into your new folder and populate your project's details.
3. Add your source code, configuration files, and dependencies.
4. Update the [Project Showcase](../README.md#projects-showcase) in the root `README.md`.
