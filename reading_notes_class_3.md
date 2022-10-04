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

