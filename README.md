# A Collaborative Git Learning Resource for Beginners

Topic
<ol type = "1">
   <li>Objective</li>
   <li>Background</li>
   <li>What is Git?</li>
   <li>How to install Git?</li>
   <li>Configure Git Settings</li>
   <li>Getting Help</li>
</ol>

# Objective
The aim of this report is to establish a collaborative Git learning resource that supports beginners in understanding and applying fundamental Git concepts effectively

---

# Background
Git is an essential open source version control system widely used in modern software development. While many learning resources are available, they are often scattered or focused on specific scenarios. This initiative is intended to provide a centralised and structured guide that simplifies the learning process and encourages knowledge sharing among contributors

---

> Learning Notes:
>
> Many of the author’s existing GitHub repositories already include Git-related guidelines tailored to specific use cases for practice. However, this repository aims to consolidate and expand those materials into a dedicated learning resource focused entirely on Git. Contributions are encouraged to continuously improve the content and share best practices with the community
>
> For Windows users, it is recommended to set up a Windows Subsystem for Linux (WSL) environment. All guidelines in this repository are designed to be used in a Linux-based environment, primarily through the Command Line Interface (CLI). This approach allows users to learn each module while becoming familiar with CLI usage
>
> Developing proficiency with the CLI will help align your skills with real-world working environments, where command-line tools are commonly used to improve productivity and ensure accuracy in daily tasks

## What is Git?
Git is a distributed version control system used to track changes in source code during software development. It allows developers to manage, record, and collaborate on code efficiently by maintaining a complete history of changes. With Git, multiple users can work on the same project simultaneously without overwriting each other’s work, ensuring better collaboration and version tracking

### Use Cases of Git
- Tracking changes in code and documents
- Collaborating with team members on projects
- Managing different versions or features using branches
- Rolling back to previous versions if issues occur
- Maintaining a clear history of project development

---

## How to install Git?
In this guide, we will focus on installing Git in a Linux Ubuntu environment or Windows Subsystem for Linux (WSL). This approach is aligned with real-world working environments, where most developers use Linux-based systems.
The Command Line Interface (CLI) provides more flexibility, advanced features, and greater control compared to graphical user interfaces (GUI), which can be more limited. Learning Git through the CLI not only improves your understanding but also prepares you to work more efficiently and effectively in professional development environments.

### For Windows user
<ol type="1">
    <li>Go to the official website:  https://git-scm.com/download/win</li>
    <li>Download the .exe file and run the installation</li>
    <li>After installation complete, run Git Bash</li>
</ol>

### For Linux Ubuntu or WSL
```bash
# 1. Check the current Git version
git --version       # Output: git version 2.x.x

# 2. Highly recommended to use latets version
sudo apt update             # update the envinronment
sudo apt install git -y     # update latest Git version
```

### For Mac user
```bash
# 1. Open terminal and check current Git Version
git --version       # Output: git version 2.x.x

# 2. Update Git version
# Go to Go to the official website:  https://git-scm.com/download/mac
# Open the .dmg file
# Run the Installer
# Or you can explore the CLI installation with brew
```

## Configure Git Settings
Default Sttings:
1. Name
2. Email
3. Line Ending

```bash
# 1. In Linux or WSL, it is recommended to work in your local user directory, as this is the common location for storing projects and helps build good development habits
cd /home/<username>

# 2. Add Username
git config --global user.name "<your username>" 

# 3. Add Email
git config --global user.name myemail@domain.com

# 4. Verify the settins
git config --global --list

# Output:
user.name=xxxxxxx
user.email=xxxxxx
```

5. Configure Line Ending
Configuring end-of-line settings is important but often overlooked, as it helps prevent inconsistencies and issues when working across different operating systems

```bash
# For Windows
git config --global core.autocrlf true

# or Mac or Linux
git config --global core.autocrlf input
```

## Getting Help
You can get more information about the Git Commands
1. Full Documemntation for Git: git-scm.com/docs
2. The Git Cheat Sheet: https://git-scm.com/cheat-sheet
3. In the terminal
```bash
# Get help
git --help

# To find help for a specific command, e.g.: git config
# For full documentation
git confif --help       # press "space" button for next page or 'q' button to quite the documentation

# or get help with summary
got config -h
```
