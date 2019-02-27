# How-to-do-stuff
This is how-to page to explain how to "push" an eclipse Project to gitHub


- First > download git from http://git-scm.com/ </br>
- Then go to http://github.com/ and create an account and repository.

On your machine:
1. Navigate to the project folder (git bash)
2. Then :   git init    - in order to initiate a new git repository in that directory
3. Register that new repo with a remote (where you'll upload -- push -- your files to), 
   which in our case is github. You'll get the correct URL from your repo on GitHub.
$ git remote add origin https://github.com/[username]/[reponame].git
4. Add your existing files to your local commit:
git add .   # this adds all the files
5. Make an initial commit:
git commit -a -m "Initial commit" # this stages your files locally for commit. 
                                  # they haven't actually been pushed yet
Now you've created a commit in your local repo, but not in the remote one. 
To put it on the remote, you do the second line you posted:
git push -u origin --all

