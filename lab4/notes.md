1. --global makes the setting apply to all Git repositories for the current user. if you omit --global the setting applies only to the current repository.
2. it revealed Git's internal files and directories used to manage the repository.
3. There were 2 untracked files. I could identify the untracked code by running git status --untracked-files=all.
4. it's the same as my setup didn't contain any .venv/ directory or compiled files to ignore.The only thing that changed was that .gitignore was added to the list of untracked files.
5. .gitignore should be committed. It needs to be tracked by Git so that everyone working on the repository shares the same ignore rules, ensuring consistent behavior across all machines and preventing unwanted files like .venv/ or compiled code from being tracked by collaborators.
6. README.md moved from "Untracked files" to "Changes to be committed". In the three-places model, running git add README.md moved the file from the Working Directory into the Staging Area (Index), preparing it to be included in the next commit.
7. Git printed [master (root-commit) 3d74830] Lab work so far. It reported that 1 file changed and 1 insertion(+) was made.
8. The first seven characters (3d74830) are called a short commit hash (or short SHA-1 checksum). They serve as a unique ID to identify that specific commit snapshot in the repository's history.
