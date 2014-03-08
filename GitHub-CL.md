# GitHub Basics (Command Line)

## Terms
__Repository__ (a.k.a. “repo”) - a place where the history of your work is stored

__Fork__ - a clone of a repository

__Branch__ - a snapshot or pointer of a repository at place in time; great explanation available at (http://git-scm.com/book/ch3-1.html)

__Commit__ - a set of changes to file(s) that belong to a repository

__Pull Request__ - a request to merge changes from a fork or branch into the main repository or vice versa

## Install Git
### Windows
Download the installer via http://msysgit.github.com/.
__Note__: This installer includes Git BASH and Git GUI. Use Git BASH.
__Note__: Do not use the native command-line app in Windows, instead use Git BASH.
__Note__: For the instructions in this document, it is assumed that Git BASH is the same as Linux and Terminal.

### OS X
Download the installer via http://code.google.com/p/git-osx-installer.

After installing, use Terminal app for code below.

### Linux
For Fedora, install Git using

    $ yum install git-core

For Debian-based Linux distributions, install Git using

    $ apt-get install git

### Set up Git
Run the following code

    $ git config --global user.name "YOUR NAME HERE"
    $ git config --global user.email "YOUR_EMAIL@EXAMPLE.COM"
    
## Create a local repository
Using the command line, navigate to the directory that you want to put your local repository. Then, run the following code.
    
    $ mkdir REPO
    # Create a directory with the name of the repository
    
    $ cd REPO
    # Navigate to this new directory
    
    $ git init
    # Initialize git in this new directory
    
    $ git remote add origin https://github.com/CHILD/REPO.git
    $ git pull origin master
    # Add repository files from GitHub to local directory
    # For a large repository, this may take while
    
    $ git remote add upstream https://github.com/PARENT/REPO.git
    # Add 'upstream' reference for parent repository

## Submit changes
When you make changes to code that belong to code in a `parent` repo, do the following:

### Make sure child is up-to-date with parent

    $ git fetch upstream
    # Get all changes from parent repository


    $ git merge upstream/master -m 'Merge from master'
    # Merge parent 'master' branch with child
    # The stuff within the single quotes is a comment
    # The comment is required, but can be anything you wish

### Commit changes
1. Make changes to the files you need changed. For best results, use `nano`.
2. If you add any files, make sure to use `$ git add file.html`.
3. After making the desired changes, use the following code:

    $ git status
    # Check status of changes (optional)
    
    $ git commit -a -m 'Title of commit'
    # Commit changes with a descriptive title
    
    $ git push origin master
    # Push changes of local repository to remote child repository

### Submit changes via Pull Request
1. From the `child/repo` page, click on the green arrow button to create a pull request.
2. The base fork should be `parent/repo` and the head fork should be `child/repo`.
3. Make sure it is using the correct branch. (`master` or `HEAD` is correct for most cases)
4. If it says “There isn’t anything to compare,” make sure you followed the steps in the previous section correctly and/or contact Star Verte support for help. Otherwise, continue on to step 5.
5. Click on the green “Create Pull Request” button, give a descriptive title, and a description (optional) and then click on “Send pull request.”
6. If you are able to merge the pull request, the green “Merge pull request” button will show up. It is usually a good idea to have someone else review the code before merging the pull request, so _don’t_ click this button.
7. If you are unable to merge the pull request, you should still be able to see something that says, “This pull request can be automatically merged.” If instead you see something that says, “This pull request cannot be automatically merged,” cancel or delete the pull request and contact Star Verte support for help.
