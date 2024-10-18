---
icon: commit
label: Uploading & contributing
description: 
layout: defualt
categories: [guide]
tags: [guide]
expanded: true
visibility: public
---
# Uploading Mods via GitHub Pull Requests

To contribute your mods to this repository, you can submit a pull request using either the GitHub web interface or your local machine. Follow the steps below for your preferred method.

## :icon-globe: Using the Web Interface

1. **Fork the Repository**: Click the "Fork" button in the upper-right corner of this repository to create a personal copy in your GitHub account.
2. **Navigate to Your Fork**: Once forked, go to your forked repository on GitHub (it will be at `https://github.com/<your-username>/<repo-name>`).
3. **Create or Edit a File**: 
    - Click on the "Add file" button and choose "Create new file" to add a new mod.
    - To edit an existing file, navigate to it, and click the pencil icon.
4. **Add Your Mod**: Add your mod code to the editor. Make sure it follows any style guidelines or contribution rules for the project.
5. **Commit Your Changes**: Scroll down to the "Commit new file" section:
    - Enter a brief commit message that describes the mod or changes you’ve made.
    - Optionally, provide more details in the extended description.
    - Click "Commit new file" (or "Commit changes" if editing an existing file).
6. **Submit a Pull Request (PR)**:
    - Navigate back to the original repository (not your fork).
    - Click on "New Pull Request".
    - Select the branch from your fork that contains your changes.
    - Add a meaningful description of your mod, explaining its functionality or purpose, then submit the pull request.

## :icon-command-palette: Using Your Local Machine (Git & CLI)

1. **Fork the Repository**: Fork the original repository by clicking "Fork" in the upper-right corner to create a copy under your GitHub account.
2. **Clone Your Fork Locally**: Clone your forked repository to your local machine:
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
   ```
3. **Create a New Branch**: Always create a separate branch for each mod or feature to keep things organized:
   ```bash
   git checkout -b my-new-mod
   ```
4. **Add Your Mod Files**: Place your mod files in the appropriate directories (`Actions`, `Themes`, etc.). Ensure they follow any existing file structure or conventions.
5. **Commit Your Changes**: Once your mod is added, stage and commit the changes:
   ```bash
   git add .
   git commit -m "Add my new mod [describe what the mod does]"
   ```
6. **Push Changes to Your Fork**: Push the new branch to your forked GitHub repository:
   ```bash
   git push origin my-new-mod
   ```
7. **Open a Pull Request (PR)**:
    - Visit the original repository on GitHub.
    - Click "New Pull Request".
    - Select the branch from your fork that contains your mod.
    - Add a detailed description, including what the mod does, why it's useful, and any special instructions for testing or using it. Then submit the PR.

## :icon-pencil: Important Notes
- **Testing**: Be sure to test your mod before submitting it. Ensure it works as expected and doesn’t introduce bugs or issues.
- **Branch Naming**: When creating a new branch, use a descriptive name that relates to the mod or feature, such as `add-action-mod` or `fix-theme-mod`.
- **Contributing Guidelines**: If this repository has a `CONTRIBUTING.md` file, make sure to read and follow it before submitting your pull request.

## :icon-repo: Useful Resources

Here are some helpful resources to assist you in contributing to this repository:

- **[Markdown Guide](https://www.markdownguide.org/)**: A comprehensive guide to Markdown, a lightweight markup language for formatting text. Learn how to structure your README files, documentation, and more.
- **[GitHub Octicons](https://primer.github.io/octicons/)**: GitHub's official icon set, commonly used across GitHub projects. Use these icons to enhance your repository's visual appeal.
- **[Retype Octicons](https://retype.com/components/octicons/#icon-list)**: A collection of GitHub Octicons that can be easily integrated into Retype-powered documentation, perfect for adding icons to enhance your documentation pages.
- **[GitHub Docs](https://docs.github.com/)**: The official GitHub documentation. Learn about GitHub features, commands, workflows, and tips for managing repositories, handling pull requests, and more.
- **[Pro Git Book](https://git-scm.com/book/en/v2)**: A free online book that covers everything you need to know about Git, from the basics to advanced topics like branching and Git workflows.
- **[GitHub Flow](https://docs.github.com/en/get-started/quickstart/github-flow)**: An explanation of the GitHub Flow, a lightweight, branch-based workflow that supports teams and projects in version control.
- **[Semantic Commit Messages](https://gist.github.com/joshbuchea/01f9d4aa31638a2b95b8)**: A guide to writing clear and concise commit messages using semantic conventions, which helps maintain an organized commit history.
- **[Learn Git Branching](https://learngitbranching.js.org/)**: An interactive Git learning game that helps you practice and understand Git branching, merging, and rebasing.
- **[GitHub CLI](https://cli.github.com/)**: GitHub’s command-line tool for managing pull requests, issues, and repositories directly from your terminal.

These resources will help you with everything from mastering Markdown to understanding Git workflows, writing better commit messages, and effectively using GitHub tools.

## Template page
[!ref](template.md)
+++ Code
:::code source="template.md" :::
+++ demo
## Welcome to the Template Page

This is a sample template page. You can use this as a starting point for creating new pages in your project.

### Table of Contents
- [Introduction](#introduction)
- [Usage](#usage)
- [Examples](#examples)
- [Conclusion](#conclusion)

### Introduction
Provide an introduction to the template page here. Explain the purpose and any relevant background information.

### Usage
Describe how to use this template. Include any necessary steps or instructions.

### Examples
Provide examples of how this template can be used. Include code snippets or screenshots if applicable.

### Conclusion
Summarize the key points of the template page. Include any final thoughts or recommendations.

Feel free to customize this template to fit your needs.

+++