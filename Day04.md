
# Day 4: Advanced Git Concepts

## Objectives

By the end of this day, you will have learned about advanced Git concepts, including:

- **Rebasing and cherry-picking**: Understand how to rebase branches and cherry-pick specific commits to manage your repository history more effectively.
- **Stashing changes**: Learn how to temporarily stash changes and reapply them later, allowing for more flexible workflow management.
- **Git tags and releases**: Understand how to create and manage tags and releases in Git, which are crucial for versioning and tracking milestones in your project.

## Activities

### 1. Rebasing

Rebasing is a powerful tool in Git that allows you to move or combine a sequence of commits to a new base commit. It's useful for maintaining a clean and linear commit history.

#### Steps:

1. **Switch to the branch you want to rebase:**

    ```bash
    git checkout feature-branch
    ```

2. **Rebase your branch onto another branch (e.g., main):**

    ```bash
    git rebase main
    ```

This command replays the commits in `feature-branch` on top of the `main` branch, creating a linear history.

**When to Use Rebasing:**

- To keep a clean, linear commit history.
- When you want to incorporate changes from another branch before merging.

### 2. Cherry-Picking

Cherry-picking allows you to apply changes from specific commits on one branch to another branch. It's useful when you want to include certain changes without merging an entire branch.

#### Steps:

1. **Identify the commit hash you want to cherry-pick:**

    ```bash
    git log
    ```

Find the commit hash (a long string of numbers and letters) of the commit you want to cherry-pick.

2. **Cherry-pick the commit:**

    ```bash
    git cherry-pick <commit-hash>
    ```

This command applies the changes from the specified commit to your current branch.

**When to Use Cherry-Picking:**

- To apply specific bug fixes or features from one branch to another without merging all changes.
- To backport changes to previous versions of your code.

### 3. Stashing

Stashing allows you to save your changes temporarily without committing them. It's useful when you need to switch branches or pull in updates without committing unfinished work.

#### Steps:

1. **Stash your changes:**

    ```bash
    git stash
    ```

This command saves your changes and reverts your working directory to the last commit.

2. **Apply your stashed changes:**

    ```bash
    git stash apply
    ```

This command reapplies the stashed changes to your working directory.

**When to Use Stashing:**

- To save your work in progress when you need to switch branches.
- To pull in updates from the remote repository without committing unfinished changes.

### 4. Tags and Releases

Tags are used to mark specific points in your repository’s history, such as releases. They are often used to indicate versions.

#### Steps:

1. **Create a tag:**

    ```bash
    git tag -a v1.0 -m "Version 1.0"
    ```

This command creates an annotated tag `v1.0` with a message.

2. **Push the tag to the remote repository:**

    ```bash
    git push origin v1.0
    ```

This command pushes the tag to the remote repository.

**When to Use Tags:**

- To mark release points (e.g., v1.0, v2.0).
- To indicate significant milestones in the project history.

## Exercises

1. **Rebase a Feature Branch onto the Main Branch**

    - Create a new branch and add some commits.
    - Switch to the main branch and add some commits.
    - Rebase your feature branch onto the main branch:

        ```bash
        git rebase main
        ```

2. **Cherry-Pick a Commit from One Branch to Another**

    - Identify the commit you want to cherry-pick using `git log`.
    - Switch to the target branch.
    - Cherry-pick the commit:

        ```bash
        git cherry-pick <commit-hash>
        ```

3. **Stash Changes and Reapply Them Later**

    - Make some changes to your working directory.
    - Stash the changes:

        ```bash
        git stash
        ```

    - Switch to another branch or pull updates.
    - Reapply the stashed changes:

        ```bash
        git stash apply
        ```

4. **Create a Tag and Push It to the Remote Repository**

    - Create a tag for your current commit:

        ```bash
        git tag -a v1.0 -m "Version 1.0"
        ```

    - Push the tag to the remote repository:

        ```bash
        git push origin v1.0
        ```

By the end of these exercises, you should have a solid understanding of how to rebase branches, cherry-pick commits, stash changes, and manage tags and releases in Git.
