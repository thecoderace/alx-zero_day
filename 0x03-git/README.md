# Project: 0x03. Git

## What is Git and GitHub?

Git is a mature, actively maintained open source revision control system used by thousands of developers around the world.

GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

## Learning Objectives

At the end of this project, you are expected to be able to [explain to anyone](https://fs.blog/feynman-learning-technique/?fbclid=IwAR2K5_BGPVo0QjJXkOIIqNsqcXK4lTskPWJvA0asKQIGtCPWaQBdKmj1Ztg), without the help of Google:

## General

* What is source code management
* What is Git
* What is GitHub
* What is the difference between Git and GitHub
* How to create a repository
* What is a README
* How to write good READMEs
* How to commit
* How to write helpful commit messages
* How to push code
* How to pull updates
* How to create a branch
* How to merge branches
* How to work as collaborators on a project
* Which files should and which files should not appear in your repo

# More Info

## Basic usage

At the end of this project you should be able to reproduce and understand these command lines:

```
$ git clone <repo>
$ touch test
$ git add test
$ git commit -m "Initial commit"
$ git push origin main
```
  
# Project Tasks:

## Create and setup your Git and GitHub account

Step 0 - Create an account on GitHub [if you do not have one already]
You will need a GitHub account for all your projects at ALX. If you do not already have a github.com account, you can create an account for free [here](https://github.com/)

Step 1 - Create a Personal Access Token on Github
To have access to your repositories and authenticate yourself, you need to create a Personal Access Token on Github.
You can follow [this tutorial](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) to create a token.
Once it’s created, you should have a token that looks like this:
![a449483cd76a72cef1b42df831e686c64faa1cf6](https://user-images.githubusercontent.com/117726036/221265787-6323ffcd-9a03-4989-8261-70dba7c68667.png)

Step 2 - Update your profile on the Intranet
Update your Intranet profile by adding your Github username

If it’s not done the Checker won’t be able to correct your work

<img width="909" alt="6270480a0a982cd1846b877eda2ee405d2e8f575" src="https://user-images.githubusercontent.com/117726036/221266711-d54b0aba-c88d-454d-a6d5-2d1548acafa9.png">

Step 3 - Create your first repository

Using the graphic interface on the [github website](https://github.com/), create your first repository.
* Name: `alx-zero_day`
* Description: `I'm now a ALX Student, this is my first repository as a full-stack engineer`
* Public repo
* No `README`, `.gitignore`, or license

<img width="740" alt="2340a2d0f7c74b5dd6f8fc2aa58f94d13ea2c775" src="https://user-images.githubusercontent.com/117726036/221267519-e4da6a7f-f620-4447-b55a-66f8fc464794.png">

Step 4 - Open the sandbox

On the intranet, just under the task, click on the button <img width="125" alt="9db8eece71455dfddf4b7d8585c037c535f1d18d" src="https://user-images.githubusercontent.com/117726036/221268970-76fe3451-804a-4840-aa55-0668f4456d25.png"> and `run` to start the machine.

Once the container is started, click on <img width="113" alt="be9d1fbfb3d97e6924a4d2af7df9290ad7ae77df" src="https://user-images.githubusercontent.com/117726036/221269042-87d3c71e-97c9-48f4-a14c-d542566f9dc1.png"> to open a shell where you can start work from.

Step 5 - Clone your repository

On the webterm of the sandbox, do the following:

* Clone your repository

```
root@896cf839cf9a:/# git clone https://{YOUR_PERSONAL_TOKEN}@github.com/{YOUR_USERNAME}/alx-pre_course.git                  
Cloning into 'alx-pre_course'...
warning: You appear to have cloned an empty repository. 
```

Replace {YOUR_PERSONAL_TOKEN} with your token from step 1

Replace {YOUR_USERNAME} with your username from step 0 and 1

Pro-Tip: On windows, use CTRL + A + V to paste in the web terminal

Step 6 - Create the `README.md` and push the modifications

* Navigate to this new directory. [Tips](https://askubuntu.com/questions/232442/how-do-i-navigate-between-directories-in-terminal)

```
root@896cf839cf9a:/# cd alx-pre_course/
root@896cf839cf9a:/alx-pre_course#
```

* Create the file `README.md` with the content `My first readme`. [Tips](https://forum.howtoforge.com/threads/echo-into-a-file.115/)

```
root@896cf839cf9a:/alx-pre_course# echo 'My first readme' > README.md                                                                 
root@896cf839cf9a:/alx-pre_course# cat README.md                                                                                      
My first readme  
```

* Update your git identity

```
root@896cf839cf9a:/alx-pre_course# git config --global user.email "you@example.com"
root@896cf839cf9a:/alx-pre_course# git config --global user.name "Your Name"
```

* Add this new file to git, commit the change with this message “My first commit” and push to the remote server / origin

```
root@896cf839cf9a:/alx-pre_course# git add .
root@896cf839cf9a:/alx-pre_course# git commit -m 'My first commit'
[master (root-commit) 98eef93] My first commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
root@896cf839cf9a:/alx-pre_course# git push                                                                                           
Enumerating objects: 3, done.                                                                                                         
Counting objects: 100% (3/3), done.                                                                                                   
Writing objects: 100% (3/3), 212 bytes | 212.00 KiB/s, done.                                                                          
Total 3 (delta 0), reused 0 (delta 0)                                                                                                 
To https://github.com/{YOUR_USERNAME}/alx-pre_course.git                                                                                       
 * [new branch]      master -> master     
```

Good job!

You pushed your first file in your `first repository` of the `first task` of your `first ALX School project`.

You can now check your repository on GitHub to see if everything is good.

## Repo-session

[alx-zero_day](./alx-zero_day) - Create a new directory called `0x03-git` in your `alx-zero_day` repo.

Make sure you include a non empty `README.md` in your directory:

* at the root of your repository `alx-zero_day`
* AND in the directory `0x03-git`

And important part: `Make sure your commit and push your code to Github - otherwise the Checker will always fail.`

## Coding fury road

[bash/alx](bash/alx), [bash/school](./bash/school), [c/c_is_fun.c](./c/c_is_fun.c), [js/main.js](./js/main.js), [js/index.js](./js/index.js) - For the moment we have an empty project directory containing only a `README.md`. It’s time to code!

* Create these directories at the root of your project: `bash`, `c`, `js`
* Create these empty files:
    * `c/c_is_fun.c`
    * `js/main.js`
    * `js/index.js`
* Create a file `bash/alx` with these two lines inside: `#!/bin/bash` and `echo "ALX"`
* Create a file `bash/school` with these two lines inside: `#!/bin/bash` and `echo "School"`
* Add all these new files to git
* Commit your changes (message: “Starting to code today, so cool”) and push to the remote server

## Collaboration is the base of a company

[bash/alx](./bash/alx), [bash/school](./bash/school), [bash/98](./bash/98) - A branch is like a copy of your project. It’s used mainly for:

* adding a feature in development
* collaborating on the same project with other developers
* not breaking your entire repository
* not upsetting your co-workers

The purpose of a branch is to isolate your work from the main code base of your project and/or from your co-workers’ work.

For this project, create a branch `update_script` and in this branch:

* Create an empty file named `bash/98`
* Update `bash/alx` by replacing `echo "ALX"` with `echo "ALX School"`
* Update `bash/school` by replacing `echo "School"` with `echo "The school is open!"`
* Add and commit these changes (message: “My personal work”)
* Push this new branch [Tips](https://docs.github.com/en/get-started/using-git/pushing-commits-to-a-remote-repository)

Perfect! You did an amazing update in your project and it’s isolated correctly from the `main` branch.

Ho wait, your manager needs a quick fix in your project and it needs to be deployed now:

* Change branch to `main`
* Update the file `bash/alx` by replacing `echo "ALX"` with `echo "ALX School is so cool!"`
* Delete the directory `js`
* Commit your changes (message: “Hot fix”) and push to the origin

Ouf, hot fix is done!

##  Collaboration: be up to date

[README.md](./README.md), [up_to_date](./up_to_date) - Of course, you can also work on the same branch as your co-workers and it’s best if you keep up to date with their changes.

For this task – `and only for this task` – please update your file `README.md` in the main branch from GitHub.com. It’s the `only time` you are allowed to update and commit from GitHub interface.

After you have done that, in your terminal:

* Get all changes of the main branch locally (i.e. your `README.md` file will be updated)
* Create a new file `up_to_date` at the root of your directory and in it, write the git command line used
* Add `up_to_date` to git, commit (message: “How to be up to date in git”), and push to the origin

## HAAA what did you do???

Collaboration is cool, but not really when you update the same file at the same time…

To illustrate that, please merge the branch `update_script` to `main`: “Cool, all my changes will be now part of the main branch, ready to be deployed!”

HHHHHHHAAAAAAAA

```
CONFLICT (content): Merge conflict in bash/alx
```

As you can see, you have conflicts between two branches on the same file.

Your goal now is to resolve conflicts by using the version of the branch `update_script`, and push the result to the origin.

At the end, you should have all your work from the branch `update_script` (new file and two updated files) and all latest `main` commits (new files, delete folder, etc.), without conflicts.

## Never push too much

[.gitignore](./.gitignore) - Create a `.gitignore` file and define a rule to never push `~` files (generated by Emacs). [Tips](https://git-scm.com/docs/gitignore)

