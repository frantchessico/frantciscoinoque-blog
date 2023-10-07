---
title: All the Git Commands You Need to Know
publishDate: 27 Sep 2023
description: Git is a powerful version control tool that plays a crucial role in modern software development.
---


Git is a powerful version control tool that plays a crucial role in modern software development. Familiarizing yourself with essential Git commands is fundamental to effectively manage your source code and collaborate with other developers. In this guide, we will explore all the Git commands you need to know to become an expert.

## Contents:

### 1.  `git init`

The first step in versioning your project with Git. This command initializes a new Git repository in your directory.

```bash
git init
```

### 2. `git clone`

Use this command to create a local copy of an existing Git repository.

```bash
git clone <repository_URL>
```

### 3. `git add`

Add changes to your upcoming commit. You can specify individual files or use `git add .` to add all modified files.

```bash
git add <file_name>
```

### 4. `git commit`

Record changes in your repository with a descriptive message.

```bash
git commit -m "Commit message"
```

### 5. `git pull`

Update your local repository with changes from the remote repository.

```bash
git pull
```

### 6. `git push`

Send your local changes to the remote repository.

```bash
git push
```

### 7. `git branch`

List all branches in your repository and show the currently checked-out branch.

```bash
git branch
```

### 8. `git checkout`

Switch between branches or create a new branch.

```bash
git checkout <branch_name>
```

### 9. `git merge`

Combine changes from one branch into another.

```bash
git merge <branch_name>
```

### 10. `git log`

 View the commit history of the repository.

 ```bash
 git log
 ```

### 11. `git stash`

 Temporarily stash uncommitted changes.

 ```bash
 git stash
 ```

### 12. `git reset`

 Undo changes in the repository.

 ```bash
 git reset <commit_hash>
 ```

### 13. `git remote`

 List configured remote repositories.

 ```bash
 git remote -v
 ```

### 14. `git fetch`

 Download information from the remote repository but do not automatically merge.

 ```bash
 git fetch
 ```

### 15. `git rebase`

 Rearrange commits for a cleaner timeline.

 ```bash
 git rebase <branch_name>
 ```

### 16. `git tag`

 Mark commits for specific versions of your project.

 ```bash
 git tag <tag_name>
 ```

### 17. `git status`

 Check the current state of your repository, including modified and untracked files.

 ```shell
 git status
 ```

### 18. `git diff`

 Display the differences between files in your working directory and the staging area.

 ```shell
 git diff
 ```

### 19. `git remote add`

 Add a new remote repository to your Git configuration.

 ```shell
 git remote add <remote_name> <remote_URL>
 ```

### 20. `git remote remove`

 Remove a remote repository from your Git configuration.

 ```shell
 git remote remove <remote_name>
 ```

### 21. `git fetch`

 Update remote repository information and download changes but do not automatically merge.

 ```shell
 git fetch
 ```

### 22 `git rebase -i`

 Perform an interactive rebase to rearrange, edit, or merge commits.

 ```shell
 git rebase -i <commit_hash>
 ```

### 23. `git cherry-pick`

 Apply a specific commit from one branch to another.

 ```shell
 git cherry-pick <commit_hash>
 ```

### 24. `git log --graph`

 Visualize the commit history graphically, showing branches.

 ```shell
 git log --graph
 ```

### 25. `git clean`

 Remove untracked files from the working directory.

```shell
 git clean -n # Show files to be removed (dry run mode)
 git clean -f # Remove untracked files (with caution!)
 ```

### 26. `git submodule`

 Manage Git submodules within your main repository.

 ```shell
 git submodule add <submodule_URL> <local_path>
 ```

This guide provides a comprehensive overview of Git commands that are essential for any developer. As you advance in your Git journey, you can explore more advanced commands and branching strategies. However, with these basic commands, you are ready to start effectively managing your source code.

Remember that consistent practice is the key to mastering Git. So, start experimenting with these commands in your own projects and see how they can enhance your efficiency in software development.