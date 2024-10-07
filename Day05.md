# Day 5: Putting It All Together

## Objectives

By the end of this day, you will have applied your Git knowledge to sample projects and worked on real-world scenarios, including:

- **Creating repositories**: Understand how to set up repositories for personal and collaborative projects.
- **Working with branches**: Learn to create, switch, and merge branches effectively.
- **Collaborating with others**: Practice resolving conflicts and using pull requests for team collaboration.

## Activities

### 1. Sample Project 1: Personal Portfolio Website

In this project, you will create a personal portfolio website and manage its development using Git.

#### Steps:

1. **Create a repository for your portfolio website:**

    ```bash
    git init my-portfolio
    cd my-portfolio
    ```

2. **Set up branches for features like homepage, about, contact:**

    - Create a branch for the homepage:

      ```bash
      git checkout -b homepage
      ```

    - Create a branch for the about page:

      ```bash
      git checkout -b about
      ```

    - Create a branch for the contact page:

      ```bash
      git checkout -b contact
      ```

3. **Merge branches and resolve conflicts:**

    - Merge the homepage branch into the main branch:

      ```bash
      git checkout main
      git merge homepage
      ```

    - If there are conflicts, Git will prompt you to resolve them. Open the conflicting files, make the necessary changes, and then continue the merge:

      ```bash
      git add .
      git commit -m "Resolve merge conflicts"
      ```

4. **Push the repository to GitHub:**

    - Create a remote repository on GitHub.
    - Add the remote repository and push your local repository to GitHub:

      ```bash
      git remote add origin https://github.com/username/my-portfolio.git
      git push -u origin main
      ```

### 2. Sample Project 2: Collaborative Project

In this project, you will collaborate on a team project, practicing branch management, conflict resolution, and pull requests.

#### Steps:

1. **Clone a team project repository:**

    ```bash
    git clone https://github.com/team/project.git
    cd project
    ```

2. **Create and switch to feature branches:**

    - Create a new branch for a feature:

      ```bash
      git checkout -b feature-branch
      ```

3. **Commit and push changes:**

    - Make changes and commit them:

      ```bash
      git add .
      git commit -m "Add new feature"
      ```

    - Push the changes to the remote repository:

      ```bash
      git push origin feature-branch
      ```

4. **Resolve conflicts and submit pull requests:**

    - If there are conflicts, resolve them as you did in the personal project.
    - Submit a pull request to merge your changes into the main branch. Go to the repository on GitHub, select your branch, and click "New Pull Request".

5. **Review and merge pull requests from team members:**

    - Review pull requests submitted by team members.
    - If everything looks good, merge the pull requests into the main branch.

## Exercises

1. **Create a repository for a personal project:**
    - Choose a small project (e.g., a simple web app or script).
    - Create a repository for the project.
    - Set up branches for different features.
    - Commit and push your changes to GitHub.

2. **Collaborate with a friend on a small project:**
    - Choose a small project to work on with a friend.
    - Set up a repository and invite your friend to collaborate.
    - Utilize branches, merging, and pull requests to manage your work.
