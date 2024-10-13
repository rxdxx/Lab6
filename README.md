# Lab6 Git-1

### version Control and Collaboration
- It's essential to use a version control system for software development and other documentation works.
- We need a systematic management system for version control and collaboration.

### Changes vs. Snapshots
- Changes
  - Storing data as changes to the base version
- Snapshots
  - Storing data as snapshots

 ### Git config : First-time setup
 - Git configurations are stored in three levels:  
(1) System level: --system option. Affects all uses and repositories on the system(administrative)  
*file: /etc/gitconfig*  
(2) Global (user) level: --global option. Affects all repositories of a current user  
*file: ~/.config/git/config*  
(3) Local level: --local option. Specific to the current repository  
*file: .git/gitconfig*  
\* Each level overrides values in the previous level: system->global->local
---
### Git
- git init: Initializing a Repository in an Existing Directory
- ls -lha: Can check hidden folder .git
- git status: Check the status of the repository
- git add [file_name]: Adding a new file to be staged(tracked)
  - git addd .: Adding all files to be staged(tracked)
- git rm --cached [file_name]: Unstaging a file
- nano .gitignore: Ignoring a file
  - \#ignore all .a files  
    \*.a  
  - \#but do track lib.a, even though you're ignoring .a files above  
    !lib.a  
  - \#only ignore the TODO file in the current directory, not subdir/TODO  
    /TODO  
  - \#ignore all files in any directory named build  
    build/  
  - \#ignore doc/notes.txt, but not doc/server/arch.txt  
    doc/*.txt  
  - \#ignore all .pdf files in the doc. diretory and any of its subdirectories  
    doc/\**/\*.pdf  

### Commit
- git commit -m "commit message"

### Change branch name
- git branch: Check branch working now
- git branch -m master main: Change branch (master -> main)
---
### Tip
- If there is a problem on nano(in windows), you can edit the file in any other text editor(e.g., 메모장)
- git log: Check commit history
