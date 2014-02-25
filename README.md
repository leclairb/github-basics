# GitHub Basics
    This repository is only intended for use by team members
    in the "New Vuyiroli Website" team
    in CIS320 - Project Management in Information Technology.

Through this assignment, you will learn about:
* GitHub registration and organizations
* Repositories (aka repos)
* Markdown
* Forks
* Branches
* Commits
* Pull Requests

`user` refers to your GitHub username

## Initial setup
1. If you do not already have a GitHub account, go to https://github.com/join and go through the guided process.
2. Email Matt at `matt -dot- beall -at- me -dot- com`. He will add you to the organization `c320vws` so that you can create/manage issues and pull requests for the various repos.
3. Go to https://github.com/c320vws/github-basics and click on "Fork." This creates a copy of `c320vws/github-basics` under your personal account, at `user/github-basics`.

## Making changes using a branch
1. Go to `user/github-basics`, click on the dropdown menu that says "branch: master" and type in the first four letters of your last name and the first two letters of your first name (i.e. `llllff`). For example, Matt Beall would become `bealma`. Hit `ENTER`. This creates a branch (copy) of the `master` branch.
2. Using the branch you just created, click on the `names` directory and then the plus sign to create a new file.
3. In this screen, you can go back and forth between the "Code" view and the "Preview." Name the new file `llllff.md`, using the same name as the branch you created.
4. In the "Code" view, type `# First Last`, using your name. Feel free to write additional markdown below this.
5. In the "Commit changes" dialog, there is a title field. You can use the default for this example (`Create llllff.md`), but in the future the default will most likely not be acceptable. The title should give a short description (less than 50 characters) of changes made.
6. If you want, you can add an optional extended description. For this commit, this doesn't really make sense, but the description may prove useful later.
7. Click "Commit changes."

## Merging changes into master branch
Now that you have added the `llllff.md` file in the `llllff` branch, it's time to merge those changes into the `master` branch.

1. Go to `user/github-basics` and make sure that you are in the correct branch. To change the branch, select the dropdown menu.
2. Click on the green button to the left of the branch dropdown.
3. On the next screen, you will see two dropdown menus: base and compare (or head).
 * the compare (or head) branch/fork is the branch/fork with the changed files
 * the base branch/fork is the branch/fork that you are merging the compare branch files into
4. Make sure the base fork is `user/github-basics` and base branch is `master`.
5. Make sure the head fork is `user/github-basics` and compare branch is `llllff`.
6. Click "Create Pull Request", and then "send pull request".
7. Because this is your personal repo, on the next page you will be able to "Merge pull request." Click on this and then "Confirm merge."
8. Please do NOT delete the branch.

## Submit pull request for parent repo
Now that you have merged the changes into your personal master branch, it's time to merge those changes into the parent (`c320vws/github-basics`) master branch.

1. Before submitting a pull request for the parent repo, make sure that your personal master branch is up to date with the parent master branch. This step is not essential in this tutorial, but will mitigate issues in the future.
 1. Go to `user/github-basics` and make sure that you are in the master branch.
 2. Click on the green button to the left of the branch dropdown.
 3. Make sure the base fork is `user/github-basics` and the base branch is `master`. (You may need to click "Edit" to change this.)
 4. Make sure the head fork is `c320vws/github-basics` and the head branch is `master`. (You may need to click "Edit" and "compare across forks" to change this.)
 5. Click "Create Pull Request", and then "send pull request".
 6. Because this is your personal repo, on the next page you will be able to "Merge pull request." Click on this and then "Confirm merge."
 7. If you are unable to merge, please email Matt for help.
2. If you have completed step one successfully, submit pull request to parent repo.
 1. Go to `user/github-basics` and make sure that you are in the master branch.
 2. Click on the green button to the left of the branch dropdown.
 3. Make sure the base fork is `c320vws/github-basics` and the base branch is `master`. (You may need to click "Edit" to change this.)
 4. Make sure the head fork is `user/github-basics` and the head branch is `master`. (You may need to click "Edit" and "compare across forks" to change this.)
 5. Click "Create Pull Request", and then "send pull request".
 6. Because this is the parent repo, you shouldn't be able to "Merge pull request." If you can, please email Matt to let him know.
 7. If you are unable to merge, please email Matt for help.

If you followed all the steps above and completed them successfully, you're done!
