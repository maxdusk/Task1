git init 
mkdir Task1
nano Task1/README.md  / touch Task1/README.md
git add Task1
git commit -m "Initial commit"
git remote add task1 https://github.com/maxdusk/Task1.git
git push task1 master

git checkout -b dev
nano test.txt  /  touch test.txt
git add test.txt
git commit -m "dev branch commit"
git push task1 dev

git checkout -b maxdusk-new_feature
nano README.md
git add README.md
git status
nano .gitignore
git add .gitignore
git commit -m "maxdusk-new_feature commit"
git push task1 maxdusk-new_feature

# pull request and mrges done through web

nano README.md 
git add README.md 
git commit -m "edited README.md in maxdusk-new_feature" 
git log 
git revert 053648948c09c0b61bcd6080057a10990a720d20 
git checkout master git log 
echo $(git log) >> ./log.txt 
git checkout master
git add log.txt
git commit -m "added log file" log.txt
git pull task1 master
git push task1 master
git push task1 --delete maxdusk-new_feature
git branch -D maxdusk-new_feature






