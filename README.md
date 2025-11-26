# Workshop Preparation Guide
## Reproducibility in Research: Markdown & GitHub



Please complete the following setup **before** attending the workshop. This will ensure we can focus on learning rather than troubleshooting installation issues.

---

## Required Software

### 1. Git

**Windows:**
- Download from [git-scm.com/download/win](https://git-scm.com/download/win)
- Run the installer with default options
- This includes Git Bash, which provides a Unix-like terminal

**macOS:**
- Option A: Install Xcode Command Line Tools by opening Terminal and running:
  ```bash
  xcode-select --install
  ```
- Option B: Download from [git-scm.com/download/mac](https://git-scm.com/download/mac)

**Linux (Debian/Ubuntu):**
```bash
sudo apt update
sudo apt install git
```

**Verify installation:**
```bash
git --version
```
You should see something like `git version 2.x.x`

---

### 2. GitHub Account

- Create a free account at [github.com](https://github.com)
- **Important:** Remember your username and password
- Consider enabling Two-Factor Authentication (2FA) for security
- (Optional) Add a profile picture and bio

---

### 3. Configure Git with Your Identity

Open a terminal (Git Bash on Windows) and run:

```bash
git config --global user.name "Your Full Name"
git config --global user.email "your.email@example.com"
```

Use the **same email** you used for your GitHub account.

---

### 4. Python & Jupyter

**Option A: Anaconda (Recommended for beginners)**
- Download from [anaconda.com/download](https://www.anaconda.com/download)
- Run the installer
- This includes Python, Jupyter, and many scientific packages

**Option B: pip install (if you already have Python 3.8+)**
```bash
pip install jupyter notebook
```

**Verify installation:**
```bash
jupyter --version
```

---

### 5. RISE (Jupyter Slideshow Extension)

After installing Jupyter, install RISE:

```bash
pip install rise
```

**For Jupyter Lab users:**
```bash
pip install rise
jupyter labextension install rise
```

**Verify:** Open a Jupyter notebook and look for a bar chart icon in the toolbar (Enter/Exit RISE Slideshow).

---

### 6. Text Editor (Choose One)

You'll need a good text editor for writing Markdown and code:

| Editor | Platform | Notes |
|--------|----------|-------|
| **VS Code** | All | Recommended - excellent Git integration |
| **Sublime Text** | All | Fast and lightweight |
| **Atom** | All | GitHub-made, good for beginners |
| **Notepad++** | Windows | Simple and reliable |

**VS Code** is particularly recommended because it has:
- Built-in Git support
- Markdown preview
- Jupyter notebook support
- Terminal integration

Download VS Code: [code.visualstudio.com](https://code.visualstudio.com)

---

## Optional but Helpful

### GitHub Desktop
A visual interface for Git operations:
- Download from [desktop.github.com](https://desktop.github.com)
- Helpful if you're uncomfortable with command line

### SSH Key Setup (Advanced)
For passwordless GitHub access:
1. Generate a key: `ssh-keygen -t ed25519 -C "your.email@example.com"`
2. Add to GitHub: Settings → SSH and GPG keys → New SSH key
3. Paste contents of `~/.ssh/id_ed25519.pub`

---

## Pre-Workshop Checklist

Please verify each item before the workshop:

- [ ] Git is installed (`git --version` works)
- [ ] You have a GitHub account and remember your login
- [ ] Git is configured with your name and email
- [ ] Jupyter is installed (`jupyter --version` works)
- [ ] RISE is installed (slideshow icon appears in Jupyter toolbar)
- [ ] You have a text editor installed
- [ ] You can open a terminal/command prompt

---

## Troubleshooting

### "git is not recognized as a command"
- Windows: Restart your terminal, or use Git Bash specifically
- Mac/Linux: Reinstall Git and restart terminal

### "jupyter: command not found"
- Make sure Python/Anaconda is in your PATH
- Try: `python -m jupyter notebook`

### RISE slideshow button not appearing
- Make sure you're in a notebook (not JupyterLab by default)
- Try: `jupyter nbextension enable rise --py --sys-prefix`

### Need help?
Contact the instructor before the workshop if you encounter issues.

---

## What to Bring

- **Laptop** with the above software installed
- **Charger** (2-hour workshop)
- **Notebook/pen** for notes (optional)

---

See you at the workshop! 🎓