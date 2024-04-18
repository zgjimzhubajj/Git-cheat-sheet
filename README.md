# Git-cheat-sheet
## Welcome to this repository where I will be showing a summary of more commonly used Git commands!
# SETUP
- Configuring user information used across all local repositories
   - `git config --global user.name “[firstname lastname]”`
      - set a name that is identifiable for credit when review version history
   - `git config --global user.email “[valid-email]”`
      - set an email address that will be associated with each history marker
# SETUP & INIT
- Configuring user information, initializing and cloning repositories
   - `git init`
      - initialize an existing directory as a Git repository
   - `git clone [url]`
      - retrieve an entire repository from a hosted location via URL (When pasting the URL avoid using brackets)
# STAGE & SNAPSHOT
- Working with snapshots and the Git staging area
   - `git status`
      - show modified files in working directory, staged for your next commit
   - `git add [file]`
      - add a file as it looks now to your next commit (stage)
   - `git add .`
      - add all changes in the current directory
   - `git reset [file]`
      - unstage a file while retaining the changes in working directory
   - `git diff`
      - diff of what is changed but not staged
   - `git diff --staged`
      - diff of what is staged but not yet commited
   - `git commit -m “[descriptive message]”`
      - commit your staged content as a new commit snapshot
   - `git commit -a`
      - commit any files you've added with git add, and also commit any files you've changed since then
# BRANCH & MERGE
- Isolating work in branches, changing context, and integrating changes
   - `git branch`
      - list your branches. a * will appear next to the currently active branch
   - `git branch [branch-name]`
      - create a new branch at the current commit
   - `git checkout`
      - switch to another branch and check it out into your working directory
   - `git merge [branch]`
      - merge the specified branch’s history into the current one
   - `git log`
      - show all commits in the current branch’s history
   - `git status`
      - list the files you've changed and those you still need to add or commit
# SHARE & UPDATE
- Retrieving updates from another repository and updating local repos
   - `git remote add [alias] [url]`
      - add a git URL as an alias
   - `git fetch [alias]`
      - fetch down all the branches from that Git remote
   - `git merge [alias]/[branch]`
      - merge a remote branch into your current branch to bring it up to date
   - `git push [alias] [branch]`
      - transmit local branch commits to the remote repository branch
   - `git push`
       - upload local repository content to a remote repository
   - `git push --all origin`
       - push all branches
   - `git pull`
     - fetch and merge any commits from the tracking remote branch






