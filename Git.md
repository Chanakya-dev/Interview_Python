### **🔹 Basic Git Questions**  

#### **1. What is Git, and how does it work?**  
Git is a **distributed version control system (VCS)** that helps developers track changes in their code, collaborate efficiently, and maintain different versions of a project. It works by keeping a **history of changes**, allowing users to create branches, merge updates, and revert to previous states if needed.

#### **2. How is Git different from other version control systems like SVN?**  
| Feature      | Git (DVCS)      | SVN (CVCS) |
|-------------|----------------|------------|
| Repository Type | Distributed | Centralized |
| Branching  | Lightweight and fast | Slow and costly |
| Offline Work | Possible | Not possible |
| Speed | Faster | Slower |

#### **3. What are the key benefits of using Git?**  
- **Distributed System** – Every developer has a full copy of the repository.  
- **Branching and Merging** – Easy to create and manage branches.  
- **Fast and Lightweight** – Performs operations efficiently.  
- **Open Source** – Free and widely used.  

#### **4. Explain the difference between Git and GitHub.**  
- **Git** is a version control system that runs locally on your computer.  
- **GitHub** is a cloud-based platform for hosting Git repositories, collaborating on code, and managing pull requests.  

#### **5. What is a Git repository, and how do you create one?**  
A Git repository is a storage location where Git tracks files and changes.  
To create a new repository:  
```sh
git init
```

#### **6. What is the difference between a local repository and a remote repository?**  
- **Local Repository**: Exists on your local machine.  
- **Remote Repository**: Hosted on a server like GitHub/GitLab/Bitbucket.  

#### **7. How do you check the current status of a Git repository?**  
```sh
git status
```
This command shows modified, staged, and untracked files.

---

### **🔹 Git Branching & Merging**  

#### **8. What is a Git branch, and why is it useful?**  
A Git branch is an independent line of development. It helps developers work on new features without affecting the main codebase.

#### **9. How do you create a new branch in Git?**  
```sh
git branch feature-branch
```

#### **10. How do you switch between branches in Git?**  
```sh
git checkout feature-branch
```
or  
```sh
git switch feature-branch
```

#### **11. What is the difference between `git merge` and `git rebase`?**  
- **`git merge`**: Combines two branches, keeping both histories.  
- **`git rebase`**: Moves commits from one branch onto another, creating a linear history.

#### **12. What happens when there is a merge conflict, and how do you resolve it?**  
A merge conflict occurs when Git cannot automatically merge changes. To resolve:  
1. Open the conflicting file.  
2. Edit and resolve conflicts manually.  
3. Stage the resolved file:  
   ```sh
   git add filename
   ```
4. Commit the changes:  
   ```sh
   git commit -m "Resolved merge conflict"
   ```

#### **13. What is a fast-forward merge in Git?**  
A fast-forward merge occurs when there are no new commits on the target branch, so Git simply moves the branch pointer forward.

#### **14. How do you delete a branch in Git?**  
- **Local branch**:  
  ```sh
  git branch -d branch-name
  ```
- **Remote branch**:  
  ```sh
  git push origin --delete branch-name
  ```

---

### **🔹 Git Commit & History**  

#### **15. How do you add changes to a Git commit?**  
```sh
git add filename
git commit -m "Commit message"
```

#### **16. What is the difference between `git commit` and `git commit -m`?**  
- `git commit`: Opens an editor to enter a commit message.  
- `git commit -m "message"`: Adds a commit with a message directly.

#### **17. How do you view the commit history in Git?**  
```sh
git log
```
or for a compact view:  
```sh
git log --oneline
```

#### **18. How can you modify the last commit in Git?**  
```sh
git commit --amend
```
This allows you to edit the last commit message or add more changes.

#### **19. What is `git revert`, and how does it differ from `git reset`?**  
- `git revert`: Creates a new commit that undoes the changes of a previous commit.  
- `git reset`: Moves the branch pointer back to a previous commit, potentially losing changes.

#### **20. What is `git cherry-pick`, and when would you use it?**  
```sh
git cherry-pick commit-hash
```
It applies a specific commit from another branch without merging the whole branch.

---

### **🔹 Git Cloning, Fetching & Pulling**  

#### **21. What is the difference between `git fetch` and `git pull`?**  
- `git fetch`: Downloads changes but doesn’t merge them.  
- `git pull`: Fetches and merges changes automatically.

#### **22. How do you clone a Git repository?**  
```sh
git clone repository-url
```

#### **23. What is the purpose of `git remote`?**  
It manages remote repository connections.

#### **24. How do you check the list of remotes added to your local repository?**  
```sh
git remote -v
```

---

### **🔹 Git Stashing & Reset**  

#### **25. What is `git stash`, and how does it work?**  
It temporarily saves uncommitted changes without committing them.  
```sh
git stash
```

#### **26. How do you apply and drop a stash in Git?**  
```sh
git stash apply  # Apply last stashed changes
git stash drop   # Remove last stash
```

#### **27. What is the difference between `git reset --soft`, `git reset --mixed`, and `git reset --hard`?**  
- **`--soft`**: Moves the commit pointer but keeps changes staged.  
- **`--mixed`** (default): Moves the commit pointer and unstages changes.  
- **`--hard`**: Removes all changes permanently.

---

### **🔹 GitHub-Specific Questions**  

#### **28. What is a Pull Request (PR) in GitHub?**  
A **Pull Request (PR)** is a request to merge changes from one branch to another in a remote repository.

#### **29. How do you fork a repository on GitHub, and why is it useful?**  
- Click the "Fork" button on GitHub to create a personal copy of a repository.  
- Forking allows independent contributions without affecting the original repository.

#### **30. What is GitHub Actions, and how does it help in automation?**  
GitHub Actions is a **CI/CD automation tool** that helps run tests, deploy code, and automate workflows.

---
