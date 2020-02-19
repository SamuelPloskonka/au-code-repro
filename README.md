# Code reproducibility and sharing in a nutshell
Aarhus University, Denmakr. February 2020. Contact: [Jakob Assmann](j.assmann@bios.au.dk): [jakobjassmann.wordpress.com](jakobjassmann.wordpress.com).
___
This is repository is intended as a super fast intorduction to code reproducibility and sharing. The main aim is to get you started as quickly as possible, by nature the content is therefore not intended to be a comprehensive discussion of the topic. If you would like to delve-in deeper, I recommend you explore the web and scientific literature on the topic.

## Content
1. What is code reproducibility? Why share your code?
2. [Getting started with git and GitHub (do it yourself)](#getting-started-with-git-and-github)
3. Documenting your code: metadata and in-line comments (#metadata-and-documenting-your-code)
4. Publishing data and 

## What is code reproducibility? Why share your code?
Reproducibility in science is a complex topic and goes to the the core of scientific philosophy. I think [Goodman et al. 2016]() recent(ish) discussion on the subject in *Science Translational Medicine* is an excellent starter, but you will find plenty of other good reading out there.

Simply put, the key idea behing code reproductibility is to ensure that your process of getting from your raw data to your results is as transparent as possible. Ideally, any other interested researcher should be able to conduct your statistical analysis and re-create your figures, tables and model outputs simply by downloading your data and running your code. 

If you managed to produce reproducible code, you will not only allow other researchers to fully judge the quality of your findings, but you also give the scientific community a chance to develop further on the hard work that you have done.

There are many more good reasons to share your code and to make sure it is as well documented as possible:
- You would like to share code with friends, colleagues or collaborators for a joint project.
- You're producing work for a journal or funding body that requires open access to all data and code.
- In ten years time (or sooner) you might want to look back at your work, but you may have forgotten what you did.
- ...

## Getting started with git and GitHub 
There are many excellent tools that can help you to manage, share and document your code. Today we will focus on two of them: **git** - a programme that helps you document and keep track of changes in your code and allow multiple people to work simultaneously on a coding project; and **GitHub** - a cloud-like platform that can host code and data with many little extras and gadgets that make collaborative coding easy.

The version control programme git has become a de-facto standard in the open source software development. Installed and engaged on your computer, it keeps track of all changes to all files in any directory you tell it to. This is super handy if you realise that a change you made a week before is actually breaking your code and you want to revert back - git will have a continous back up. But it also makes simultatneous code development amongst multiple people possible as it knows excactly who made what change and when, so it can merge files from different developers into one. 

The code sharing platform GitHub is the most popular type of its kind on the web.  
