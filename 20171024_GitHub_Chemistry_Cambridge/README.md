
<img align="right" src=images/labtocat.png width="200">

## An introduction to GitHub for chemists

- Date: 24th October 2017, 3 - 4pm
- Location: [Unilever Lecture Theatre, Department of Chemistry](https://www.google.co.uk/maps/place/Department+of+Chemistry,+University+of+Cambridge/@52.197861,0.1233163,17z/data=!3m1!4b1!4m5!3m4!1s0x47d87099683bd269:0xd9d90c335a84ddd!8m2!3d52.197861!4d0.125505), University of Cambridge, UK
- Sign up [here](https://www.training.cam.ac.uk/event/2307013)
- Please bring your own laptop or mobile device to follow the practical part
- All workshop materials are available here: http://tinyurl.com/2017githubchemistry
- *Refreshments will be provided*


### Overview

Are you interested in learning Git and GitHub to manage your code and research data? This introductory workshop will be covering the following:

- Background and motivation
- What is Git? What is GitHub? What is version control?
- How can it be useful for you?
- Practical session: working with GitHub


### Background and motivation

Team work often means unnecessary work for some:

- Multiple versions of the same file (e.g. research manuscript)
- Many people working on it (you, your lab colleague, your group leader, collaborators abroad ...)

<p align="center">
<img src=images/finaldoc.gif width="600">
</p>



### What is Git? What is GitHub? What is version control?

[Git](https://git-scm.com/) is a free and open source *distributed version control system* that allows you:

- To track changes in files and folders
- To collaborate with others

<p align="center">
<img src=images/dvcs.png width="800">
</p>


[Github](https://en.wikipedia.org/wiki/GitHub) is a web platform that allows you to upload and manage your repositories online.

Changes are identified by a number named the *revision number*. Each revision is associated with a *timestamp* and the person making the change. Revisions can be compared, restored, and with some types of files, merged.

Version control systems are frequently used for groups writing software and code, but can be used for any kind of files or projects.

Another software for version control is subversion ([svn](https://en.wikipedia.org/wiki/Apache_Subversion)).


#### Interfaces to github

- Directly [online](http://github.com/)
- Via the command line using *git*
- Github [desktop](https://desktop.github.com/)


#### Public (free) and private repositories

A user has to create an account in order to contribute content to the site, but public repositories can be browsed and downloaded by anyone.

Pricing of plans for [private repositories](https://github.com/pricing). Developer plan costs $7/month but is free, if you are a [student](https://education.github.com/pack).

There are alternatives to github, e.g. [gitlab](https://about.gitlab.com/), which uses a different business model with free private repositories and cost plans for public ones.


#### Features

General:

- Documentation
- Issues
- Pull requests
- History of commits
- Email notifications
- Github pages

Social-network like:

- Wikis
- Feeds
- Followers


#### Markdown

Github uses markdown, a lightweight markup language with plain text formatting syntax, to render pages. See examples of markdown syntax [here](https://en.wikipedia.org/wiki/Markdown)



### How can it be useful for you?

These are several ways how people use github:

#### To release and distribute software

e.g. Heng Li's software package for mapping DNA sequences against a large reference genome, a.k.a [bwa](https://github.com/lh3/bwa)


#### To share contents of a book

e.g. Vince Buffalo shares the data discussed in his book Bioinformatics Data Skills [book](http://shop.oreilly.com/product/0636920030157.do) using a dedicated github [page!](https://github.com/vsbuffalo/bds-files)


#### To create your own personal website or the website for your course

e.g. Michael Love has created his own research [website](http://mikelove.github.io/) using the feature known as github [pages](https://pages.github.com/)

e.g. the Statistics course from the University of British Columbia is hosted in [GitHub](http://stat545.com/index.html).

#### To host slides and materials

e.g. Bérénice Batut uses github to share her research [slides](https://bebatut-slides.github.io/backofen_lab_retreat_04_17/#/)

also, I just started to use github to share materials from training [sessions](https://github.com/semacu/training) and [talks](https://github.com/semacu/talks)


#### To share the research code from your paper/thesis

Some groups release the computer code associated to a paper when manuscripts are published, e.g. a Balasubramanian's group recent [paper](https://www.nature.com/articles/s41525-017-0007-6?WT.feed_name=subjects_molecular-biology) and associated github [page](https://github.com/sblab-bioinformatics/epigenetics-of-glioblastoma).



### Practical: working with GitHub

#### Create a new GitHub account

Demonstrate by creating an account for our data group, e.g. wolfson-data

- Profile
- Account
- Email
- Student developer plan


#### Create a new repository directly online

Demonstrate using my account [semacu](https://github.com/semacu) or the newly created wolfson-data

- Modify README.md
- Markdown
- Commits


#### Add collaborators to your repository

Demonstrate using my account [semacu](https://github.com/semacu) or the newly created wolfson-data

- If you are not the owner or a collaborator, fork, make changes and submit a submit a pull request to the owner


#### Making changes locally: using git in the command line

Create a temporary directory:

```bash
cd /Users/martin03/Desktop
mkdir tmp
cd tmp
```

Tell git who you are (your github username) and what your email address is:

```bash
git config --global user.name "semacu"
git config --global user.email "sermarcue@gmail.com"
```

Clone github repository:

```bash
git clone https://github.com/semacu/test_today.git
cd test_today
```

Make a change to the README.md file using your text editor.

Check the change:

```bash
git status
```

Track the file and stage the changes:

```bash
git add README.md
git status
```

Commit changes:

```bash
git commit -a -m "made tomorrow's changes"
git status
```

Push changes to the online github repository:

```bash
git push origin master
```

Done. Now your changes have been made in your github repository



### Additional reference materials

Books:
- [Happy Git and GitHub for the useR](http://happygitwithr.com/)

Courses:
- [Software Carpentry workshops](https://software-carpentry.org/workshops/)
- [A Friendly Introduction to GitHub](https://kirstiejane.github.io/friendly-github-intro/)
- [A quick introduction to Git and GitHub](http://www.datacarpentry.org/semester-biology/materials/git-in-30-minutes/)
- [Version Control with Git](https://swcarpentry.github.io/git-novice/)
- [Git Intro for Librarians](http://data-lessons.github.io/library-git/)

Papers:
- Perez-Riverol et *al.* [Ten Simple Rules for Taking Advantage of Git and GitHub](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004947)

Websites:
- [git](https://git-scm.com/)
- [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)



### License

This work is distributed under a [CC-BY license](https://en.wikipedia.org/wiki/Creative_Commons_license). Anyone may copy, distribute, display and perform the work and make derivative works and remixes based on it only if they give the author attribution.

<p align="center">
<img src=images/UniversityCambridge_logo.png height="50"> <img src=images/CRUKCI_logo.jpg height="50"> <img src=images/Jisc_logo.png height="50"> <img src=images/WellcomeTrust_logo.jpg height="50">
</p>
