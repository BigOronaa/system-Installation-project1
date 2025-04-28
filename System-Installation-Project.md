## Answer to my project.
# System Installation Project 

This document covers the installation steps for the development environment tools required for the project (using WindowsPowerShell).

---

## 1. Git Installation 

- Download Git for Windows from the [official site](https://git-scm.com/).
- Run the installer and accept default settings.
- After installation, open PowerShell and verify Git:

```powershell
git --version

# Visual Studio Code Installation and Setup Guide (PowerShell)

This guide details how to install and configure Visual Studio Code (VS Code) for development using PowerShell.

---

## 1. Download and Install VS Code

- Visit the official Visual Studio Code website: [https://code.visualstudio.com/](https://code.visualstudio.com/)
- Download the appropriate installer for your operating system (Windows, macOS, or Linux).
- Run the installer and follow the setup wizard.
- Accept the default installation options for simplicity.
- After installation, VS Code should be available in your system's PATH.

---

## 2. Verify VS Code Installation

Open PowerShell and run:

```powershell
code --version

# SSH and SSH-Agent Setup 

This guide details how to install and configure SSH along with the SSH-Agent for GitHub access using PowerShell.

---
# Installing Extensions in Visual Studio Code
## 1. Open Extensions View

To begin installing extensions:

- Open VS Code.
- Click on the **Extensions** icon in the Activity Bar on the side of the window
## 2. Search for Extensions

- In the Extensions view, you’ll see a search bar at the top.
- Type the name of the extension you want to install (e.g., "GitLens", "Prettier", "Python", etc.).
- Extensions will appear in the search results.
## 3. Install an Extension

- Click on the **Install** button next to the extension you want to add.
- The extension will be automatically installed and ready for use.

## 1. Verify SSH Installation


1. Go to **Settings** → **Apps** → **Optional Features**
2. Look for **OpenSSH Client**. If not installed, click on **Add a feature** → **OpenSSH Client** → Install.

Verify SSH is installed by running:

```powershell
ssh -V

# SSH Agent Setup 

---

## 1. Check if SSH is Installed

```powershell
ssh -V
ssh-keygen -t rsa ed25519 "edwardoronaa@gmail.com" 
Press Enter to accept the default file location for your SSH key. You can also add a passphrase (optional) or leave it empty.

Next, start the SSH-Agent to manage your SSH keys. Run the following in PowerShell:
Get-Service ssh-agent | Set-Service -StartupType Automatic
Start-Service ssh-agent
After the SSH-Agent is started, add your private SSH key to the agent:
ssh-add $env:USERPROFILE\.ssh\id_rsa

Verify SSH-Agent is Running
ssh-add -L

# GitHub Account Creation Guide

This guide walks through the process of creating a GitHub account.
## 1. Visit GitHub Website

Go to the GitHub website: [https://github.com](https://github.com/)

---

## 2. Sign Up

Click on the **Sign up** button and fill in the following details:

- **Username**: Choose a unique username.
- **Email**: Provide a valid email address.
- **Password**: Choose a strong password.
- **Verification**: Complete any CAPTCHA if prompted.

---

## 3. Verify Your Email

GitHub will send a verification email to the address you provided.  
Click on the verification link to activate your account.
 Adding SSH Key to GitHub

This guide shows how to add your SSH key to your GitHub account for authentication.

---

## 1. Copy Your SSH Public Key

Run the following command in PowerShell to display your public SSH key:

```powershell
Get-Content $env:USERPROFILE\.ssh\id_rsa.pub 

