# Contributing to Coffee Joy

Thank you for your interest in contributing to Coffee Joy!

## Branch Structure

This repository uses the following branch structure:

- **`main`**: The primary development branch. All development work should be based on this branch.
- **`gh-pages`**: Automatically generated deployment branch for GitHub Pages. This branch is created and updated automatically by our CI/CD workflow and should not be modified manually.

### Feature Branches

When contributing, please create feature branches from `main`:

```bash
git checkout main
git pull origin main
git checkout -b feature/your-feature-name
```

### Viewing All Branches

If you've cloned the repository and can't see all branches, make sure your git is configured to fetch all branches:

```bash
# Fetch all remote branches
git fetch --all

# View all branches (local and remote)
git branch -a

# View only remote branches
git branch -r
```

If you still don't see all branches, verify your git remote configuration:

```bash
git config --get-all remote.origin.fetch
```

This should output: `+refs/heads/*:refs/remotes/origin/*`

If it shows something different, update it with:

```bash
git config remote.origin.fetch "+refs/heads/*:refs/remotes/origin/*"
git fetch --all
```

## Development Workflow

1. Fork the repository
2. Create a feature branch from `main`
3. Make your changes
4. Test your changes locally
5. Commit with clear, descriptive messages
6. Push your feature branch
7. Create a Pull Request to the `main` branch

## Questions?

If you have any questions or run into issues, please open an issue on GitHub.
