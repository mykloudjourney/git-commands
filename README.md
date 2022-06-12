# git-commands

# Git global setup
git config --global user.name "MyKloudJourney"
git config --global user.email "mykloudjourney@gmail.com"

# Clone Remote Repository
git clone <git-url>
cd <cloned-repo-name>
git switch -c main
touch README.md
git add README.md
git commit -m "add README"
git push -u origin main

# Push to an existing folder
cd <repo-name>
git init --initial-branch=main
git remote add origin <repo-url>
git add .
git commit -m "Initial commit"
git push -u origin main

# Push an existing Git repository
cd <repo-name>
git remote rename origin old-origin
git remote add origin <repo-url>
git push -u origin --all
git push -u origin --tags