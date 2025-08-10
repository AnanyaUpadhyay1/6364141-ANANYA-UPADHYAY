# Week 8 – Git Hands-On Labs

**Author:** Ananya Upadhyay  
**University:** KIIT University  
**Superset ID:** 6364141  
**University Roll No:** 22053488  

---

## 📌 Contents
1. **Lab 1:** Git Setup & Initial Commit  
   - Configured Git username, email, and default editor (Notepad++)  
   - Created `GitDemo` repository  
   - Added and committed `welcome.txt`  

2. **Lab 2:** Using `.gitignore`  
   - Created `log/` folder and `.log` files  
   - Updated `.gitignore` to exclude logs and folders  
   - Committed `.gitignore`

3. **Lab 3:** Branching & Merging  
   - Created branch `GitNewBranch`  
   - Added `newfile.txt`  
   - Merged branch into `master`

4. **Lab 4:** Merge Conflict Resolution  
   - Created branch `GitWork` and modified `hello.xml`  
   - Modified same file in `master` to create conflict  
   - Resolved conflict and committed merged file  
   - Updated `.gitignore` to exclude backup files

5. **Lab 5:** Cleanup & Push to Remote  
   - Verified branch status  
   - Pulled latest changes from remote  
   - Pushed all final commits to GitHub

---

## 🛠️ Git Commands Used
```bash
git init
git config --global user.name
git config --global user.email
git config --global core.editor
git status
git add
git commit -m
git branch
git checkout -b
git merge
git log --oneline --graph --decorate
git remote add origin
git push origin master
git pull origin master
