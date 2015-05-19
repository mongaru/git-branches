# git-branches
A small repository to test git branches with multiple actions to have an easy history on how to manage development of new features in projects.

# Procedure

\# **Step 1**:

create file "index.html" with simple content.

\# **Step 2**:

create the folloging folder structure:

-assets<br/>
--css<br/>
---style1.css - with some basic css rules<br/>

\# **Step 3**:

Commit to repository and origin.

\# **Step 4**:

Create brach called "branch-1".

\# **Step 5**:

Create the following files:

-assets<br/>
--css<br/>
---style2.css<br/>
---style1.css - change the existing file<br/>

\# **Step 6**:

Commit changes to "branch-1".

Change local branch to master and check if the folder structure has changed.

Comment: At this point when changing the branch and go back to the text editor you should get the following message.

"/Applications/XAMPP/xamppfiles/htdocs/git-branches/README.md - Has changed on disk. - Do you want to reload it?"

As you can see when changing to a different branch, git restores the files AND FOLDERS AS WELL since you will not see the "style2.css" file. This means that a branch (which is basically a pointer to a commit in the history) has the changes made to the repository in a certain point.

Important Notice: the reason why git insist in commit any modified files when switching branches is because you will loose any modification that was not commited in the given branch.

\# **Step 7**:

Go back to "branch-1" and push branch to origin.

\# **Step 8**:

Checkout to local master branch.

Merge "branch-1" with master local and then push to master origin.

Comment: You will notice now that all changes from "branch-1" are in the master, so they are both in sync.

\# **Step 9**:

Create a new branch "branch-2", with the following files:

-assets<br/>
--js<br/>
---script1.js<br/>

\# **Step 10**:

Commit new files and push changes to origin.

\# **Step 11**:

Checkout master and see if the new file is present.

Comment: the file is not be present since the new file is only at the "branch-2".

\# **Step 12**:

Add new content to the index.html in the master.

\# **Step 13**:

Checkout to "branch-2" and merge with master to load all changes from master.

Comment: at this point we still won't see the new file since we are syncing master onto "branch-2" not the other way. This needs to be done before pushing any changes to master (just like an svn update).

Checkout to master and merge with "branch-2" so we have the new files.

Comment: now "branch-2" and master are in sync but "brunch-1" is behing. This is acceptable since you should remove any branch once you merge with the master.


# Conclusion

This was a small example on how to work with branches in git, as you see the sort call "magic" that git does with keeping the files from one branch to another is visible here.

Hope you enjoy it!