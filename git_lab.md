# Week 1: Git/Github Lab
![Image of Github Octopus](http://www.storybench.org/wp-content/uploads/2015/09/github-octocat-1200x806.jpg)

## Create A Github Account
1. Go to https://github.com/
2. Click "Sign Up for Github"
3. Follow steps to create your Github account

## Setup Github Desktop
1. Download Github desktop: https://desktop.github.com/
2. Once installation completes, sign in with your new account

## Create A Github Repository (aka repo) for your final project
1. Go to https://github.com/
2. Sign in with your account
3. Click "New Repository"
4. Use a informational repository name and description
5. Choose "Private"
6. Check "Initialize this repository with a README"
7. Click "Create Repository"

## Import Your Repo to Github Desktop
1. On your repo web page (github.com/<account_name>/<repo_name>), click "Clone or Download"
2. Copy the web URL
3. Open Github Desktop
4. Click "File -> Clone Repository"
5. Use the web URL from step #2 (and local path should be automatically created for you)
6. Click "Clone"

## Create A Development Branch
1. (Option A) open Github Desktop, click "Branch -> New Branch", enter "develop" as the new branch name
2. (Option B) go to your repo web page, click "Branch: master", enter "develop" in the textbox, click "Create branch: develop"
3. **Best practice: you should use `develop` branch for code development and testing, and once all code on `develop` branch is well tested and ready-to-run, create a pull request (which will appear in later section) to merge code from `develop` branch to `master` branch**

## Add GWC Logo and Commit via Github Desktop
![Image of GWC](https://upload.wikimedia.org/wikipedia/commons/a/a1/GWC_logo_2016_.png)
1. What is **commit**: a commit is a collection of changes to be made together, like a save point or a check point in video games :D
2. Switch current branch to `develop` on Github Desktop (*if you cannot find `develop` branch, click "Fetch origin" to sync with Github server*)
3. Create a folder called "images" under your repo's local path (where all files of your repo are stored on your local desktop/laptop)
4. Download the GWC logo above to the images folder you just created 
5. Go to Github Desktop, you should see the GWC logo file appears as a change
6. Use "Summary" textbox to summarize the changes you made (e.g. Upload GWC logo imagine file)
7. Use "Description" textbox to give more details of your changes (e.g. This logo will be used in README.md)
8. Click "commit to develop"
9. Now you have *saved* your change as a commit **locally**, and nobody else can see this change yet until you *sync* with Github server.
10. Click "Pull origin" to sync with Github server
11. Now your change is global! Check your repo web page to find the GWC logo imagine file under images folder!

## Learn about Markdown and Commit via Github Web
1. On your repo page (github.com/<account_name>/<repo_name>), switch to `develop` branch, click "README.md"
2. Click the pencil icon to edit README.md (a Markdown file)
3. Refer to [Mastering Markdown](https://guides.github.com/features/mastering-markdown/) to add following items to your README.md:
   1. Add GWC logo under the main title
   2. Add your name in bold (e.g. Repository Owner: **Xinran Waibel**)
   3. Add a hyperlink to [Girls Who Code website](https://girlswhocode.com/)
   4. Explore Markdown formatting syntax and add whatever is relavant to your project :D
4. Commit the changes you made to README.md to `develop` branch using "Commit changes" section at the bottom

## Create A Pull Request (PR)
1. Does your README.md look good? If YES, you are ready to merge your code from `develop` to `master`!
2. Go to your repo web page, click "New Pull Request"
3. Select `master` as base branch, and `develop` as compare branch
4. At the bottom of PR page, you will see a list of change that will be merged to `master` branch
5. Review code changes to be merged.
6. Give a description of code changes in this PR (e.g. Added repo owner and project information in README.md)
7. Click "Create pull request"
8. Click "Merge pull request"
9. Click "Confirm merge"
10. Go to your repo web page, the images folder and your changes to README is in `master` branch now!

## Add TAs As Collaborators
1. Since your repo is private, others cannot see your repo unless your explicitly add them as collaborators
2. On your repo web page, click "Settings"
3. Click "Collaborators"
4. Type xinranduan in the textbox
5. Click "Add collaborator"
6. Now Julina can view your repo! Next, add Yiwen as a collaborator.

## Fork `GWC_UMN_FALL_2018` Repo to Add Your Contact Info
1. What is **fork**: fork allows you to create a clone of someone else's Github repo. Since the forked repo still links back to the original repo, you can create PRs later to merge changes on the forked repo to the original repo.
2. Go to https://github.com/xinranduan/GWC_UMN_FALL_2018
3. Click "Fork"
4. On the forked repo web page, edit the README.md to add your information under "Students" section
5. Create a PR to merge changes to the original repo (hint: base branch is `xinranduan/GWC_UMN_FALL_2018/master` and compare branch is `<your_account_name>/GWC_UMN_FALL_2018/master`)
6. Wait for me to merge your PR
