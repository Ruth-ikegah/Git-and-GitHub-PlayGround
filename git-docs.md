<div align="center">
    <h1>Git</h1>
</div>

## What is Git

Git is the most commonly used version control system. Git tracks the changes you make to files, so you have a record of what has been done, and you can revert to specific versions should you ever need to. Git also makes collaboration easier, allowing changes by multiple people to all be merged into one source.

Version control is a means of recording changes to a file or set of files over time so that you can recall specific versions later.

### 1. Install Git

First, you need to install the Git version control software.

- Git:
  Install [git](https://git-scm.com/downloads)


### 2. Checking status of the repository

The _git status_ command allows you to know the status of the project:
If it is

- initiated
- modified
- staged

We can write the command _git status_ at any time. It is a means to to check what is happening on your project.


### 3. Configure your name and your email

Open the Git bash if your device is Windows, or open the Mac terminal if your device is MacOS and then write the following commands

```shell
git config --global user.name 'yourname'
git config --global user.email 'youremail'
```

### 4. Create a local git repository

In this step, you will create a folder (directory) for your project. A project is just a simple folder that stores all the files related to a certain project. A local repository is a project or a folder that is on your computer.

If your Git bash is not opened, go to start and type git bash. Git terminal will popup on Windows devices. If it is MasOS just open the Mac terminal. On the terminal write:

```shell
mkdir project_name
cd project_name
```

By the way, you can also create the folders the usual way using on the GUI(Graphical User Interface) of Windows or Mac.


### 5. Initialize Git

After creating a new local repository or in an existing local repository, initialize the repository by the following command:

```shell
   git init
```

Once, the repository is initialized git tracks the changes in the files and folders of the project.


### 6. Add file to the staging area

The file can be added to the staging area in multiple ways.
To add a single file, we use the _git add_ command followed by a file name

```shell
   git add filename
```

To add multiple files using their file names using the command _git add_ followed by file names

```shell
   git add filename1 filename2
```

Sometimes, we make a lot of changes, and adding files one by one is time consuming. Therefore, we can use a short and productive way. The _git add_ command followed by a dot allows adding files and folders at once to the staging area. Remember, there is a space between the add and the dot.

To add all files and folders at once

```shell
   git add .
```

### 7. Unstage a file

```shell
    git reset HEAD filename
```

### 8. Commit the changes

Commit means taking a snapshot or a copy of your file at that point in time. You may associate it with saving a file with a new name (save as).

```shell
   git commit -m 'your message'
```
Your commit message has to be associated with the changes or modifications you make.

To add and commit at the same time

```sh
   git commit -am 'commit message'
```

### 9. Git log

The _git log_ command allows you to check  the commit history of the project. It list down all the commit history

```sh
   git log
```


### 13. Creating a branch

Branch in Git is similar to the branch of a tree. Analogically, a tree branch is attached to the central part of the tree called the trunk. While branches can generate and fall off, the trunk remains compact and is the only part by which we can say the tree is alive and standing. Similarly, a branch in Git is a way to keep developing and coding a new feature or modification to the software and still not affecting the main part of the project. We can also say that branches create another line of development in the project. The primary or default branch in Git is the main branch (similar to a trunk of the tree). As soon as the repository creates, so does the main branch (or the default branch).

To create a branch:

- Only to create branch

```shell
    git branch -u branch-name
```

- To create and checkout to the branch at the same time:

```shell
    git checkout -b branch-name
```

To switch between branches:

```shell
    git checkout main
    git checkout branch-name
```

To list down all the branches:

```shell
    git branch
```