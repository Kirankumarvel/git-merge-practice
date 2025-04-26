# Git Merge Practice

This repository is a practice project for learning and experimenting with Git merge operations, including creating branches, committing changes, and resolving merge conflicts. It serves as an excellent resource for beginners and intermediate developers to understand Git workflows and conflict resolution techniques.

---

## 📚 What You’ll Learn
- How to create and switch branches in Git.
- Committing and pushing changes to remote repositories.
- Performing merges, including fast-forward merges and conflict resolution.
- Best practices for Git workflows in collaborative environments.

---

## 🛠 Steps Followed in This Project

### 1. **Cloned the Repository**
   The repository was cloned from GitHub to a local machine to start practicing Git commands:
   ```bash
   git clone https://github.com/Kirankumarvel/git-merge-practice.git
   cd git-merge-practice
   ```

### 2. **Created a Feature Branch**
   A new branch called `feature-branch` was created from the `main` branch:
   ```bash
   git checkout -b feature-branch
   ```

### 3. **Made Changes on Feature Branch**
   Changes were made in the `feature-branch`, such as adding a new line of text to the `README.md` file:
   ```bash
   echo "Feature 1 implemented" >> README.md
   git add README.md
   git commit -m "Added Feature 1 details"
   ```

### 4. **Pushed the Feature Branch**
   The changes made in the feature branch were pushed to the remote repository:
   ```bash
   git push origin feature-branch
   ```

### 5. **Merged the Feature Branch into Main**
   The changes from the `feature-branch` were merged into the `main` branch:
   ```bash
   git checkout main
   git merge feature-branch
   git push origin main
   ```
   - A **fast-forward merge** was performed if no conflicts were present.

### 6. **Resolved Merge Conflicts**
   In case of merge conflicts:
   - Conflicted files were manually edited.
   - Post-resolution, the following commands were used:
     ```bash
     git add <conflicted-file>
     git commit -m "Resolved merge conflict"
     git push origin main
     ```

---

## 🚀 Commands Used

### Create a New Branch
```bash
git checkout -b feature-branch
```

### Make Changes and Commit
```bash
echo "Feature 1 implemented" >> README.md
git add README.md
git commit -m "Added Feature 1 details"
```

### Push the Feature Branch
```bash
git push origin feature-branch
```

### Switch to Main and Merge
```bash
git checkout main
git merge feature-branch
```

### Push the Merged Changes
```bash
git push origin main
```

---

## 🎯 What You Can Learn from This Repository
- **Branch Creation and Management**: Understand how to create, switch, and manage branches in Git.
- **Pushing Changes**: Learn how to push local changes to remote repositories.
- **Merging Branches**: Practice merging feature branches into the main branch, including fast-forward merges.
- **Conflict Resolution**: Gain hands-on experience resolving merge conflicts and committing the resolved changes.
- **Git Best Practices**: Discover the importance of regular commits, meaningful commit messages, and keeping branches in sync.

---

## 📂 Project Structure
- **README.md** — Detailed instructions and project overview.
- **Feature files** — Example files created or modified during the practice sessions.

---

## 💡 Tips for Practicing
1. Always pull the latest changes from the `main` branch before merging to avoid unnecessary conflicts:
   ```bash
   git pull origin main
   ```
2. Use `git status` frequently to check the status of your working directory and staged files.
3. If you encounter conflicts during a merge:
   - Open the conflicted files in a text editor.
   - Resolve conflicts by manually editing the files.
   - Use `git add` to stage the resolved files and `git commit` to finalize the merge.

---

## 📢 Note
This repository is for **educational purposes** only. Feel free to fork it, clone it, and use it to practice Git commands and workflows.

---

## 📜 License
This project is open-source and available under the **MIT License**.  
See the [LICENSE](LICENSE) file for more details.

