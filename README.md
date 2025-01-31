# Github-Workshop

:shipit:: *Aye tuts*, cmon here... join me for this Github Workshop wontcha

:shipit:: Youze can call me Lorenzo, and today I'll be showing you the ropes for **Git/GitHub**... please join us... *unless your a fraidy-cat?*

![cool cats](https://private-user-images.githubusercontent.com/74038190/240820725-a754eac4-5a8b-4e8f-922b-aff555400790.gif?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzgzNDY2NjIsIm5iZiI6MTczODM0NjM2MiwicGF0aCI6Ii83NDAzODE5MC8yNDA4MjA3MjUtYTc1NGVhYzQtNWE4Yi00ZThmLTkyMmItYWZmNTU1NDAwNzkwLmdpZj9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTAxMzElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwMTMxVDE3NTkyMlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTk3ZmNiOWQ1NjJhNTlkZjQ1ZjE3Nzc0ZGJkYmUyODg5NjUzYWU1ODVkOTgyY2U4OGE1MzAyNjdjY2Q2NmJlODgmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.uBBbwEGNcAqe0HQtrvfETca-ShcjiQFNxjjzvWQkD-o)


## Agenda
1. Setting up a GitHub Account
2. Installing Git (if needed)
3. Basic Git Commands (Working locally)
4. HTML vs. SSH Approaches
5. HTML Setup
6. SSH Setup
7. Playing with Remote Repos

## Prerequisites
- A **GitHub** account ([Sign up here](https://github.com/))
- Ensure Git is installed on your machine ([Download here](https://git-scm.com/))
- A code editor (e.g., **VS Code**, **Notepad++**, **Sublime Text**, etc)

## Getting Started

### Step 1: Setting Up a GitHub Account
1. Go to [GitHub](https://github.com/) and sign up for an account.
2. Verify your email and set up your profile.

### Step 2: Installing Git
1. Check if Git is installed:
   ```bash
   git --version
   ```
2. If Git is not installed, download and install it from [git-scm.com](https://git-scm.com/).

### Step 3: Basic Git Commands (Local Repository Management)
Before working with **GitHub**, it's essential to understand how **Git** works locally.

1. Initialize a new Git repository:
   ```bash
   git init my-project
   cd my-project
   ```
2. Create a new file:
   ```bash
   echo "Hello, Git!" > file.txt
   ```
3. Check repository status:
   ```bash
   git status
   ```
4. Add changes to the staging area:
   ```bash
   git add file.txt
   ```
5. Commit changes:
   ```bash
   git commit -m "Initial commit"
   ```
6. View commit history:
   ```bash
   git log
   ```

### Step 4: Understanding HTML vs. SSH Approaches
GitHub allows you to interact with repositories using different authentication methods: **HTTPS** and **SSH**.

#### HTML Approach (HTTPS Clone Method):
- **Pros:**
  - Simple to set up and use.
  - Works on any network without additional configuration.
  - Great for beginners.
- **Cons:**
  - Requires entering credentials (or a personal access token) for each `push`.
  - May have authentication issues if multi-factor authentication (MFA) is enabled.

#### SSH Approach:
- **Pros:**
  - Much more secure authentication method.
  - No need to enter credentials repeatedly.
  - Ideal for frequent Git users who interact with repositories regularly.
- **Cons:**
  - Requires additional setup (generating and adding SSH keys).

Choose one approach when working with a repository, not both.

### Step 5: HTML Setup
1. Clone this repository using HTTPS:
   ```bash
   git clone https://github.com/lorenzom222/Github-Workshop.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Github-Workshop
   ```
3. Add a simple HTML file:
   ```bash
   echo "<h1>Hello, GitHub!</h1>" > index.html
   ```
4. Add and commit changes:
   ```bash
   git add index.html
   git commit -m "Added simple HTML file"
   ```
5. Push changes to GitHub:
   ```bash
   git push origin main
   ```

### Step 6: Setting Up SSH
1. Generate an SSH key (if not already set up):
   ```bash
   ssh-keygen -t rsa -b 4096 -C "your-email@example.com"
   ```
2. Add the SSH key to GitHub ([Guide](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)).
3. Clone the repository using SSH:
   ```bash
   git clone git@github.com:your-username/Github-Workshop.git
   ```
4. Navigate to the project directory:
   ```bash
   cd Github-Workshop
   ```
5. Add a simple HTML file and commit:
   ```bash
   echo "<h1>Hello, GitHub over SSH!</h1>" > index.html
   git add index.html
   git commit -m "Added HTML file using SSH"
   ```
6. Push changes to GitHub:
   ```bash
   git push origin main
   ```

### Step 7: Working with Remote Repositories
Once you've set up your local repository, you can interact with remote repositories on GitHub.

1. Link a local repository to a remote repository:
   ```bash
   git remote add origin https://github.com/your-username/Github-Workshop.git
   ```
2. Push local changes to GitHub:
   ```bash
   git push -u origin main
   ```
3. Pull the latest changes from GitHub:
   ```bash
   git pull origin main
   ```

## Resources
- [GitHub Docs](https://docs.github.com/)
- [Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf)
- [Pro Git Book](https://git-scm.com/book/en/v2)

---

And that’s a wrap, folks! I'm out...

![penguin walking away](https://user-images.githubusercontent.com/74038190/213911167-6bc9ef46-2950-481c-a03c-189f9506083b.gif)
