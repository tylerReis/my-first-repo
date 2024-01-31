On Github select the repository you would like to clone and select the https url.
On your local git, clone the repo with the following command
git clone <https_url_to_repo_from_github>
Remove the remote branch on your local git
git remote rm origin
Create a new repo on github and ensure NOT TO CREATE A README with this repo. This repo should return an https url for the repo. Copy this url origin.
Add the new https origin from your newly created repo onto your local git
git remote add origin <https_url_from_new_repo>
Add, commit, and push any changes onto your own github
git add .
git commit -m 'init'
git push origin <main/master>

below is used to add a new remote:

git remote add origin git@github.com:User/UserRepo.git
below is used to change the url of an existing remote repository:

git remote set-url origin git@github.com:User/UserRepo.git
below will push your code to the master branch of the remote repository defined with origin and -u let you point your current local branch to the remote master branch:

git push -u origin main