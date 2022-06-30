# myKeyShortCuts
 all important shortcuts, commands, etc.

## Commands
### Recursively Remove .DS_Store
- Open Terminal
- cd to/your/directory
- type: find . -name '.DS_Store' -type f -delete
- enter

Remove existing files from the repository:

find . -name .DS_Store -print0 | xargs -0 git rm -f --ignore-unmatch
Add this line:

.DS_Store
to the file .gitignore, which can be found at the top level of your repository (or create the file if it isn't there already).
You can do this easily with this command in the top directory:

echo .DS_Store >> .gitignore
Then commit the file to the repo:

git add .gitignore
git commit -m '.DS_Store banished!'