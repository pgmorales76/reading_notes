[Home](https://pgmorales76.github.io/reading_notes/)
# Class 3 Reading Notes

## Version Control

### - Version Control is a system that allows you to revisit various versions of a file or set of files by recording changes.### - By utilizing a Version Control System (VCS), mistakes with files can easily be rectified

## Local Version Control

### - Many years ago, programmers created Local Version Control systems. A Local VCS entails one database on your hard disk that stores changes to files

## Centralized Version Control

### - The need for collaboration within a developer team on a single file or set of files led to the advent of the Centralized Version Control System (CVCS)

## Distributed Version Control

### - A Distributed Version Control systems (DVCS) addresses the major vulnerability of the CVS: the server as a single point of failure. To prevent this type of catastrophic loss, a DVCS allows clients to create mirrored repositories

## So, what is Git?

### Snapshots

#### - Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called a commit — Git creates a snapshot of the file and stores a reference to it

### Local Operations

#### - Git mostly relies on local operations because most necessary information can be found in local resources

### Tracking Changes

#### - Every single change applied to any file, or directory. is tracked by Git

### Loss of Data

#### - Git is set up to greatly minimize the possibility of irreversible damage to files, such as accidentally lost data

### States

#### - Files in Git can reside in three main states: committed, modified and staged

#### - *Committed*: Data is securely stored in a local database

#### - *Modified*: File has been changed but not committed to the database

#### - *Staged*: Flagged a file’s changed version to be committed in the next snapshot

![Git states](/images/git_wit_it.png)

## History of Git

### - Git traces its roots to the open source software project Linux kernel

### - In 2005, Linus Torvalds, the chief architect of the Linux kernel, began creating Git

### - Git allowed for non-linear development via multiple branches, could support large projects, possessed strong mechanisms preventing corruption, and had a simple design

### - Since its inception in 2005, Git has become one of the most utilized Version Control Systems in the world

## Workflow

### Local Repository Structure

#### - The local Git repository has three components

1. Working Directory: The actual files reside here.
2. Index: The area used for staging.
3. Head: Points to the most recent commit.

![Git workflow](/images/git_wit_it_2.png)

### Saving Changes

#### - All files in a checked out (or working) copy of a project file are either in a tracked or untracked state

#### - *Tracked*: Can be modified, unmodified, or staged; they were part of the most recent file snapshot

#### - *Untracked*: Not in the last snapshot and does not currently reside in the staging area

### The Life Cycle of File Status

1. After you edit a file, Git flags it as modified because of changes made after the previous commit.
2. You stage the modified file.
3. Then, you commit staged changes.

![File Status Life Cycle](/images/git_wit_it_3.png)

[Git Tutorial](https://blog.udemy.com/git-tutorial-a-comprehensive-guide/)
