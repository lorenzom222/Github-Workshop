# Github-Workshop

:shipit:: Hellloooooooo and welcome to my **Github/Git** Workshop!

:shipit:: My name is Lorenzo, and today I'll be showing you the ropes for the for very very basic of git so you can be cool. Please join us... *unless your a fraidy-cat?*

![cool cats](https://c.tenor.com/muDKReI2icIAAAAd/tenor.gif)





## Agenda
1. WTF is Git & GitHub... aren't they the same thing???
   > :shipit: No, you idiot—version control!
2. Getting youze guys situated on GitHub
3. Installing Git ~~(if needed... but it's 2025)~~ IMPORTANT FOR WINDOWS USERS
4. Babie Git Commands (Working locally)
5. HTML vs. SSH Approaches
   > :shipit:: More importantly why SSH is superior
6. HTML Setup
7. SSH Setup
8. Playing with Remote Repos



## What is Git? 🌲
- Git is a version control system.
- Make creates repositories (repos), which are like folders that contain your project and track its changes.
- Repos = Containers that store all your code and its history of changes
- Basically, if someone changes a file (like opens a document and writes stuff in it -- like poop -- changes a line of code, or so on) it records the differences between the new version and the old version, and maintains a history.
- You can also do things like branching for collabing with folks, which allows for friends to work on the same thing without interfering with one another.
- Then subsequently merge each branch changes together into a single version at the end of the day.
   > :shipit:: I like to think of it as an awesome tree, where the main code is the trunk and the branches are different experimental versions.
   > Each branch can grow on it's, but they can be merged back together to form a big stick... tree dont really do that tho...

 
### Git 🌲 vs. GitHub 🐙: How Are They Related?
GitHub is an online service that **hosts your repositories** and makes collaboration easy.
- **GitHub** = Website to host your repos (trees) for version control. Like a forest of trees.
- **Git** = Command-line software handling version control on your local machine.
- **GitHub uses Git** behind the scenes—think of Git as the engine and GitHub as the fancy dashboard.


## WHAT YOU NEED BEFORE 🛑
- A computer that works... duh
- Know how to open your terminal... or powershell if your on windows ig
- A code editor (e.g., **VS Code**, **Notepad++**, **Sublime Text**, **Wattpad??**)
   > :shipit:: I like me sum VS Code... but if ur into souls-like... try sum Vim hehehehehe
- _Optional_: A couple of brain cells
   > :shipit:: ... cmon who are we kidding

## Let's gooooo :octocat::

### Step 1: Setting Up a GitHub Account
1. Go to [GitHub](https://github.com/) and sign up for an account.
2. Verify your email and set up your profile.
   > :shipit:: Make a cool username to really mog on other programmers 🦾

### Step 2: Installing Git
1. Check if Git is installed:
   ```bash
   git --version
   ```
2. Windows doesn't come preinstall with git. So, download and install it from [git-scm.com](https://git-scm.com/).
   1. Also need to figure out Xcode for mac in order to use Git.


### Step 3: Basic Git Commands (Local Repository Management)
Before working with **GitHub**, it's essential to understand how **Git** works locally. These step-by-step instructions will help you manage your repository on **macOS, Linux, and Windows**.

---

### First: Initialize a New Git Repository
This creates a new Git repository in a specified folder.

#### macOS & Linux:
1. Open the terminal.
2. Create a new folder and navigate into it:
   ```bash
   mkdir my-awesome-project && cd my-awesome-project
   ```
3. Initialize Git:
   ```bash
   git init
   ```

#### Windows (PowerShell):
1. Open PowerShell.
2. Create a new folder and navigate into it:
   ```powershell
   mkdir my-awesome-project; cd my-awesome-project
   ```
3. Initialize Git:
   ```powershell
   git init
   ```

> :shipit: Now your project is a Git repository!

---

### Second: Create a New File and Add Content
Git needs files to track changes. Let’s create a simple file.

#### macOS & Linux:
1. Open the terminal.
2. Run this command to create and open a file in a text editor:
   ```bash
   nano hello.py
   ```
3. Type the following text inside the editor:
   ```python
   print('Hello, world!')
   ```
4. Save the file by pressing **CTRL + X**, then **Y**, and hit **Enter**.

#### Windows (PowerShell):
1. Open PowerShell.
2. Run this command to create and open a file in Notepad:
   ```powershell
   notepad hello.py
   ```
3. Type the following text inside Notepad:
   ```python
   print('Hello, world!')
   ```
4. Save the file and close Notepad.


---

### Third : Check Repository Status
Before committing changes, check what has been modified.

1. Run:
   ```bash
   git status
   ```

> :eyes: See what’s changed before committing!

---

### Fourth: Add Changes to the Staging Area
This prepares files for commit.

1. To add a specific file:
   ```bash
   git add hello.py
   ```
2. To add all files:
   ```bash
   git add .
   ```

> :file_folder: Staging prepares your files for commit!

---

### Fifth: Commit Changes
A commit saves a snapshot of your project.

1. Run:
   ```bash
   git commit -m "Initial commit: Added hello.py"
   ```

> :shipit: Think of commits as save points in a video game.

---

### Sixth: View Commit History
See a log of previous commits.

1. Run:
   ```bash
   git log
   ```
2. To see a short version:
   ```bash
   git log --oneline
   ```

> :scroll: Keep track of your project history!

---

Now you have a Git repository with a tracked file, and you know the basics of version control!



### Step 4: Understanding HTML vs. SSH Approaches
GitHub allows you to interact with repositories using different authentication methods: **HTTPS** and **SSH**.

#### HTML Approach (HTTPS Clone Method):
- **Pros:**
  - Simple to set up and use.
  - Works on any network without additional configuration.
  - Great for beginners.
- **Cons:**
  - ~~Requires entering credentials (or a personal access token) for each `push`.~~
  - You **NEED** personal access token for each `push`
     - *No more login because insecure???*
  - May have authentication issues if multi-factor authentication (MFA) is enabled.

#### SSH Approach:
- **Pros:**
  - Much more secure authentication method.
  - No need to enter credentials repeatedly.
  - Ideal for frequent Git users who interact with repositories regularly.
- **Cons:**
  - Requires additional setup (generating and adding SSH keys).
     > :shipit:: But since we are grown up big physicist, we are going to do this...

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
   git clone git@github.com:lorenzom222/Github-Workshop.git
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
