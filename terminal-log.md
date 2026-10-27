# Terminal Log - Task 5.1

practice location: ~/terminal-practice (outside repo)

Exercise 1: Basic Navigation
- pwd - printed current directory
- ls- listed files
- cd ~/Documents - moved to documents folder
- cd .. - went back one level
- cd ~ - went to home

Exercise 2: Create project structure
- mkdir -p my-project/src/css - created css folder
- mkdir -p my-project/src/js - created js folder
- mkdir -p my-project/src/images - created images folder
- mkdir -p my-project/docs - created docs folder
- mkdir -p my-project/tests - created tests folder
- touch my-project/README.md - created empty README file
- ls -R my-project - checked the structure
- Copy-Item about.html -Destination my-project/src/ copied about.html to src
- Copy-Item styles.css -Destination my-project/src/css/ - copied css to css folder
Copy-Item sunset.jpg -Destination my-project/src/images/ - copied image to images folder

# Terminal Log - Task 5.2 Exercise 1:

- New=Item index.html - created new file
- Copy-Item index.html backup.html - copied index to backup
- Move-Item backup.html docs/ - moved backup to docs folder
- Rename-Item index.html home.html - renamed index to home
- Remove-Item home.html - deleted home.html

# Terminal Log - Task 5.2 Exercise 2

- Copy-Item -Recurse src/ src-backup/ copied src folder recursively
- Move-Item src-backup/ archive/ - moved src-backupto archive
- Remove-Item archive/ - tried to remove (folder not empty error)
- Remove-Item -Recurse -Force archive/ - force deleted archive folder
# Terminal Log - Task 5.3 Exploring portfolio

1. Count HTML files

- Command: dir -Recurse -Filter *.html
- Result: Found 2 files - about.html(2388 bytes) and backup.html
- Answer:2 HTML files in total
2. Search for "contact":

- Command: -Filter *contact*
- Result: No matches found / or Found 0 - no contact.html in this folder
Answer: No contact file in this folder
3. Count CSS lines

- Command: Get-Content .\src\css\styles.css |Measure-Object -Line
- Result: Lines = 131
- Answer: styles.css has 131 lines
4. Command history

- Command: history
- Result: Shows last commands like dir, Get-ChildItem, Select-String, history
- Answer: Last commands were file exploration commands
# Terminal Log Git Basics

1. Command: git add styles.css
   Result: staged changes
   Answer: Added navigation hover underline

2. Command: git commit -m "style: add navigation hover underline"
   Result: commit created
   Answer: First commit 

3. Command: git commit -m "Fix: correct responsive breakpoint fot projects grid"
   Result: commit created
   Answer: Fixed projects grid to1fr at 800px

4. Command: git commit -m "Docs: add terminal log"
   Result: commit created
   Answer: completed with 3 commits