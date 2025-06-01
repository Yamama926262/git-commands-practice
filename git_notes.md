# Git Commands Practice

---

## `git init`

This command **initializes a new Git repository** in your current directory. It creates a hidden `.git` folder that tracks all your project's version history.

* **Use Case:** Start tracking changes for a brand-new project that isn't yet under version control.
* **Example Usage:**

    ```bash
    # Navigate to your project folder
    cd my-awesome-project

    # Initialize the Git repository
    git init
    ```

---

## `git clone`

`git clone` **creates a local copy of a remote Git repository**. It downloads all the files, branches, and the complete commit history from a server (like GitHub) to your computer.

* **Use Case:** Get a copy of an existing project that's hosted online so you can start working on it.
* **Example Usage:**

    ```bash
    # Clone a repository from GitHub
    git clone [https://github.com/octocat/Spoon-Knife.git](https://github.com/octocat/Spoon-Knife.git)
    ```

---

## `git status`

This command **shows the current state of your working directory and the staging area**. It tells you which files are modified, staged for commit, or untracked.

* **Use Case:** Quickly see what changes you've made since your last commit and what's ready to be saved.
* **Example Usage:**

    ```bash
    # Check the status of your repository
    git status
    ```

---

## `git add`

`git add` **stages changes for your next commit**. When you modify a file, Git sees it as "modified." This command moves those changes to the "staging area," preparing them to be part of the next snapshot.

* **Use Case:** Selectively include specific modifications in your upcoming commit.
* **Example Usage:**

    ```bash
    # Stage a specific file
    git add index.html

    # Stage all changes in the current directory
    git add .
    ```

---

## `git commit`

The `git commit` command **saves a snapshot of your staged changes to the repository's history**. Each commit is a unique record with a message explaining the changes, and it points back to previous commits.

* **Use Case:** Save the current state of your project after completing a logical unit of work.
* **Example Usage:**

    ```bash
    # Commit staged changes with a descriptive message
    git commit -m "Add initial structure for the website"
    ```

---

## `git push`

`git push` **uploads your local commits to a remote repository**. This makes your changes visible to others and synchronizes your local history with the shared remote version.

* **Use Case:** Share your local commits with your team or update the central repository on platforms like GitHub.
* **Example Usage:**

    ```bash
    # Push your current branch to the 'origin' remote (common name for your main remote)
    git push origin main
    ```

---

## `git pull`

This command **fetches changes from a remote repository and integrates them into your current local branch**. Think of it as a combined `git fetch` (downloading changes) and `git merge` (integrating them).

* **Use Case:** Get the latest updates from the remote repository that your teammates have pushed.
* **Example Usage:**

    ```bash
    # Pull changes from the 'main' branch of the 'origin' remote
    git pull origin main
    ```

---

## `git branch`

`git branch` is used to **manage branches in your repository**. You can use it to list existing branches, create new ones, or delete them.

* **Use Case:** Isolate new features or bug fixes from the main development line, allowing parallel work.
* **Example Usage:**

    ```bash
    # List all local branches
    git branch

    # Create a new branch named 'feature/new-login'
    git branch feature/new-login
    ```

---

## `git checkout`

The `git checkout` command **switches between branches or restores working tree files**. It lets you move between different versions of your project stored in various branches.

* **Use Case:** Switch to a different feature branch, a bugfix branch, or even revert a file to an earlier state.
* **Example Usage:**

    ```bash
    # Switch to an existing branch
    git checkout feature/new-login

    # Switch to a new branch and create it if it doesn't exist (shorthand)
    git checkout -b develop
    ```

---

## `git merge`

`git merge` **integrates changes from one branch into another**. This command combines the commit histories of two branches, often by creating a new "merge commit."

* **Use Case:** Incorporate a completed feature from a separate branch back into your main development branch.
* **Example Usage:**

    ```bash
    # First, switch to the branch you want to merge *into* (e.g., main)
    git checkout main

    # Then, merge the 'feature/new-login' branch into 'main'
    git merge feature/new-login
    ```
