# Intro Tutorial

TERMS
https://training.github.com/downloads/github-git-cheat-sheet.pdf

- Commit: A change to a file/set of files. For example, you can make a branch, make changes, commit the change, then propse the change be added to the 
main branch with a pull request.
- Branch: A lightweight moveable pointer to a commit. Allows you to fix bugs and experiment with new ideas in a contained area of your repository. 
For example, a collaborator for a project can make changes on a branch, then make a pull request so changes are added to the main branch. 
The branch can then be deleted.
- Clone: A local version of a repository including all commits and branches. 
- Fork: Copy of a repository on GitHub owned by a different person. 
- Pull Request: A place to compare and discuss the differences introduced on a branch with reviews, comments, integrated tests, and more. 


CREATING A PERSONAL ACCESS TOKEN
https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token
Make sure you have verified you email address. 
1. Click on your profile photo
2. Go to settings
3. From the left side bar, click on "< > Developer Settings"
4. From the left side bar, click on "Personal access tokens"
5. Generate a new token and give it a name
6. Pick and expiration for the token
7. Check off the permissions you want to grant the token. If you will be using this to access repositories from the command line, make sure you check "repo"
8. Generate Token
*Tokens are like password so keep them secret*

When performing Git operations over HTTPS, use the token as the password. 
example:
$ git clone https://github.com/username/repo.git
Username: [your username]
Password: [your token]


CREATE A NEW DIRECTORY AND TURN IT INTO A GIT REPOSITORY
https://training.github.com/downloads/github-git-cheat-sheet.pdf
1. Create a new folder with the following command (skip this step if you are using an existing folder):
$ mkdir NewDirName
2. cd into the folder and turn it into a git repository with the following command:
$ git init


ADD A FILE TO YOUR REPOSITORY THROUGH THE COMMAND LINE
https://training.github.com/downloads/github-git-cheat-sheet.pdf
1. cd into your git repository folder
2. Clone your repository to get a copy on your local computer. 
To find the URL, go to the repository on GitHub, click the green "Code" button and copy the https link
$ git clone [URL]
3. In the command line, cd into the clone. 
4. Create the new file any way you like. For example, you can use echo:
$echo "This is the new file" > NewFileName
5. $ git add .
6. $ git commit -m "Add a new file"
7. $ git push origin main (or other branch name)
