Cañezo, Jay R. CSIT327 G5
Git Team Sync Lab - Workflow Answers

1. What did the rejected push error message tell you, and why did it happen?
The rejected push error message stated that updates were rejected because the remote contains work that my local branch does not have. This happened because the remote repository had already advanced(due to another clone/teammate pushing changes), making our local history outdated. Git prevents you from overwriting remote changes blindly.

2. What's the actual difference between how you resolved Task 3 (merge) vs Task 4 (rebase)?
Task 3 Combined different files by creating a new merge commit. It preserved both independent paths and showed the exact integration point where the two branches met.
Task 4 on the other hand, Took local commits and replayed them directly on top of the latest tip of the remote branch. This rewrote the local commit history to maintain a clean, linear timeline without adding a merge commit.

4. What one habit would have avoided both rejected pushes in this lab?
Having a habit of Running 'git pull' or 'git fetch' to sync with the remote repository before starting new work or attempting to push could avoid rejection problems.

5. Which approach – merge or rebase – would you default to on a shared team branch, and why?
I would default to merge on a shared team branch. Merging is non-destructive and preserves a transparent, accurate historical record of team collaboration and when features were integrated. Rebase rewrites history, which can disrupt teammates if used carelessly on shared branches.
