# Code reproducibility and sharing (in a nutshell)
Aarhus University, Denmark. February 2020. E-mail [Jakob Assmann](j.assmann@bios.au.dk) or visit [jakobjassmann.wordpress.com](jakobjassmann.wordpress.com).
___
This is repository provides a super fast intorduction to code reproducibility and sharing. The main aim is to get you started as quickly as possible. By nature, the content is not intended to be a comprehensive discussion of the topic. If you would like to delve in deeper, I recommend you explore the web and scientific literature.

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

## Let's get going!
From here on I'll assume that you're an ecologist and that you're mainly coding for statistical purposes using R in R Studio, and that both together with [git](https://git-scm.com/downloads) are fully set up on your computer.
### Task 1: Create a repository and clone it to your computer
Start by creating your own repository by copying this one:

1. On this website click the *green* 'Use this template' button (maybe by opening it in a new window / tab).
2. Give the repostiory a name and decide whether you would like it to be public or private.
3. 'Clone' the content of the repository to your local computer
    1. On the main page of your new repostiory (which will look exactly like this, except for your new name), click the 'Clone or Download' button in the top right.
    2. Copy the HTTPS url to the clipboard.
    3. Open RStudio.
    4. Click 'New Project', then select 'Version Control' and 'Git', paste the HTTPS repository url into the relevant field and specify the local directory where you want the project to be saved. Finish by clicking 'Create Project'.
    5. Enter your GitHub username and password if you're doing this for the first time.
 
Well done! You have cloned your first repository. You could have also created an empty one from scratch (try it out later), but for now having some content in the 'repo' will speed things up.

### Task 2: Make some changes
 
