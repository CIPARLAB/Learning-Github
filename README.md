# CIPAR LAB

## GitHub Tutorial 

### What is GitHub? 
GitHub is a platform that allows you to store and manage your code. It is a version control system that allows you to keep track of the changes that you make to your code. It is also a collaboration tool that allows you to work with other people on the same project.

### How to use GitHub? 
To use GitHub you have to install `git` on your local machine. you can download `git` from the following link: [git](https://git-scm.com/downloads).

In order to use `git` you have to open the terminal which is a command-line interface that allows you to interact with your computer. Terminal is installed on MacOS and Linux by default. While on Windows you have to install it. You can download the terminal from the following link: [Windows Terminal](https://www.microsoft.com/en-us/p/windows-terminal/9n0dx20hk701?activetab=pivot:overviewtab).
Alternatively, you can use `git bash` which is a terminal that comes with `git` installation or use one of Editor's terminal like `VSCode` or `PyCharm`.

### How to create a repository? 
To create a repository you have to go to the GitHub website and click on the `New` button. Then you have to fill in the information about the repository. You have to specify the name of the repository, the description of the repository, and the visibility of the repository. You can choose between public and private. If you choose public, everyone can see the repository. If you choose private, only the people that you invite can see the repository. Finally, you have to click on the `Create repository` button.

### How to clone, fetch, pull, and push a repository?

#### Git configuration
Before using `git` you have to configure it. You have to specify your name and your email. You can do this by using the following commands:
```bash 
git config --global user.name "Your Name"
git config --global user.email "Your Email"
```
The global option makes sure that every project in this computer uses the same username and email.  
You can also specify the default editor that you want to use. You can do this by using the following command:
```bash     
git config --global core.editor "Your Editor"
```
#### Setup a folder in local machine
To create a repository in your local machine you have to create a folder and then you have to open the terminal and navigate to the folder. You can do this by using the following command:
```bash
cd path_to_the_folder
```
Git would store all information in this folder. Making an entry, Staging Files. 
Git has a staging area that stores file changes that have not been committed yet. You can add files to the staging area by using the following command:
```bash
git add file_name
git add .
git add -A
git add -u
git add --all 
``` 
The first command adds a specific file to the staging area. The second command adds all the files in the folder to the staging area. The third command adds all the files in the folder to the staging area. The fourth command adds all the files that have been modified or deleted to the staging area. The fifth command adds all the files that have been modified, deleted, or created to the staging area.

You can always verify that Git is tracking your files by using the following command:
```bash
git status
git log 
```

#### Commit
After adding the files to the staging area you have to commit the changes. You can do this by using the following command:
```bash
git commit -m "Your Message"
```
The `-m` option is used to specify the message of the commit. The message should be a short description of the changes that you made.


#### Clone, fetch, pull, and push
##### Clone
`Clone` the repository means to download the repository to your local machine. Literally, you are making a copy of the repository in your local machine.  
To clone the repository you have to use the command `git clone` followed by the URL of the repository. 
```bash
git clone URL
```

While if you already have a copy of the repository in your local machine in order to synchronize the information that is on GitHub with the information that is on your local machine you have to use the
command `fetch`. `fetch` is used to download the information from the repository to your local machine.
```bash
git fetch
```

**pull** command is the combination of `fetch` and `merge`. It is used to download the information from the repository to your local machine and to merge the information that is on the repository with the information that is on your local machine.
```bash
git pull
```
However, you have to specify the branch that you want to merge in the case of lack of tracking information for the current branch. In this case, you have to use the following command:
```bash 
git pull origin branch_name
```
or alternatively, you can use the following command:
```bash
git branch --set-upstream-to=origin/branch_name
```

Finally, `push` command is used to upload the information that is on your local machine to the repository. 
```bash
git push
```
This command pushes to the main branch of the repository. If you want to push to a different branch you have to use the following command:
```bash
git push --all
```



### Ignoring files
Sometimes you want to ignore some files. For example, you want to ignore the files that are generated by the operating system or the files that are generated by the programming language that you are using. You can do this by creating a file called `.gitignore` in the root directory of the repository. In this file, you have to specify the files that you want to ignore. You can use wildcards to specify the files that you want to ignore. For example, you can use the following line to ignore all the files that have the extension `.log`:
To take care of ignoring files, a .gitignore file can be created at the root level
of your project, and inside that file, add any file or patterns that want to be
ignored:
   - .DS_Store
   - .vscode\
   - authentification.json
   - notes/
   - node.modules/
   - **/**-todo.md

Alternatively, you can use the following command to ignore files:
```bash
git config --global core.excludesfile [file]
git rm -r --cached . 
```

### Branching
Branching is a feature that allows you to work on different parts of the code at the same time. It is useful when you want to add a new feature to the code or when you want to fix a bug. You can create a new branch by using the following command:
```bash
git branch branch_name
```
This command creates a new branch called `branch_name`. You can switch to the new branch by using the following command:
```bash
git checkout -b branch_name
git switch -c branch_name
```
You can also create a new branch and switch to it by using the following command:
```bash
git checkout -b branch_name
```
You can list all the branches by using the following command:
```bash
git branch
```
You can delete a branch by using the following command:
```bash
git branch -d branch_name
```
You can merge a branch into the main branch by using the following command:
```bash
git merge branch_name
```
You can also rebase a branch into the main branch by using the following command:
```bash

git rebase branch_name
```
### Resolving conflicts
Sometimes when you merge a branch into the main branch you get a conflict. A conflict occurs when the changes that you made to the code conflict with the changes that someone else made to the code. You can resolve the conflict by opening the file that has the conflict and editing it. You can also use the following command to resolve the conflict:
```bash
git mergetool
```
    
    

Danial Zendehdel king 
