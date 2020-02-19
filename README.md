# Code reproducibility and sharing (in a nutshell)
Aarhus University, Denmakr. February 2020. E-mail [Jakob Assmann](j.assmann@bios.au.dk) or visit [jakobjassmann.wordpress.com](jakobjassmann.wordpress.com).
___
This is repository is intended as a super fast intorduction to code reproducibility and sharing. The main aim is to get you started as quickly as possible. By nature, the content is not intended to be a comprehensive discussion of the topic. If you would like to delve in deeper, I recommend you explore the web and scientific literature.

## Content
1. [What is code reproducibility? Why share your code?](#what-is-code-reproducibility?-why-share-your-code?)
2. [Getting started with git and GitHub (do it yourself)](#getting-started-with-git-and-github)
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

## Getting started with git and GitHub 

There are some excellent tools that can help you to manage, share and document your code. Here we focus on two of them:
- **git** - a programme that documents and tracks changes in your code for back up and collaboration.
- **GitHub** - a cloud-like platform that hosts code and data with tools that make collaborative coding easy.

### git

The programme **git** has become the de-facto standard for version control in open source software development. Installed on your computer, it tracks all changes to all files in any directory you tell it to. Handy if a change you made the week before is breaking your code and you want to go back, but also if multiple people simultaneous develop code. 

Knowing excactly when and who by a change to the code was made, **git** can merge changes to a file from different developers into one. To facilitate sharing, **git** can sync the changes tracked locally on your computer to a remote repository - a data store on a server. This can be a local server (at your univeristy) or a server on the web.  

### GitHub
The code sharing platform **GitHub** is the most popular platform for hosting **git** repositories. The free plan only allows you to create public repositories - visible to anoyne on the web. However, as a studnet / teacher you can join the [education programme](https://education.github.com/), which gives you free access to the 'Pro' plan with unlimited private repositories. 

In addition to hosting **git** repositories, **GitHub** has lot of little extras that make collaborative coding easier, these inlcude issue tracking, milestone setting etc. We will not go into these here, but I recommend you to check them out!

Recently, [GitLab](https://about.gitlab.com/) - an alternative to **GitHub** - has increased in popularity. Functionally they are the same, but **GitLab** allows you to make private repositories without signing up to an education programme. Good news: you can simply sing up to **GitLab** using your **GitHub** account!
