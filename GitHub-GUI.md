# GitHub Basics (GUI)

## Terms
__Repository__ (a.k.a. “repo”) - a place where the history of your work is stored

__Fork__ - a clone of a repository

__Branch__ - a snapshot or pointer of a repository at place in time; great explanation available at http://git-scm.com/book/ch3-1.html

__Commit__ - a set of changes to file(s) that belong to a repository

__Pull Request__ - a request to merge changes from a fork or branch into the main repository or vice versa

## Commit changes
When you make changes to code that belong to code in a `parent` repo, do the following:

### Make sure child is up-to-date with parent
1. If you have not already, fork `parent/repo` to your own `child/repo`.
2. From the `child/repo` page, click on the green arrow button to create a pull request.
3. The base fork should be `child/repo` and the head fork should be `parent/repo`. (__Note:__ _This is the exact opposite of what the default is._)
4. Make sure it is using the correct branch. (`master` or `HEAD` is correct for most cases)
5. If it says “There isn’t anything to compare” skip to the next section. Otherwise, continue with step 6.
6. Click on the green “Create Pull Request” button, and then click on “Send pull request.”
7. Then, if you can, click on the green “Merge pull request” button. If you are unable to merge pull request, please contact Star Verte support for help.
8. Continue on to the next section.

### Commit changes
1. From the `child/repo` page, click on the file you wish to edit.
2. From the file view page, click on “Edit” and make the desired changes.
3. Give a descriptive title for the commit, like “Removed extra spacing between paragraphs” or “Added function flint_content”
4. If applicable or helpful, add a description for the commit. The title should be less than 50 characters, so if you weren’t able to describe the changes in 50 characters, describe it here.
5. Click the green “Commit changes” button.
6. If you have other files to change, repeat this process until you have made all the desired changes.
7. Continue on to the next section.

### Submit changes via Pull Request
1. From the `child/repo` page, click on the green arrow button to create a pull request.
2. The base fork should be `parent/repo` and the head fork should be `child/repo`.
3. Make sure it is using the correct branch. (`master` or `HEAD` is correct for most cases)
4. If it says “There isn’t anything to compare,” make sure you followed the steps in the previous section correctly and/or contact Star Verte support for help. Otherwise, continue on to step 5.
5. Click on the green “Create Pull Request” button, give a descriptive title, and a description (optional) and then click on “Send pull request.”
6. If you are able to merge the pull request, the green “Merge pull request” button will show up. It is usually a good idea to have someone else review the code before merging the pull request, so _don’t_ click this button.
7. If you are unable to merge the pull request, you should still be able to see something that says, “This pull request can be automatically merged.” If instead you see something that says, “This pull request cannot be automatically merged,” cancel or delete the pull request and contact Star Verte support for help.
