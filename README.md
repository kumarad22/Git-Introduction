
# 📘 Git Introduction

This repository contains a list of essential Git commands and a step-by-step guide on how to push a local repository to GitHub.

---

## 🚀 How to Push a Local Repository to GitHub

Follow the steps below to initialize Git locally, set up the remote connection, and push your code to GitHub.

---

### ✅ 1. Set Up SSH (Recommended)

- Generate an SSH key using:
  ```bash
  ssh-keygen -t ed25519 -C "your-email@example.com"
  ```
- Copy the contents of the public key file (e.g., `~/.ssh/id_ed25519.pub`)
- Go to your GitHub **Settings → SSH and GPG Keys**
- Click **"New SSH key"** and paste the key

> Alternatively, you can use HTTPS if you prefer not to use SSH

---

### ✅ 2. Create a New Repository on GitHub

- Go to: [https://github.com/new](https://github.com/new)
- Choose a repository name
- **Do not check "Initialize with README"** (to avoid conflicts)
- Click **"Create repository"**

---

### ✅ 3. Initialize Git Locally

In your project directory, open Git Bash and run:

```bash
git init
```

---

### ✅ 4. Add and Commit Files

```bash
git add .
git commit -m "Initial commit"
```

If you have a README and want to add it first to avoid merge conflicts:

```bash
git add README.md
git commit -m "Add README"
```

---

### ✅ 5. Rename the Default Branch (if needed)

GitHub uses `main` by default. Rename your local branch to match:

```bash
git branch -m main
```

---

### ✅ 6. Add the Remote Repository

Use either HTTPS or SSH:

```bash
# HTTPS
git remote add origin https://github.com/your-username/your-repo-name.git

# OR SSH
git remote add origin git@github.com:your-username/your-repo-name.git
```

---

### ✅ 7. Push to GitHub

```bash
git push -u origin main
```

---

## ✅ Done!

Your local project is now successfully pushed to GitHub. You can continue development, and use the following Git commands for future work:

---

## 🛠️ Common Git Commands

```bash
git status             # Show modified/staged files
git add <file>         # Stage a specific file
git commit -m "msg"    # Commit staged files
git push               # Push commits to GitHub
git pull               # Pull remote changes
```

---

## 📌 Tips

- Create a `.gitignore` file to prevent tracking unwanted files
- Use `git log` to view commit history
- Use `git diff` to see what's changed

---

## 🧠 Useful Resources

- GitHub Docs: https://docs.github.com/en/get-started
- Git Handbook: https://guides.github.com/introduction/git-handbook/
