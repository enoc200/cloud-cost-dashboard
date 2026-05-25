# Git Scenario-Based Questions (Intermediate → Advanced)

## 1. Merge Conflict Scenario
- Conflict happens when two branches edit the same section of a file.  
- Resolve by manually editing the file, keeping correct changes, then `git add` and `git commit`.

## 2. Accidental Commit to Main
- Create a new branch from the commit (`git branch feature-branch`).  
- Reset `main` to the previous clean commit (`git reset --hard origin/main`).

## 3. Remote Push Rejected
- Remote has commits not present locally.  
- Run `git pull --rebase origin main` before pushing.

## 4. Deleted Branch Recovery
- Commits can be recovered since Git history remains.  
- Use `git reflog` or `git log` to find and restore.

## 5. Sensitive Credentials Exposure
- Immediately rotate/invalidate exposed keys.  
- Remove secrets from history using `git filter-repo` or BFG.  
- Deleting the file alone is not enough because history still contains the keys.

## 6. Rebase vs Merge Decision
- Rebase gives a clean, linear history.  
- Risk: rewriting history can cause conflicts if others already pulled the branch.

## 7. Emergency Production Hotfix
- Create a `hotfix` branch from `main`.  
- Fix → test → merge into `main` → deploy → merge back into `develop`.

## 8. Working Directory Interruption
- Use `git stash` to save unfinished work.  
- Switch to `main`, fix issue, then `git stash pop` to resume.

## 9. Wrong Commit Message
- Correct with `git commit --amend -m "Clear, professional message"`.

## 10. Local Branch Behind Main
- Merge: `git merge main` → keeps history with merge commit.  
- Rebase: `git rebase main` → cleaner linear history.

## 11. Multiple Remote Repositories
- Organizations use multiple remotes for redundancy or different platforms.  
- Push with `git push github main` or `git push gitlab main`.

## 12. CI/CD Deployment Failure
- Use `git log` or `git bisect` to find the breaking commit.  
- Roll back safely with `git revert <commit>`.

## 13. Large Feature Development
- Problems: merge conflicts, outdated code.  
- Best practice: regularly rebase/merge with `main`.

## 14. Detached HEAD Situation
- HEAD points to a commit, not a branch.  
- Danger: new commits may be lost unless a branch is created.

## 15. Protected Main Branch
- Prevents accidental commits and enforces reviews.  
- Pull requests improve quality through review, testing, and collaboration.

