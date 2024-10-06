
# Day 3: Collaboration with Git

## Objectives
By the end of this day, you will have learned how to:
- Work with remote repositories: Understand how to connect your local repository to a remote one to facilitate collaboration.
- Push and pull changes: Learn how to upload your changes to a remote repository and fetch updates made by others.
- Fork repositories and submit pull requests: Understand how to contribute to other projects by forking repositories and submitting your changes for review.

## Activities

### 1. Remote Repositories
Remote repositories are versions of your project hosted on the internet or another network. They allow multiple collaborators to work on the same project from different locations. To add a remote repository:

```bash
git remote add origin https://github.com/username/repository.git
```

This command sets up a connection between your local repository and a remote repository hosted on GitHub (or another platform).

### 2. Pushing and Pulling
Pushing and pulling are essential operations for collaborating with others on a project.

**Push changes to a remote repository:**

```bash
git push origin main
```

This command uploads your local changes in the main branch to the remote repository, allowing others to access your updates.

**Pull changes from a remote repository:**

```bash
git pull origin main
```

This command fetches and integrates changes from the remote main branch into your local branch, ensuring you have the latest updates from other collaborators.

### 3. Forking and Pull Requests
Forking is a way to create a personal copy of someone else's repository on GitHub, allowing you to make changes without affecting the original project. Pull requests are used to propose these changes back to the original repository.

**Fork a repository on GitHub:**
1. Navigate to the repository you want to fork.
2. Click the "Fork" button in the upper right corner of the page.

**Make changes and submit a pull request:**
1. Clone your forked repository locally using `git clone`.
2. Make your desired changes in your local copy.
3. Push the changes back to your forked repository on GitHub using `git push`.
4. Go to the original repository on GitHub and click "New Pull Request" to submit your changes for review.

## Exercises

1. **Fork a repository, make a change, and submit a pull request:**
    - Find a public repository on GitHub that interests you.
    - Fork the repository and clone it locally.
    - Make some meaningful changes or improvements.
    - Push your changes back to your forked repository.
    - Submit a pull request to propose your changes to the original project.
