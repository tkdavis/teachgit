# TEACH GIT

_add your readme text somewhere here for your challenges_  

This guide is intended as a very soft introduction to git. Meaning it is missing many helpful and necessary commands like merge, rebase, reset, clean, clone, and many many others.
What isn't explained in this readme I will likely just explain in person for now. If I see common questions early on I can add to this guide as it is a living document.

A few useful references include:
* Cheatsheet - https://training.github.com/downloads/github-git-cheat-sheet/
* Documentation & more - https://git-scm.com/doc
* Github Docs Learning Resources - https://docs.github.com/en/get-started/start-your-journey/git-and-github-learning-resources

Come back to this very basic reference for the workflow as needed:  
<pre>
add -> commit -> push  
                   > (if failed push: ) -> pull -> push -> status to check if same as origin/main  
</pre>

---

### Challenge 1:  
Add a line to this Readme, stage, commit, and push to the remote repo.  
```git add .```  
```git status```  
```git commit -m "your short message here"```  
```git status```  
```git push origin main```  
```git status```  
```git log```

Check Github for your success!  

---

### Challenge 2:
Make some changes to the readme.  
Check the status, then remove your recent changes back to the main branch's state using the checkout command.  

```git status```  
(filename should be red meaning changes were made and are unstaged / haven't used the add command yet)  
```git checkout .```  
```git status```  
(checkout resets whatever you specify after the command to the original state of the most recent commit)  
(the . means you are checking out ALL unstaged files. you can instead specify a specific file if you want to reset just one file. See next line:)  
```git checkout readme.md```  

---

### Challenge 3:
Create a new feature branch, change this readme file again.  
Now we will repeat steps from challenge 1 but instead, push our new branch up and merge it through github via pull request.  

```git branch```  
```git checkout -b my-feature```  
```git branch```  
```git add .```  
```git status```  
```git commit -m "your short message here"```  
```git status```  
The -u flag below adds branch as a remote tracking branch, after pushing once with this flag you can use push without it in the future.  
```git push -u origin my-feature```  
```git status```  

Your branch should be successfully pushed up to Github!  
Now go through the pull request process with me (not covered in readme yet)  

---

Guide to be continued...



