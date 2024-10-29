---
icon: file-directory-open-fill
label: Storage Best Practices
description: Where to store you BMD bot project
layout: defualt
categories: [faq]
tags: [faq, project]
expanded: true
visibility: public
---

## Project Storage Best Practices On Windows

### 1. Primary Drive Storage

Store projects on your main internal SSD (e.g., `C:\ Drive`) for improved performance and reliability:
- **SSD Benefits**: Faster read/write speeds, enhanced project load times, and reduced risk of mechanical failure.

### 2. Avoid External Drives

While external drives are convenient, they’re prone to degradation, especially HDDs. Instead:
- Opt for internal SSDs or high-quality USB 3.0 drives if external storage is needed.

### 3. Organized Directory Structure

Create a clear folder hierarchy, like `Documents/BMD_Projects`, to keep projects organized:
- **Example**:
  ```plaintext
  C:\Users\YourName\Documents\BMD_Projects\ProjectName
  ```

### 4. Use Version Control

Integrate Git or other VCS tools to manage versions and avoid redundant copies:
- **Recommendation**: Use platforms like GitHub or Bitbucket for cloud versioning.
Here’s an in-depth guide to setting up and using version control for your project:

Version control tracks changes to your project files, making it easy to manage updates, collaborate, and revert to previous versions. **Git** is a widely used version control system, and **GitHub** provides a remote repository option. Here’s how to set up version control:

#### Step 1: Install Git
1. Download Git from [git-scm.com](https://git-scm.com/) and follow the installation instructions.
2. Configure Git by running the following commands in your terminal:
    ```bash
    git config --global user.name "Your Name"
    git config --global user.email "your-email@example.com"
    ```

#### Step 2: Initialize Git in Your Project Directory
1. Open a terminal in your project folder and initialize Git:
    ```bash
    cd path/to/your/project
    git init
    ```
2. This creates a `.git` folder to track changes.

#### Step 3: Create a Repository on GitHub
1. Go to [GitHub](https://github.com/) and create a new repository for your project.
2. Copy the repository URL for setup.

#### Step 4: Link Your Local Repository to GitHub
1. In your terminal, link your local repository to GitHub:
    ```bash
    git remote add origin <repository-url>
    ```
2. Verify the link with `git remote -v`.

#### Step 5: Commit and Push Changes
1. Add files to the staging area:
    ```bash
    git add .
    ```
2. Commit your changes:
    ```bash
    git commit -m "Initial commit"
    ```
3. Push the changes to GitHub:
    ```bash
    git push -u origin main
    ```

#### Step 6: Managing Changes
- Use `git status` to check modified files.
- To pull updates from GitHub, use `git pull`.
- Make regular commits to track changes and use GitHub’s interface to manage branches and collaborate with others.

### 5. Regular Backups

Automate backups to an external drive or cloud storage to ensure data recovery:
- **Tip**: Schedule weekly or bi-weekly backups.






## Project Storage Best Practices on Linux

### 1. Primary Drive Storage

Store projects on your main internal SSD (e.g., `~/Projects` on `/home`) for fast and reliable performance:
- **SSD Benefits**: Faster read/write speeds, enhanced project load times, and less risk of mechanical failure compared to HDDs.

### 2. Avoid External Drives

While external drives offer flexibility, they degrade faster, especially HDDs. If you need additional storage:
- Opt for an internal SSD or high-quality USB 3.0/SSD external drive.

### 3. Organized Directory Structure

Maintain a well-organized folder hierarchy, like `~/Projects/BMD_Projects`, to simplify navigation:
- **Example**:
  ```plaintext
  /home/YourUsername/Projects/BMD_Projects/ProjectName
  ```

### 4. Use Version Control

Implement Git or another VCS for tracking changes and collaborating. Here’s how to set up Git:

#### Step 1: Install Git
1. Install Git using your package manager:
    ```bash
    sudo apt install git   # Debian/Ubuntu
    sudo dnf install git   # Fedora
    sudo pacman -S git     # Arch
    ```
2. Configure Git:
    ```bash
    git config --global user.name "Your Name"
    git config --global user.email "your-email@example.com"
    ```

#### Step 2: Initialize Git in Your Project Directory
1. Navigate to your project folder and initialize Git:
    ```bash
    cd /home/YourUsername/Projects/ProjectName
    git init
    ```

#### Step 3: Create and Link a GitHub Repository
1. Create a new repository on [GitHub](https://github.com/) and copy the URL.
2. Link the local repository to GitHub:
    ```bash
    git remote add origin <repository-url>
    ```

#### Step 4: Commit and Push Changes
1. Stage your files:
    ```bash
    git add .
    ```
2. Commit the changes:
    ```bash
    git commit -m "Initial commit"
    ```
3. Push to GitHub:
    ```bash
    git push -u origin main
    ```

#### Step 5: Manage Changes
- Check changes with `git status`.
- Pull updates from GitHub with `git pull`.
- Make frequent commits to keep your project history updated.

### 5. Regular Backups

Automate backups to another storage location, such as a secondary internal drive or cloud storage, to ensure project safety:
- **Tip**: Use `rsync` for scheduled backups or services like Dropbox for cloud storage.