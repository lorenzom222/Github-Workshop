# Github-Workshop

:shipit:: *Aye tuts*, cmon here... join me for this Github Workshop wontcha

:shipit:: Youze can call me Lorenzo, and today I'll be showing you the ropes for **Git/GitHub**... please join us... *unless your a fraidy-cat?*

![cool cats](https://c.tenor.com/muDKReI2icIAAAAd/tenor.gif)





## Agenda
1. WTF is Git & GitHub... aren't they the same thing???
   > :shipit: No, you idiot—version control!
2. Getting youze guys situated on GitHub
3. Installing Git (if needed... but it's 2025)
4. Babie Git Commands (Working locally)
5. HTML vs. SSH Approaches > More importantly why SSH is superior
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


## WHAT YOU NEED BEFORE
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
2. If for whatever godforsaken reason Git is not installed, get a new laptop or download and install it from [git-scm.com](https://git-scm.com/).

![No Git](https://c.tenor.com/b4RoQd-nV94AAAAC/tenor.gif)

### Step 3: Basic Git Commands (Local Repository Management)
Before working with **GitHub**, it's essential to understand how **Git** works locally.

1. Initialize a new Git repository:
   ```bash
   git init my-super-awesome-cool-project
   cd my-super-awesome-cool-project
   ```
   or just
   ```bash
   cd my-other-super-awesome-cool-project
   git init
   ```
   > :shipit: Innit bruv! 🤌
3. Create a new file in that folder and put some stuff innit, for example:
   ```bash
   echo "Hello freaks and geeks!" > yuh.py
   ```
4. Check repository status:
   ```bash
   git status
   ```
5. Add changes to the staging area:
   ```bash
   git add yuh.py
   ```
6. COMMIT changes:
   ```bash
   git commit -m "top of the morning"
   ```
   > :shipit:: dont be afraid of commitment, you can always go back
7. View commit history:
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
