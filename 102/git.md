# Reading notes on git

Git is a Version Control System or VCS

## VCS's come in 3 flavors
1. Local Version Control
   - Does not allow for easy collaboration between people
2. Centralized Version Control
   - Allows for collaboration, but because there is a single point of access has a weak point.
   - If the server fails, then clients cannot work on projects
3. Distributed Version Control
   - This is how we are using git

## Git states
There are 3 main states within git:
1. committed
   - When committed, data is securely stored locally
2. modified
   - When data is modified, it is not yet committed
3. staged
   - When data is staged, it is flagged to be committed in the next snapshot

## Git flow
1. Set up your user settings

   ```bash
   git config --global user.name "Your Name"
   ```

   ```bash
   git config --global user.email "your@email.com"
   ```

2. set up a repository

   ```bash
   git clone <URL or path>
   ```

3. Edit your code in VS code or your preferred editor and then ACP

   ```bash
   # A(dd), C(ommit), P(ush)
   gat add [filename or directory]
   git commit -m "comments"
   git push <branch>
   ```

4. Additional git commands

   
   - `git status` - Show the current status of local snapshot
   - `git pull` - pull the HEAD commit from a master repository
   - `git branch` - creates a new branch
   - `git diff` - view the differences between two branchs
   - `git merge` - merge changes between two branches

[<= Back](README.md)                                                                                                                                                                                                                                                             