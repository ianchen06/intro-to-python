# Intro to Git

This section will introduce you to Git, a version control system that allows you to track changes to files over time. It is a distributed version control system, which means that it stores a full copy of the repository on each developer's computer. This allows developers to work on the same project simultaneously without needing to be connected to a central server.

## Important Concepts

- Git is only used for text files, not binary files.
- Review the files before committing them to the repository.
  - Don't include any sensitive information in the repository.
  - Don't include any large files in the repository. (e.g., images, videos, etc.)
- When you are not sure about the outcome of a git command, copy the repository to a different location and experiment with it there.

## Common Git Commands

### Creating a Repository

1. `git init` - Initialize a new Git repository in the current directory.
2. `git clone <url>` - Clone an existing Git repository from a remote server.
3. `git remote add <name> <url>` - Add a new remote server to the repository.

### Making Changes

1. `git status` - Display the current status of the repository.
2. `git add <file>` - Add a file to the staging area.
3. `git commit -m <message>` - Commit staged changes to the repository.
4. `git push <remote> <branch>` - Push local commits to a remote server.

### Branching

1. `git branch` - List all branches in the repository.
2. `git branch <name>` - Create a new branch.
3. `git checkout <name>` - Switch to a different branch.
4. `git merge <name>` - Merge a branch into the current branch.
5. `git branch -d <name>` - Delete a branch.

### Viewing History

1. `git log` - Display the commit history of the repository.
2. `git diff <commit> <commit>` - Show the differences between two commits.
3. `git show <commit>` - Show the changes introduced by a commit.

### Undoing Changes

1. `git reset <file>` - Unstage a file.
2. `git checkout -- <file>` - Discard changes to a file.
3. `git revert <commit>` - Revert a commit.
4. `git reset --hard <commit>` - Reset the repository to a previous commit.

### Miscellaneous

1. `git config` - Configure Git settings.
2. `git help` - Display help information about Git.

## Git Workflow

### 1. Create a Repository

1. Create a new directory for your project.
2. Initialize a new Git repository in the directory using `git init`.
3. Create a new file called `README.md` and add some content to it.
4. Add the file to the staging area using `git add`.
5. Commit the changes to the repository using `git commit`.
6. Create a new repository on GitHub.
7. Add the remote repository to your local repository using `git remote add`.
8. Push the changes to the remote repository using `git push`.
9. View the repository on GitHub.

### 2. Making Changes

10. Create a new branch called `feature` using `git branch`.
11. Switch to the `feature` branch using `git checkout`.
12. Make some changes to the `README.md` file.
13. Commit the changes to the `feature` branch.
14. Push the changes to the remote repository.
15. View the repository on GitHub.

### 3. Merging Changes

16. Create a pull request to merge the `feature` branch into the `main` branch.
17. Ask someone to review your pull request.
18. Merge the pull request.
19. Delete the `feature` branch.
20. Pull the changes from the remote repository using `git pull`.
21. View the repository on GitHub.

## Practice Exercises

1. Create a new directory called "my-project" and initialize a new Git repository in it.
2. Create a new file called "README.md" and add some content to it.
3. Add the file to the staging area and commit the changes to the repository.
4. Create a new repository on GitHub and add the remote repository to your local repository.
5. Push the changes to the remote repository and view the repository on GitHub.
6. Create a new branch called "feature" and switch to it.
7. Make some changes to the "README.md" file and commit the changes to the "feature" branch.
8. Push the changes to the remote repository and view the repository on GitHub.
9. Create a pull request to merge the "feature" branch into the "main" branch.
10. Merge the pull request and delete the "feature" branch.
11. Pull the changes from the remote repository and view the repository on GitHub.

## Additional Resources

- [Git Documentation](https://git-scm.com/doc)
- [Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf)
- [Git Tutorial](https://www.atlassian.com/git/tutorials)
- [Git Handbook](https://guides.github.com/introduction/git-handbook/)
- [Git Best Practices](https://www.git-tower.com/learn/git/ebook/en/command-line/appendix/best-practices)
- [Git Workflows](https://www.atlassian.com/git/tutorials/comparing-workflows)

