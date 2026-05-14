# git-commands
# go into your repo
cd git-commands

# overwrite README.md
cat > README.md << 'EOF'
# git-commands

## Description
This repository provides a beginner-friendly guide to essential Git commands and their commonly used flags.

## Purpose
The purpose of this repo is to help users understand how to use Git for version control, including cloning repositories, managing branches, committing changes, and working with remote repositories.

## Files
- commands.md – Contains explanations and examples of Git commands and flags

## How to Use
Open commands.md to learn what each command does and how to use it with examples.

## Author
imspidermanbatman
EOF

# overwrite commands.md
cat > commands.md << 'EOF'
# Git Commands Guide

## git clone
Clones a remote repository to your computer.
git clone <repository-url>

## git checkout
Switches branches.
git checkout branch-name

### -b
Creates and switches to a new branch.
git checkout -b new-branch

## git status
Shows current changes.
git status

## git push
Uploads commits to remote.
git push

### -u
Sets upstream branch.
git push -u origin main

## git pull
Fetches and merges changes.
git pull

## git add
Stages files.
git add file.txt
git add .

## git commit
Saves changes.

### -m
Adds a message.
git commit -m "message"

### -a
Stages modified files.
git commit -a

### -am
Stages + message.
git commit -am "message"

## git branch
Lists branches.
git branch

### -a
Lists all branches.
git branch -a

### -d
Deletes a branch.
git branch -d branch-name

## git merge
Merges branches.
git merge branch-name
EOF

# push changes
git add .
git commit -m "Add README and commands documentation"
git push