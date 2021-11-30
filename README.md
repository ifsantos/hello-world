# Top 30 Git Commands To Become a Git Master :godmode:

00.  Setup ssh key

       ssh-keygen -t ed25519 -C fs.ismael@gmail.com
       // Set public key on Github settings
       eval $(ssh-agent -s)
       ssh-add id_ed25519

0. List config
1. 
       git config --list

1. Set Up Your Username and Email
        
       git config --global user.name "Tara Routray"
       git config --global user.email "dev@tararoutray.com"

2. Cache Your Login Credentials
   
        git config --global credential.helper cache

3. Initialize a Repository

        git init

4. Add Individual File or All Files To Staging Area

        git add somefile.js
        git add .

5. Check a Repository Status

        git status

6. Commit Changes With a Single Line Message or Through an Editor

        git commit -m "Your short summary about the commit"
        git commit

7. View Commit History With Changes
 
        git log -p

8. View a Particular Commit
    
        git show 1af17e73721dbe0c40011b82ed4bb1a7dbe3ce29
        git show 1af17e

9. View Changes Before Committing
    
        git diff
        git diff --staged
        git diff somefile.js

10. Remove Tracked Files From The Current Working Tree
        
        git rm dirname/somefile.js
        git rm dirname/*.html

11. Rename Files

        git mv dir1/somefile.js dir2

12. Revert Unstaged and Staged Changes
        
        git checkout somefile.js
        git reset HEAD somefile.js
        git reset HEAD

13. Amend The Most Recent Commit (Alert!!! Don’t amend public commits.)

        git commit --amend -m "Updated message for the previous commit"
        git add dir1  
        git commit 
        
    Here you forgot to add dir2 to commit, you can execute the following command to amend the other files and folders.
    
        git add dir2  
        git commit --amend --no-edit

14. Rollback Last Commit
        
        git revert HEAD

15. Rollback a Particular Commit
        
        git revert 1af17e

16. Create and Switch To a New Branch

        git branch new_branch_name
        git checkout -b new_branch_name

17. List All Branches

        git branch
        git branch -a

18. Delete a Branch

        git branch -d existing_branch
        git branch -D existing_branch_name
        git push origin --delete existing_branch_name //# Pushing local deletion to remote

19. Merge Two Branches

        git merge existing_branch_name
        git merge --no-ff existing_branch_name //# Generates a merge commit

20. Show Commit Log as Graph For Current or All Branches

        git log --graph --oneline --decorate
        git log --all --graph --oneline --decorate //# for all brnaches

21. Abort a Conflicting Merge

        git merge --abort
        git reset

22. Add a Remote Repository

        git remote add awesomeapp https://github.com/someurl..

23. View Remote URLs
        
        git remote -v

24. Get Additional Information About a Remote Repository

        git remote show origin

25. Push Changes To a Remote Repository

        git push origin main

26. Pull Changes From a Remote Repository

        git pull
        git pull --verbose

27. Merge Remote Repository With Local Repository

        git merge origin

28. Push a New Branch To Remote Repository

        git push -u origin new_branch

29. Remove a Remote Branch

        git push --delete origin existing_branch

30. Use Rebase (Rebasing is a process to combine or move a sequence of commits to a new base commit.)
        
        git rebase branch_name
   -[ ] The above command will change the base of your branch from one commit to another, which will make it appear as if you have created your branch from a different commit. Git achieves this by creating new commits and applying them to the specified base. It’s very necessary to understand that even though the branch looks the same, it’s comprised of entirely new commits.

## Refference:
 - <https://levelup.gitconnected.com/top-30-git-commands-you-should-know-to-master-git-cli-f04e041779bc>


