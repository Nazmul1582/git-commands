# Git Commands 🔥
### A list of git commands which are commonly used.

### *1. Some basic command line*
| Command | Description |
| ------- | ----------- |
| `ps` | show the default terminal of a system ( not working in windows operating system) |
| `ls` | show all file and folder of the directory |
| `pwd` | show present working directory name |
| `cd\` | go to the root folder or C: drive | 
| `d:` | changed the directory into D: drive |
| `cd NewFolder` | entered the folder named **NewFolder** | 
| `cd 'New folder'` | entered the folder named **New folder** (if the folder's name is more than one word, have to write folder name in quotation |
| `cd ..` | back from the directory |
| `mkdir NewFolder ` | `mkdir` means "make directory". this command create a folder named "NewFolder" |
| `rmdir existingFolder ` | `rmdir` means "remove directory". this command removed the folder named "existingFolder" |
| `touch fileName (index.js)` | create index.js file |
| `rm existingFile ` | removed the file named "existingFile" |
| `cat index.js` | show all content of index.js |
| `start index.js` | opened index.js file in the default software |
| `start firefox index.js` | opened index.js file in Firefox browser  |
| `⬆` | show the previous command |
| `⬇` | show the next command |
| `Tab` | by clicking tab key after typing few letters, it does fulfill the name. (example: cd in "clicked tab key", it will cd index.js "again clicked tab key", it will show all files & folders which is started by in [like: index.html, index.js, info ...]  ) |
| `clear` | clear the terminal |

## 🏢 Working with git and github

### *2. Git initialized and set username and email*
| Command | Description |
| ------- | ----------- |
| `git init` | initialize git in your working directory |
| `git config --global user.name "username"` | set username in git globally |
| `git config --global user.email "email"` | set email address in git globally |

### *3. Add/Staged repository from working directory(wd)*

| Command | Description |
| ------- | ----------- |
| `git status` | see the changes |
| `git add --all` or `git add -A` | staged all changes (files and folders)  |
| `git add .` | staged this directory also it's childs(it's files and folders)  |
| `git add *` | staged changes without deleted  files and folders |
| `git add demo.js` | staged only demo.js |
| `git add myFolder/demo.js` | staged only myFolder/demo.js |
| `git add *.js` | staged all .js extention files |

### *4. Restore*

| Command | Description |
| ------- | ----------- |
| `git reset` | back working directory from staged |
| `git reset HEAD~` | back working directory from local repository |
| `git reset --hard` | back changes and deleted files to working directory from local repository |
| `git checkout index.html` | restored and staged index.html from local repository after commited |
| `git checkout -f` | restored and staged all files and folders from local repository after commited |

### *5. Commit*

| Command | Description |
| ------- | ----------- |
| `git commit -m "message"` | commited (local repository) |
| | **Another way to commit** |
| `git commit [another way]` | `press i` to active vim editor. Then type massage (initial commit) & `press Esc` key. Finally type `:wq` & `press Enter` key | 

### *6. Remove files or folders*

| Command | Description |
| ------- | ----------- |
| `git rm index.js` | removed index.js and staged (if you remove manually, have to staged again ) |
| `git rm index.js -f` | removed index.js and staged after modified or changed |
| `git rm --cached index.js` | removed index.js and staged after modified or changed but still remain index.js in wd which is untracked! |
| `git rm -r folderName` | removed the folder and it's all child files and folders |

### *7. Checkout, Branch and Merge*

| Command | Description |
| ------- | ----------- |
| `git branch` | show all branches |
| `git branch dev` | created a new branch named "dev". It's a copy of master branch |
| `git checkout dev` | Switched to branch "dev" |
| `git checkout -b another` | Created and Switched to a new branch "another" |
| `git merge dev -m "message"` | Merging on master with dev |

### *8. Clone and Remote*

| Command | Description |
| ------- | ----------- |
| `git clone "link"` | cloned the remote repository in local repository |
| `git remote` | show the remote name |
| `git remote -v` | show remote name and address (this command used to check/verify remote) |
| `git remote add origin "link"` | set the remote in repository |
| `git remote set-url origin "link"` | set the new remote in repository (used to change remote) |


### *9. Push*

| Command | Description |
| ------- | ----------- |
| `git push origin master` | pushed local repository to remote/github (here origin is remote & master is branch)  |
| `git push -u origin master` | pushed local repository to remote/github (here origin is remote & master is branch) |

### *10. Fetch, Merge and Pull*

| Command | Description |
| ------- | ----------- |
| `git fetch` | all changes of remote to local repository (not wd/ not updated local branch ) |
| `git fetch` + `git merge` | all changes of remote to local repository & wd(nothing to commit) |
| `git pull` | all changes of remote to local repository & wd(nothing to commit) |

### *11. Log and Diff*

| Command | Description |
| ------- | ----------- |
| `git log`| show all commits with author, date and time [`press q` to go the terminal]  | 
| `git log -p -1`| show last 1 commit with difference and info [`press q` to go the terminal] | 
| `git diff`| show the difference between unstaged and last commit (`git diff` works before commited) [`press q` to go the terminal] | 
| `git diff --staged`| show the difference between staged and the last commit [`press q` to go the terminal] | 
