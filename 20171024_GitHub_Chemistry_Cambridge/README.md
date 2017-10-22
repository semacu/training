
<img align="right" src=images/labtocat.png width="200">

# An introduction to GitHub for chemists

- Date: 24th October 2017, 3 - 4pm
- Location: [Unilever Lecture Theatre, Department of Chemistry](https://www.google.co.uk/maps/place/Department+of+Chemistry,+University+of+Cambridge/@52.197861,0.1233163,17z/data=!3m1!4b1!4m5!3m4!1s0x47d87099683bd269:0xd9d90c335a84ddd!8m2!3d52.197861!4d0.125505), University of Cambridge, UK
- Sign up [here](https://www.training.cam.ac.uk/event/2307013)
- Please bring your laptop or mobile device if you'd like to follow the practical part
- All workshop materials are available here: http://tinyurl.com/2017githubchemistry
- *Refreshments will be provided*


## Overview

Are you interested in learning Git and GitHub to manage your code, manuscripts or research data? This introductory workshop will be covering the following:

- [Background and motivation](README.md#background-and-motivation)
- [What is Git? What is version control? What is GitHub?](README.md#what-is-git-what-is-version-control-what-is-github)
- [How can Git and GitHub be useful for you?](README.md#how-can-git-and-github-be-useful-for-you)
- [Practical session: working with Git and GitHub](README.md#practical-working-with-git-and-github)


## Background and motivation

- *A system to keep track and compare the history of changes made to your files (versions)*

- *A platform to share and showcase your work online with colleagues and beyond*

- *Team work often means unnecessary work for some:*
  - Many people working on the same file at the same time (you, your lab colleague, your group leader, collaborators abroad ...)
  - Multiple versions of it (e.g. research manuscript, computer script ...)

<p align="center">
<img src=images/finaldoc.gif width="600">
</p>

<p align="right">
(http://phdcomics.com/comics/archive_print.php?comicid=1531)
</p>

The lifetime of a project:
- Project v1
- Project v2
- Project v3
- ...
- Project v25
- ...


## What is Git? What is version control? What is GitHub?

[Git](https://git-scm.com/) is a **free and open source** *distributed version control system*, which allows you to:

- Create repositories to host your projects using the [command-line](https://en.wikipedia.org/wiki/Command-line_interface)
- Track changes in the files and folders within your repositories


Version control systems were originally created by groups writing software and code (e.g. Linux project), but can be used for any kind of files or projects.

<p align="center">
<img src=images/vcs.png width="800">
</p>

<p align="right">
(adapted from http://lhzuigao.com/309note.html)
</p>

Advantages of *distributed* over *centralised* version control systems involve:
- If the central repository (server) crashes, it could be recovered / backed up from any of the local repositories created by the researcher, collaborator or group leader.
- Each person can make changes to their local repositories *offline*. Then integrate their individual changes in the central repository (server) when connected *online*.

[GitHub](https://en.wikipedia.org/wiki/GitHub) is a web platform that allows you to upload and manage your local or central repositories online (Hub). It provides:

- A backup of your repositories
- A nice visual interface to your repositories
- A way to collaborate with others

Changes are identified by a number named the *revision number*. Each revision is associated with a *timestamp* and the person making the change. Revisions can be compared, restored, and with some types of files, merged.

There are other softwares for version control, e.g. subversion ([svn](https://en.wikipedia.org/wiki/Apache_Subversion)).


### Interfaces to Git and GitHub

- Via the command line using *git*
- Directly [online](http://github.com/)

<p align="center">
<img src=images/github_online.png width="800">
</p>

- Github [desktop](https://desktop.github.com/) (available for Mac and Windows)

<p align="center">
<img src=images/github_desktop.png width="800">
</p>

<p align="right">
(https://programminghistorian.org/lessons/getting-started-with-github-desktop)
</p>


### Public (free) and private repositories

A user has to create a GitHub account in order to create repositories:

- Public repositories are free, and can be browsed and downloaded by anyone.
- Private repositories have associated costs - see [pricing of plans](https://github.com/pricing). The developer plan costs $7/month but is free, if you are a [student / academic](https://education.github.com/pack).

There are alternatives to GitHub, e.g. [GitLab](https://about.gitlab.com/), which works similarly but uses a different strategy with free private repositories and cost plans for public ones.


### Markdown

GitHub uses Markdown, a language with plain text formatting syntax, to render pages online. See examples of Markdown syntax [here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).



## How can Git and GitHub be useful for you?

These are many ways how people use Git and GitHub. Here are some examples:

- To host and share your research outputs, software or training materials
  - Research slides by [Bérénice Batut](https://bebatut-slides.github.io/backofen_lab_retreat_04_17/#/).
  - The Balasubramanian laboratory [computational projects](https://github.com/sblab-bioinformatics).
  - The Bender group [GitHub page](https://github.com/BenderGroup).
  - The BWA software to align DNA sequences to reference genomes is available [here](https://github.com/lh3/bwa).

- To create websites
  - Using [GitHub pages]((https://pages.github.com/)) to create your personal research [website](http://mikelove.github.io/).
  - To distribute information about your courses and activities, e.g. the Statistics course in the University of British Columbia is hosted [here](http://stat545.com/index.html).
  
- To share the contents of a book
  - The Bioinformatics Data Skills [book](http://shop.oreilly.com/product/0636920030157.do) shares materials in a dedicated GitHub [page](https://github.com/vsbuffalo/bds-files).



## Practical: working with Git and GitHub

### Create a GitHub account

Demonstrate by creating an account for our data group, e.g. wolfson-data

- Profile
- Account
- Email
- Student developer plan


### Install Git




### Create a new repository directly online

Demonstrate using my account [semacu](https://github.com/semacu) or the newly created wolfson-data

- Modify README.md
- Markdown
- Commits


### Add collaborators to your repository

Demonstrate using my account [semacu](https://github.com/semacu) or the newly created wolfson-data

- If you are not the owner or a collaborator, fork, make changes and submit a submit a pull request to the owner


### Making changes locally: using git in the command line

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



## Additional reference materials

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

Videos:
- [Git & GitHub tutorial for Beginners](https://www.youtube.com/watch?v=3RjQznt-8kE&list=PL4cUxeGkcC9goXbgTDQ0n_4TBzOO0ocPR)

Websites:
- [git](https://git-scm.com/)
- [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)



## License

This work is distributed under a [CC-BY license](https://en.wikipedia.org/wiki/Creative_Commons_license). Anyone may copy, distribute, display and perform the work and make derivative works and remixes based on it only if they give the author attribution.

<p align="center">
<img src=images/UniversityCambridge_logo.png height="50"> <img src=images/CRUKCI_logo.jpg height="50"> <img src=images/Jisc_logo.png height="50"> <img src=images/WellcomeTrust_logo.jpg height="50">
</p>
