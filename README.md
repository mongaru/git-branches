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

Create brach called "branch-1"

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

Merge "branch-1" with master local and then push to master origin.



branch 2
    css
        style2.css

ver master - si se ven los archivos
volver a branch

merge 2

branch 3
    js
        script1.js

master
    index.html

ver master - si se ven los archivos
volver a branch

merge 3