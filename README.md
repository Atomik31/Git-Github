# 📚 Git Cheat Sheet - Essential Git Commands Reference

A comprehensive reference guide for the most important and commonly used Git commands.

## 📖 About

Git is the free and open source distributed version control system that handles everything GitHub-related happening locally on your computer. This cheat sheet compiles essential Git commands for quick reference.

## 🚀 Installation

### Windows
[GitHub Desktop for Windows](https://windows.github.com)

### macOS
[GitHub Desktop for Mac](https://mac.github.com)

### Linux and Solaris
[Git for All Platforms](http://git-scm.com)

## 📋 Essential Commands

### Initial Setup

Configuring user information for all local repositories:

```bash
# Set your username
git config --global user.name "[firstname lastname]"

# Set your email address
git config --global user.email "[valid-email]"

# Enable automatic command line coloring
git config --global color.ui auto
```

### Initialize and Clone

```bash
# Initialize a Git repository in an existing directory
git init

# Clone a remote repository
git clone [url]
```

### Stage & Snapshot

Working with snapshots and the Git staging area:

```bash
# Show modified files
git status

# Add a file to the staging area
git add [file]

# Unstage a file
git reset [file]

# View unstaged differences
git diff

# View staged differences
git diff --staged

# Create a commit
git commit -m "[descriptive message]"
```

### Branch & Merge

Isolating work in branches and integrating changes:

```bash
# List branches (* indicates the active branch)
git branch

# Create a new branch
git branch [branch-name]

# Switch to another branch
git checkout [branch-name]

# Merge a branch into the current one
git merge [branch]

# Show commit history
git log
```

### Share & Update

Retrieving and sending updates:

```bash
# Add a remote repository
git remote add [alias] [url]

# Fetch remote branches
git fetch [alias]

# Merge a remote branch
git merge [alias]/[branch]

# Push local commits to remote repository
git push [alias] [branch]

# Fetch and merge automatically
git pull
```

### Tracking Path Changes

```bash
# Delete a file and stage the removal
git rm [file]

# Move/rename a file
git mv [existing-path] [new-path]

# Show history with file movements
git log --stat -M
```

### Temporary Commits (Stash)

Temporarily saving modifications:

```bash
# Stash modified changes
git stash

# List stashed changes
git stash list

# Apply the latest stash
git stash pop

# Discard the latest stash
git stash drop
```

### Inspect & Compare

```bash
# Show history of the active branch
git log

# Compare two branches
git log branchB..branchA

# Follow a file's history
git log --follow [file]

# Compare differences between branches
git diff branchB...branchA

# Show a specific Git object
git show [SHA]
```

### Rewrite History

```bash
# Rebase a branch
git rebase [branch]

# Hard reset to a specific commit
git reset --hard [commit]
```

### Ignoring Patterns

Configuring patterns to ignore:

```bash
# Set a global exclusion file
git config --global core.excludesfile [file]
```

Example `.gitignore` file:

```
logs/
*.notes
pattern*/
```

## 🎓 Educational Resources

GitHub is free for students and teachers. Discounts are available for other educational uses.

**Contact:** education@github.com  
**Website:** [education.github.com](https://education.github.com)

## 📄 License

This cheat sheet is based on the official GitHub Education documentation.

## 🤝 Contributing

Feel free to suggest improvements via pull requests!

---

**Note:** For more detailed information, consult the [official Git documentation](https://git-scm.com/doc).