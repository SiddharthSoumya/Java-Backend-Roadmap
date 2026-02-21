# Phase 0 — CONFLICT A
# Phase 0 — Git + Linux + Tooling -:

## My Git workflow (the one I will follow)  
- **branch naming:** `feature/<short-description>` or `bugfix/<ticket-number>`  
- **commit style:** Conventional Commits (e.g., `feat: add login API`, `fix: correct typo in README`)  
- **steps:** branch → commit → push → merge (via pull request, after review)

## Commands I can use without looking  
- **git status / add / commit / push:**  
  - `git status`  
  - `git add <file>`  
  - `git commit -m "message"`  
  - `git push origin <branch>`  
- **branch / merge:**  
  - `git branch <branch-name>`  
  - `git checkout <branch-name>`  
  - `git merge <branch-name>`  
- **revert vs reset:**  
  - `git revert <commit-hash>` → creates a new commit that undoes changes  
  - `git reset --hard <commit-hash>` → moves HEAD back, discards changes  
- **stash:**  
  - `git stash` → save uncommitted changes  
  - `git stash pop` → reapply stashed changes  

## Merge conflict: what happened + how I resolved it  
- **conflict markers:**  
  - `<<<<<<< HEAD`  
  - `=======`  
  - `>>>>>>> branch-name`  
- **what I kept:** Chose the correct logic from my branch and added missing lines from incoming branch.  
- **final command sequence:**  
  - `git status` → see conflicted files  
  - edit files → resolve conflicts  
  - `git add <resolved-file>`  
  - `git commit`  
  - `git push`  

## Linux debugging flow  
1. Check logs → `cat`, `tail -f`, `grep "error" logfile.log`  
2. Check process → `ps aux | grep <process>`, `top`  
3. Check port → `ss -tuln` or `netstat -tuln`  
4. Curl endpoint → `curl -v http://localhost:8080/health`  

## Week 1 proof links  
- **link to conflict resolution commit:** (example) `https://github.com/<user>/<repo>/commit/<hash>`  
- **link to CI green run:** (example) `https://github.com/<user>/<repo>/actions/runs/<id>`  

---
