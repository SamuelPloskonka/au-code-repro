# Code reproducibility and sharing (in a nutshell)
Aarhus University, Denmark. February 2020. E-mail [Jakob Assmann](j.assmann@bios.au.dk) or visit [jakobjassmann.wordpress.com](jakobjassmann.wordpress.com).
___
This is repository provides a super fast intorduction to code reproducibility and sharing. The main aim is to get you started as quickly as possible. By nature, the content is not intended to be a comprehensive discussion of the topic. If you would like to delve in deeper, check out the web and bountiful scientific literature.

## Content
1. [What is code reproducibility? Why share your code?](#what-is-code-reproducibility?-why-share-your-code?)
2. [git and GitHub](#git-and-github)
3. Documenting your code: metadata and in-line comments (#metadata-and-documenting-your-code)
4. Publishing data and 

## What is code reproducibility? Why share your code?
Reproducibility in science is a complex topic and goes to the the core of scientific philosophy.[Goodman et al. 2016](https://doi.org/10.1126/scitranslmed.aaf5027) recent(ish) discussion on the subject in *Science Translational Medicine* is an excellent starter, but you will find plenty of other good reading out there.

Simply put, the key idea behing code reproductibility is to ensure that your process of getting from your raw data to your results is as transparent as possible. Ideally, any interested researcher should be able to conduct your statistical analysis and re-create your figures, tables and outputs simply by downloading your data and running your code. 

If you managed to produce reproducible code, you will not only allow other researchers to fully judge the quality of your findings, but you also give the scientific community a chance to build on the hard work that you have done.

There are many more good reasons to share your code and to make sure it is as well documented as possible:
- You would like to share code with friends, colleagues or collaborators working on a joint project.
- You're producing work for a journal or funding body that requires open access to all data and code.
- In ten years time (or sooner) you look back at your work, but you may have forgotten what you did.
- ...

## git and GitHub 

There are some excellent tools that can help you to manage, share and document your code. We focus on two of them:
- **git** - a programme that documents and tracks changes in your code for back up and collaboration.
- **GitHub** - a cloud-like platform that hosts code and data with tools that make collaborative coding easy.

### git

The programme **git** has become the de-facto standard for version control in open source software development. Installed on your computer, it tracks changes to all files in any directory you tell it to. Handy if a change you made the week before is breaking your code and you want to go back, but also if multiple people work on the code. 

Knowing excactly when and who made a change to the code, **git** can merge changes to a file from different developers into one. To further facilitate sharing, **git** can sync the changes made locally on your computer to a remote repository. This repository can be on a local server (e.g. at your univeristy) or on a server on the web.  

### GitHub
The code sharing platform **GitHub** is the most popular platform for hosting **git** repositories. The free plan only allows you to create private repositories with a maximum of three colaborators. But as a student / teacher you can join the [education programme](https://education.github.com/), which gives you free access to the 'Pro' plan with unlimited private repositories. 

In addition to hosting **git** repositories, **GitHub** has lot of extras that make collaborative coding easier, these inlcude issue tracking, milestone setting etc. We will not go into these here, but I recommend you to check them out!

Recently, [GitLab](https://about.gitlab.com/) - an alternative to **GitHub** - has increased in popularity. Functionally they are the same, but **GitLab** allows you to make private repositories without signing up to an education programme. Good news: you can simply log on to **GitLab** using your **GitHub** account. So pick your choice!

## Let's get going with git and GitHub!

From here on I'll assume that you're mainly coding for statistical purposes using R in R Studio, and that both as well as [git](https://git-scm.com/downloads) are fully set up on your computer.

You will have to complete the following tasks:
- Task 1: 

### Task 1: Create a repository and clone it to your computer!
Create your own repository by copying this one:

1. On this website click the *green* 'Use this template' button (maybe by opening it in a new window / tab).
2. Give the repostiory a name and decide whether you would like it to be public or private.

Clone the content of the repository to your local computer:

  1. On the main page of your new repostiory (which will should exactly like this, except for the new repository name), click the 'Clone or Download' button in the top right.
  2. Copy the **HTTPS repository url** to the clipboard.
  3. Open RStudio.
  4. Create a 'New Project', select 'Version Control' and 'Git', paste the **HTTPS repository url** into the relevant field and specify the local directory where you want the project to be saved. Finish by clicking 'Create Project'.
  5. Enter your GitHub username and password if you're doing this for the first time.
 
Well done! You have created and cloned your first repository using a template. You could have also created an empty one from scratch (try it out later!), but for now having some content in the 'repo' will speed things up.

**Important:** When you clone a repository to your local computer, **git** will automatically track any changes made to files in the local folder.

### Task 2: Make some changes!

This repo - a common short for repository - is populated with a couple of R scripts in the /scripts folder, a CSV file containing some numbers in the /data folder, and a plot output in the /plots folder. Make a change to one of the R scripts!

1. Open one of the two R scripts in RStudio.
2. Change something! (e.g. add an in-line comment, or change a number).
3. Save the file.

After saving the file **git** will automatically notice that you have changed the file. You can see that it appeared in the 'Git' pane on the top right of the RStudio default view. If you can't see the pane bring it to focus via 'View' -> 'Show Vcs'. Let's look what happened there:

1. Hilight the file you changed in the RStudio 'Git' pane with a single click.
2. Press the 'diff' button in the top-left of the 'Git' pane.

A new window will open that highlights the changes you have made. Now, for now **git** has only noticed that you have made a change, but the change has not been logged. The file is saved locally on your harddrive, but the **git** is waiting for you to confirm the change. This gives you the opportunity to make further changes to the file if you want to. 

Once you're satisfied with the change you have made you need to 'commit' the change. Good news: you can commit changes for a single file or multiple files at once. However, you will always have to add a short message to the commit that briefly explains the changes you have made. **Git** will get angry at you if you don't add a message (try it out).

Commit your change: 

1. Click the little checkbox next to the file you have changed.
2. Add a message in the 'Commit message' box. (keep it short and informative).
3. Press the 'Commit' button.

Your changes are now commited (logged) by git.

### Task 3: Sync (push/pull) to GitHub

Once you have commited your changes they're logged on your local computer, but the changes have not been synced with your remote repository on **GitHub** yet. To update the remote repostiory we need to 'push' our changes:

1. Push the changes by pressing the 'Push' button in the 'RStudio: Review Changes' window or in the RStudio 'Git' pane.
2. Follow the flow and check out the messages. You might have to enter your GitHub account name and password again.

To check that your changes have been pushed you can navigate to the file you changed on GitHub and view it. *GitHub* also has a nice way of visualising the change history of a file. When you have opened the file on **GitHub** you can click 'History' button and you will see all commits that have affected the file. If you click on the commit code you will see the changes made for that commit.

### Task 4: Invite a collaborator to your GitHub repository

It's time to collaborate! You will need a friend for this. :)

1. Ask your neighbour (if you are at the workshop) or a friend for their **GitHub** account name.
2. On the **GitHub** repository website, go to 'Settings' in the top panel of your repository overview.
3. Click on 'Manage access'.
4. Click on 'Invite a collaborator'.

Your neighbour will get an email with an invite to collaborate. They will have to click the link to accept the collaboration.

### Task 5: Simultaneously edit a file!

First, sync a change between computers:

1. With your neighbour / friend, decide on one of you to clone the others repository to their local computer.
2. Decide on a file to change.
3. Make a change to the file on one of your computers, save, commit and push the change.
4. Pull the changes to the other computer.

Easy right!? Now let's repeat the exercise but this time both of you edit the file at the same time.

1. Make sure you have both pulled the latest changes from the repo.
2. Both of you make a change to the same file (start by editing different lines first).
3. Save, commit and push first on one, then on the second computer.

You might get an error message when pushing on the second computer.




