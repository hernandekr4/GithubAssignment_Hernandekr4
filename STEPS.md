# Steps for Git Assignment

1. Initialize repository.
   Command: `git init`

2. Created README.md and made initial commit.
   Command: `git add README.md`
            `git commit -m "Commit 0: Add initial README.md file"`

3. Added meme image and committed it.
   Command: `git add meme.png`
            `git commit -m "Commit 1: Add meme image"`

4. Created branches:
   Commands: 
     - `git checkout -b bug-fix`
     - `git checkout -b bug-fix-experimental`

5. Made conflicting changes on `master` and `bug-fix`:
   Commands:
     - On `master`: `git commit -m "Commit 5: Update Line 13 on master"`
     - On `bug-fix`: `git commit -m "Commit 6: Update Line 13 on bug-fix"`

6. Resolved merge conflict between `master` and `bug-fix`.
   Commands:
     - `git merge bug-fix`
     - Resolved conflict in README.md
     - `git add README.md`
     - `git commit -m "Resolve conflict between master and bug-fix"`

7. Pushed all branches to GitHub.
   Commands:
     - `git push origin master`
     - `git push origin bug-fix`
     - `git push origin bug-fix-experimental`
