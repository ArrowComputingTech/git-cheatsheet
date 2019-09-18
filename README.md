--- Github cheat sheet ---

Configure git (only once per machine/O.S. install/environment setup)
   git config --global user.name "ArrowComputingTech"
   git config --global user.email "github@arrowcomputing.tech"

Creating a new local repo and push to a new Github repo:
   *do some coding
   cd /base_directory_of_project
   git init
   git add README.md
   git commit -m 'first commit'
   git remote add origin git@github.com:your_username/what_you_want_your_repo_named.git
   git push -u origin master

Get project from Github
   Go to project repo.
   // Click 'Clone or download' & copy link.
   git clone paste_link

Create new branch
   git branch new_branch_name
   // Then, switch to branch
   git checkout new_branch_name
   // OR use -b option to auto-switch
   git branch -b new_branch_name

Check what branch you're currently in
   git status

Push a change to Github
   git add .
   git commit -m 'Commit message'
   // OR combine these two commands with:
   git push -u origin master (or branch_name if you're on a different branch)

Merge a branch into master
   *do some work on a branch
   git checkout master
   git merge your_branch_name	

Delete a file from your local git repo
   git rm some_dir/file_name.txt

Rename a file in git repo
   git mv some_dir/first_file_name.txt some_dir/new_file_name.txt
