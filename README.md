# HelloWorld (IntelliJ + Git + GitHub)

This repository contains a minimal Java Hello World project suitable for IntelliJ on Windows.

Files created:
- `src/Main.java` — Hello World program
- `.gitignore` — ignores IntelliJ and compiled files

Quick steps (PowerShell):

1. Open IntelliJ IDEA → New Project → Java → select JDK → Name `HelloWorld` → Finish.
2. Place `src/Main.java` under project `src` and run from IntelliJ.

Git commands (run in project root, e.g., `C:\Users\HP\IdeaProjects\HelloWorld`):

```powershell
git init
git branch -m main
git add src/
git commit -m "Initial commit - HelloWorld program"

# add .gitignore and commit
git add .gitignore
git commit -m "Add .gitignore to ignore IntelliJ files"

# (optional) configure user identity if commit fails
# git config --global user.name "Your Name"
# git config --global user.email "you@example.com"

# connect to GitHub (create repo on GitHub first)
# git remote add origin https://github.com/username/HelloWorld.git
# git push -u origin main
```

Notes:
- `.idea/` and `*.iml` are not committed.
- If you see `LF will be replaced by CRLF`, run `git config --global core.autocrlf true` to auto-convert.

If you want, I can also:
- create the GitHub repo for you (requires authentication), or
- run the git commands here and push (if you provide credentials/token).

Push to your supplied GitHub repository
-------------------------------------

Since you provided the repository URL `https://github.com/Advik2302/Step_AG1`, here are exact PowerShell commands to run from the project root (e.g., `C:\Users\Admin\Desktop\advik\HelloWorld`):

```powershell
# initialize (if you haven't already)
git init
git branch -m main

# stage source and README
git add src/ .gitignore README.md
git commit -m "Initial commit - HelloWorld program"

# add remote and push
git remote add origin https://github.com/Advik2302/Step_AG1.git
git push -u origin main
```

Authentication:
- If prompted, complete auth in the browser or use a personal access token (PAT).
- To avoid CRLF warnings on Windows: `git config --global core.autocrlf true`.

If you'd like, run the commands and tell me any errors you see, or ask me to create a push script for you to run.
