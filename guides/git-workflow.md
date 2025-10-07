# Git Workflow Guide

**Difficulty:** Beginner  
**Estimated Time:** 30 minutes  
**Prerequisites:** Basic Git knowledge

## Overview

This guide describes the Git workflow used by the DTRG team for version control and collaboration.

## What You'll Learn

- Branch naming conventions
- Commit message standards
- Pull request workflow
- Code review process

## Prerequisites

Before starting, you should:
- [ ] Have Git installed
- [ ] Have access to the team's GitHub repositories
- [ ] Have basic understanding of Git commands

## Branching Strategy

### Main Branches

**`main`** (or `master`)
- Production-ready code
- Protected branch (requires PR and review)
- Never commit directly to main

**`develop`** (if used)
- Integration branch for features
- Used in projects with formal release cycles

### Feature Branches

Create a new branch for each feature, fix, or change:

```bash
# Create and switch to a new branch
git checkout -b feature/your-feature-name

# Or for bug fixes
git checkout -b fix/bug-description

# Or for documentation
git checkout -b docs/documentation-update
```

### Branch Naming Conventions

Use descriptive, kebab-case names with prefixes:

- `feature/` - New features
- `fix/` - Bug fixes
- `docs/` - Documentation updates
- `refactor/` - Code refactoring
- `test/` - Adding or updating tests
- `chore/` - Maintenance tasks

Examples:
- `feature/user-authentication`
- `fix/login-error-handling`
- `docs/api-documentation`
- `refactor/database-queries`

## Commit Messages

### Format

```
<type>: <subject>

<body (optional)>

<footer (optional)>
```

### Types

- `feat:` - New feature
- `fix:` - Bug fix
- `docs:` - Documentation changes
- `style:` - Code style changes (formatting, no logic change)
- `refactor:` - Code refactoring
- `test:` - Adding or updating tests
- `chore:` - Maintenance tasks

### Examples

Good commit messages:
```
feat: add user authentication system

Implements JWT-based authentication with refresh tokens.
Includes middleware for protected routes.

Closes #123
```

```
fix: resolve database connection timeout

Increases connection pool size and adds retry logic
to handle temporary network issues.
```

```
docs: update API documentation for new endpoints
```

### Best Practices

- Use present tense ("add" not "added")
- First line is 50 characters or less
- Capitalize first letter
- No period at the end of subject line
- Blank line between subject and body
- Body explains what and why (not how)
- Reference issues/PRs in footer

## Pull Request Workflow

### 1. Create Your Branch

```bash
git checkout -b feature/your-feature
```

### 2. Make Your Changes

```bash
# Make changes to files
git add .
git commit -m "feat: descriptive commit message"
```

### 3. Keep Your Branch Updated

```bash
# Fetch latest changes
git fetch origin

# Rebase on main (or merge if preferred by project)
git rebase origin/main

# Or merge
git merge origin/main
```

### 4. Push Your Branch

```bash
git push origin feature/your-feature
```

### 5. Create Pull Request

1. Go to the repository on GitHub
2. Click "New Pull Request"
3. Select your branch
4. Fill in the PR template:
   - Clear title
   - Description of changes
   - Related issues
   - Testing performed
   - Screenshots (if UI changes)

### 6. Address Review Comments

```bash
# Make requested changes
git add .
git commit -m "fix: address review comments"
git push origin feature/your-feature
```

### 7. Merge

Once approved, merge using the project's preferred method:
- Squash and merge (default for most projects)
- Rebase and merge
- Create merge commit

## Code Review Process

### As a Reviewer

- Review code for correctness, style, and maintainability
- Check tests and documentation
- Be constructive and respectful
- Approve or request changes

### As an Author

- Respond to all comments
- Make requested changes or explain why not
- Re-request review after updates
- Thank reviewers for their time

## Common Git Commands

```bash
# Check status
git status

# See changes
git diff

# Create branch
git checkout -b branch-name

# Switch branches
git checkout branch-name

# Update from remote
git pull origin main

# View commit history
git log --oneline

# Undo last commit (keep changes)
git reset --soft HEAD~1

# Discard local changes
git checkout -- filename
```

## Troubleshooting

### Merge Conflicts

```bash
# When you encounter a conflict
git status  # See conflicting files

# Edit files to resolve conflicts
# Look for <<<<<, =====, >>>>> markers

git add resolved-file
git commit
```

### Accidentally Committed to Main

```bash
# Move commits to a new branch
git branch feature/my-feature
git reset --hard origin/main
git checkout feature/my-feature
```

### Need to Update Branch with Main

```bash
# Option 1: Rebase (cleaner history)
git checkout feature/my-feature
git fetch origin
git rebase origin/main

# Option 2: Merge
git checkout feature/my-feature
git merge origin/main
```

## Best Practices

1. **Commit often**: Small, focused commits are easier to review
2. **Pull frequently**: Stay up-to-date with main branch
3. **Test before pushing**: Ensure code works and tests pass
4. **Write good messages**: Future you will thank you
5. **Keep PRs focused**: One feature/fix per PR when possible
6. **Review your own code first**: Catch obvious issues before requesting review

## Additional Resources

- [Pro Git Book](https://git-scm.com/book/en/v2)
- [GitHub Flow Guide](https://guides.github.com/introduction/flow/)
- [Conventional Commits](https://www.conventionalcommits.org/)

---

*For team-specific Git policies, see [Rules & Guidelines](../rules/)*
