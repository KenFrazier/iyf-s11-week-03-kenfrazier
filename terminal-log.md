# Terminal Log — Week 03

A log of key CLI commands used this week, with notes on what each one did.

## Linux Navigation & File Search

```bash
pwd
```
Confirmed current working directory (`/workspaces/iyf-s11-week-03-kenfrazier`).

```bash
ls -a
```
Listed all files, including hidden ones like `.gitignore`.

```bash
find . -name "*.html"
```
Located all HTML files in the project directory.

## Shell Scripting

```bash
nano create-boilerplate.sh
```
Created a shell script using a heredoc to generate HTML boilerplate files.

```bash
chmod +x create-boilerplate.sh
./create-boilerplate.sh about
```
Made the script executable and ran it to generate `about.html`.

## Git — Remote Workflow

```bash
git clone <repo-url>
```
Cloned the Week 03 repository into Codespaces.

```bash
git remote -v
```
Verified the remote origin URL.

```bash
git pull origin main
```
Pulled the latest changes from the remote before starting work.

## Git — Branching & Merging

```bash
git branch feature/about-page
git checkout feature/about-page
```
Created and switched to a new feature branch for the about page.

```bash
git checkout main
git merge feature/about-page
```
Merged the feature branch back into `main`, resolving a conflict in the process (kept version A of the heading).

## Git — Committing & Pushing

```bash
git add .
git commit -m "feat: add about page"
git push origin main
```
Staged, committed with a conventional commit message, and pushed changes to GitHub.

## .gitignore

```bash
touch .gitignore
nano .gitignore
```
Created and configured `.gitignore` to exclude unnecessary files from version control.

---

*Log reflects commands practiced during IYF Season 11 Week 03 (Linux CLI, Git remote workflows, shell scripting).*
