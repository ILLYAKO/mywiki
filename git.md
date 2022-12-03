Helpful info about git.

Problem:
I have created a new project and tried to push it to GitHub. Git requested a username and password. My regular password was rejected because GitHub changed the password strategy and asked for personal access token instead.

Solution:
Creating the personal access token
1. Login GitHub account
2. Click on your profile icon in the upper-right corner and choose Setting
3. Go to Developer settings
4. Click Personal access tokens -> Tokens (classic)
5. Select a Generate new token, then click Generate new token (classic).
6. Give the token name and token expiration 
7. Select the scope. it should be "repo"
8. Click Generate token, copy token, and save for next use.

The created token will be used instead of the password for the execution of the git command in the command line.

$ git clone https://github.com/USERNAME/REPO.git

Username: YOUR_USERNAME

Password: YOUR_TOKEN
