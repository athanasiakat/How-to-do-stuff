# How-to-do-stuff
This is how-to page to explain how to "push" an eclipse Project to gitHub


- First > download git from http://git-scm.com/ </br>
- Then go to http://github.com/ and create an account and repository.
</br>
On your machine:
1. Navigate to the project folder (git bash)
2. Then :   <b> git init </b>   - in order to initiate a new git repository in that directory
3. Register that new repo with a remote (where you'll upload -- push -- your files to), 
   which in our case is github. You'll get the correct URL from your repo on GitHub.
<b> $ git remote add origin https://github.com/[username]/[reponame].git </b>
4. Add your existing files to your local commit:
<b>git add . </b>  # this adds all the files
5. Make an initial commit:
git commit -a -m "Initial commit" # this stages your files locally for commit. </br>
                                  # they haven't actually been pushed yet</br>
Now you've created a commit in your local repo, but not in the remote one. </br>
To put it on the remote, you do the second line you posted:</br>
<b>git push -u origin --all</b>


___
Steps :
1.Right click on your eclipse project -> Team -> Share project
2. Choose git and then check the box asking create/use repository -> click on create repository and click finish. 
- This will create a local git repo. (Assuming you have already installed git  )
3. Right click on project -> Team -> Commit - Select only the files you want to commit and click on Commit. 
- Now the files are committed to your local repo.
4. Go to git repositories view in eclipse ( or Team -> Show in repositories View)
5. Expand the git repo of your project and Right click on Remotes -> Create Remote
Remote name will appear as origin, select 'Configure Push' Option and click ok
6.Click on change next to URI textbox and give your git url, username, password and click on 'Save and Push'. 
This configures git Push.
</br>
For configuring Fetch, go to Git Repositories -> Remote -> Configure Fetch -> Add -> Master Branch -> Next -> Finish -> Save and Fetch
</br>
For configuring Master Branch, Branch -> Local -> Master Branch -> Right click and configure branch -> Remote: origin and Upstream Branch : refs/heads/master -> click ok
