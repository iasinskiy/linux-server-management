# Linux Server Management Project

## 1. Project Purpose
Automated Bash scripts and technical documentation designed for Linux server administration, monitoring, user setup, and backups.

## 2. Project Structure
linux-server-management/
├── scripts/
│   ├── system_info.sh
│   ├── user_management.sh
│   └── backup.sh
├── docs/
│   ├── installation.md
│   ├── configuration.md
│   └── troubleshooting.md
├── .gitignore
└── README.md

## 3. Development Workflow
1. Create a dedicated feature branch for any task.
2. Commit changes with clean, semantic commit messages (`feat:`, `docs:`, `refactor:`, `fix:`).
3. Push the feature branch to GitHub and open a Pull Request (PR) to `main`.
4. Conduct Code Review, address inline review comments, and push fix commits.
5. Merge PR into `main` after checks pass.

## 4. Branching Strategy
- `main`: Production-ready, stable codebase.
- `feature/*`: Short-lived branches for developing new scripts, docs, or configuration changes.

## 5. Contribution Process
- Branch naming convention: `feature/<feature-name>`.
- Always open a PR against `main` for changes.
- Address all review comments before merging.

## 6. Testing Process
- Make scripts executable: `chmod +x scripts/*.sh`.
- Execute scripts inside Git Bash / Linux environment to verify system stats and error handling.
- Verify strict error mode (`set -euo pipefail`) in shell scripts.

## 7. Troubleshooting Process
- **Merge Conflicts**: Merge `main` into your feature branch, resolve markers (`<<<<<<<`), stage, and commit.
- **Faulty Commits**: Use `git revert <commit_hash>` for non-destructive rollback.
- **Detailed Guides**: Refer to `docs/troubleshooting.md` for specific script diagnostic steps.
