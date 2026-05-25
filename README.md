Git Scenario-Based Questions (Intermediate
→ Advanced)
1. Merge Conflict Scenario
Two developers edited the same section of app.py in different branches. During merge, Git
reports a conflict.
●​ Why did the conflict happen?
●​ How would you resolve it safely?
2. Accidental Commit to Main
You accidentally committed unfinished code directly to the main branch instead of a feature
branch.
●​ How would you move the work to a new branch safely?
3. Remote Push Rejected
You try:
git push origin main
but Git says:
rejected because remote contains work you do not have locally
●​ Why did this happen?
●​ What should you do next?
4. Deleted Branch RecoveryA teammate deleted a feature branch after merge, but later realized important work is missing.
●​ Can the commits still be recovered?
●​ Which Git tools could help?
5. Sensitive Credentials Exposure
A developer accidentally pushed AWS keys into GitHub.
●​ What immediate actions should be taken?
●​ Why is deleting the file alone not enough?
6. Rebase vs Merge Decision
Your team wants a clean linear Git history with fewer merge commits.
●​ Would you recommend merge or rebase?
●​ What are the risks involved?
7. Emergency Production Hotfix
Your production application is down due to a login bug while new features are still being
developed.
●​ Which branch strategy should be used?
●​ Explain the workflow.
8. Working Directory Interruption
You are halfway through implementing a feature when your manager asks you to urgently fix
another issue on main.
●​ What Git feature helps you switch tasks safely without committing incomplete work?9. Wrong Commit Message
You committed:
git commit -m "stuff fixed"
●​ How can you correct the commit message professionally without creating another
commit?
10. Local Branch Behind Main
Your feature branch is several commits behind the latest main branch.
●​ How can you update your branch?
●​ Compare merge vs rebase approaches.
11. Multiple Remote Repositories
A DevOps engineer pushes code to both GitHub and GitLab from one local repository.
●​ Why might organizations use multiple remotes?
●​ How would you push to a specific remote?
12. CI/CD Deployment Failure
After merging code into main, the CI/CD pipeline fails and production deployment breaks.
●​ How can Git help identify the problematic changes?
●​ How can you safely roll back?
13. Large Feature DevelopmentA developer works on one branch for three months without merging updates from main.
●​ What problems can this create?
●​ What best practices could prevent this situation?
14. Detached HEAD Situation
A student checks out a specific commit directly using:
git checkout a1b2c3d
●​ What is a detached HEAD state?
●​ Why can it become dangerous?
15. Protected Main Branch
Your company prevents direct pushes to the main branch.
●​ Why is branch protection important?
●​ How do pull requests improve software quality and collaboration?
Expected Deliverables:
