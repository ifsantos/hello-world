# Top 30 Git Commands You Should Know To Become a Git Master

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
12. Revert Unstaged and Staged Changes
13. Amend The Most Recent Commit
14. Rollback Last Commit
15. Rollback a Particular Commit
16. Create and Switch To a New Branch
17. List All Branches
18. Delete a Branch
19. Merge Two Branches
20. Show Commit Log as Graph For Current or All Branches
21. Abort a Conflicting Merge
22. Add a Remote Repository
23. View Remote URLs
24. Get Additional Information About a Remote Repository
25. Push Changes To a Remote Repository
26. Pull Changes From a Remote Repository
27. Merge Remote Repository With Local Repository
28. Push a New Branch To Remote Repository
29. Remove a Remote Branch
30. Use Rebase

## Refference:
<https://levelup.gitconnected.com/top-30-git-commands-you-should-know-to-master-git-cli-f04e041779bc>
