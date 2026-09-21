# Git Workflow Lab

## Screenshots
### Task 1
![Task 1](screenshots/task1.png)
### Task 2
![Task 2](screenshots/task2.png)
### Task 3
![Task 3](screenshots/task3.png)
### Task 4
![Task 4](screenshots/task4.png)
### Task 5
![Task 5](screenshots/task5.png)
### Task 6
![Task 6](screenshots/task6.png)

## Questions

**What did the rejected push error message tell you, and why did it happen?**
It told me my local branch was behind the remote repository. This happened because Clone A pushed changes first, and when Clone B tried pushing without pulling first, Git blocked it to prevent overwriting code.

**What's the actual difference between how you resolved Task 3 (merge) vs Task 4 (rebase)?**
A merge combined our histories and created an extra merge commit. A rebase temporarily shifted my commit aside, pulled the remote updates, and replayed my commit on top to keep the history in a straight, clean line.

**What one habit would have avoided both rejected pushes in this lab?**
Running `git pull` right before starting work and before pushing.

**Which approach - merge or rebase - would you default to on a shared team branch, and why?**
I'd use rebase for updating my local feature branch to keep the history clean. I'd use merge for bringing a finished feature into `main` to show when the work was completed.