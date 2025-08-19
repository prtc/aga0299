# PAULA.md

Personal reference guide for working with this repository across different devices.

## Repository Information

- **Repository**: `aga0299-lab-beginners-guide`
- **URL**: https://github.com/prtc/aga0299-lab-beginners-guide
- **Description**: Course materials for AGA0299 Lab - Beginner's Guide to Astronomical Data

## Essential Git Commands

### Initial Setup (First Time on New Device)

```bash
# Clone the repository
git clone https://github.com/prtc/aga0299-lab-beginners-guide.git

# Navigate to the project
cd aga0299-lab-beginners-guide

# Set up your identity (if not already configured globally)
git config user.name "Your Name"
git config user.email "your.email@example.com"
```

### Daily Workflow

```bash
# Check current status
git status

# Pull latest changes from remote
git pull

# Add changes to staging
git add .                    # Add all changes
git add filename.ext         # Add specific file

# Commit changes
git commit -m "Description of changes"

# Push changes to remote
git push
```

### Quick Reference

```bash
# See what changed
git diff                     # Unstaged changes
git diff --staged           # Staged changes

# View commit history
git log --oneline           # Compact view
git log                     # Detailed view

# Undo changes (careful!)
git checkout -- filename   # Discard unstaged changes to file
git reset HEAD filename     # Unstage file
```

## Quarto Commands

```bash
# Render all documents
quarto render

# Live preview during development
quarto preview

# Render specific presentation
quarto render file.qmd --to revealjs

# Render as HTML course page
quarto render file.qmd --to html
```

## Project Workflow Reminder

1. **Before starting work**: `git pull`
2. **Make your changes** to .qmd files
3. **Test**: `quarto render` to ensure everything works
4. **Stage changes**: `git add .`
5. **Commit**: `git commit -m "Descriptive message"`
6. **Push**: `git push`

## Emergency Commands

```bash
# If you're lost, check where you are
pwd
git status
git log --oneline -5

# If you need to abandon local changes
git reset --hard HEAD       # DANGER: Loses all uncommitted work

# If push is rejected, pull first
git pull --rebase
git push
```

## Notes

- Always `git pull` before starting work on a new device
- Write clear commit messages describing what you changed
- Test with `quarto render` before committing
- When in doubt, `git status` is your friend