
<img align="right" src=images/IntroductionGitHubSlide.png width="225">

# An introduction to GitHub for chemists

- Date: 24th October 2017, 3 - 4pm
- Location: [Unilever Lecture Theatre, Department of Chemistry](https://www.google.co.uk/maps/place/Department+of+Chemistry,+University+of+Cambridge/@52.197861,0.1233163,17z/data=!3m1!4b1!4m5!3m4!1s0x47d87099683bd269:0xd9d90c335a84ddd!8m2!3d52.197861!4d0.125505), University of Cambridge, UK
- Sign up [here](https://www.training.cam.ac.uk/event/2307013)
- Please bring your laptop or mobile device if you'd like to follow the practical part
- All workshop materials are available here: 
http://tinyurl.com/2017githubchemistry
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
  - Many people working on the same file at the same time (you, your lab colleague, your group leader, collaborators abroad ...).
  - Multiple versions of it (e.g. research manuscript, computer script ...).

<p align="center">
<img src=images/finaldoc.gif width="600">
</p>

<p align="right">
(http://phdcomics.com/comics/archive_print.php?comicid=1531)
</p>

Mood during the lifetime of a project:
- v1 :smile:
- v2 :wink:
- v3 :expressionless:
- ... :pensive:
- v25 :sob:
- ... :scream:


## What is Git? What is version control? What is GitHub?

[Git](https://git-scm.com/) is a **free and open source** *distributed version control system*, which allows you to:

- Create repositories to host your projects using the [command-line](https://en.wikipedia.org/wiki/Command-line_interface).
- Track changes in the files and folders within your repositories.


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

- Via the command-line using *git*

<p align="center">
<img src=images/git_commandline.png width="600">
</p>

- Directly [online](http://github.com/)

<p align="center">
<img src=images/github_online.png width="800">
</p>

- Github [Desktop](https://desktop.github.com/) (available for Mac and Windows)

<p align="center">
<img src=images/github_desktop.png width="800">
</p>

<p align="right">
(https://programminghistorian.org/lessons/getting-started-with-github-desktop)
</p>


### Public (free) and private repositories

A user has to create a GitHub account in order to create repositories:

- Public repositories are free, and can be browsed and downloaded by anyone.
- Private repositories have associated costs - see [pricing of plans](https://github.com/pricing). The developer plan costs $7/month but it is free if you are a [student / academic](https://education.github.com/pack).

There are alternatives to GitHub, e.g. [GitLab](https://about.gitlab.com/), which works similarly but uses a different strategy with free private repositories and cost plans for public ones. Other alternatives: [Bitbucket](https://bitbucket.org/).


### Markdown

GitHub uses Markdown, a language with plain text formatting syntax, to render pages online. See examples of Markdown syntax [here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).



## How can Git and GitHub be useful for you?

### Some examples

These are many ways how people use Git and GitHub.

- To host and share your research outputs, software or training materials
  - Research slides by [Bérénice Batut](https://bebatut-slides.github.io/backofen_lab_retreat_04_17/#/).
  - The Balasubramanian laboratory [computational projects](https://github.com/sblab-bioinformatics).
  - The Bender group [GitHub page](https://github.com/BenderGroup).
  - The source code of the BWA software, which aligns DNA sequences to reference genomes, is available [here](https://github.com/lh3/bwa).
  - The source code of the PIDGIN software, which predicts protein targets for drug-like molecules, is available [here](https://github.com/lhm30/PIDGINv2).

- To create websites
  - Using [GitHub pages]((https://pages.github.com/)) to create your personal research [website](http://mikelove.github.io/).
  - To distribute information about your courses and activities, e.g. the Statistics course in the University of British Columbia is hosted [here](http://stat545.com/index.html).
  
- To share the contents of a book
  - The Bioinformatics Data Skills [book](http://shop.oreilly.com/product/0636920030157.do) shares materials in a dedicated GitHub [page](https://github.com/vsbuffalo/bds-files).


### In the context of our research group

- Most projects have both an experimental and a computational leader
- Classical ways of sharing are: conversations/meetings, email, DropBox, common/shared folders ...
- An environment where:
  - Computational colleagues can share code and results, review work of others and get credit from their collaborative project work.
  - Experimental colleagues can follow development, access results and learn computational methods.

- Reproducibility in computational research to avoid situations like ...

<p align="center">
<img src=images/reproducibility.gif width="800">
</p>

<p align="right">
(http://phdcomics.com/comics.php?f=1689)
</p>

- A happier lifetime for a project:

<p align="center">
<img src=images/project_timeline.png width="800">
</p>

<p align="right">
(https://github.com/semacu/talks/tree/master/20170703_GitHubintheLab_CRUK-CI)
</p>



## Practical: working with Git and GitHub

- [Create a GitHub account](README.md#create-a-github-account) (+)
- [Create your first repository](README.md#create-your-first-repository) (+)
- [Explore your first repository and GitHub account](README.md#explore-your-first-repository-and-github-account) (++)
- [Making changes using Git in the command-line](README.md#making-changes-using-git-in-the-command-line) (+++)

### Create a GitHub account

- Go to https://github.com
- Fill in your **Username**, **Email** and **Password**. Then click on the green button "Sign up for GitHub".

<p align="center">
<img src=images/p1_1.png width="800">
</p>

- Choose your personal plan page. For now select "Unlimited public repositories for free". Then click on "Continue".

<p align="center">
<img src=images/p1_2.png width="800">
</p>

- Tailor your experience page. Choose the boxes that apply to you and click on "Submit". Otherwise, just go to "skip this step".

<p align="center">
<img src=images/p1_3.png width="800">
</p>

- You have created a GitHub account! :smile:



### Create your first repository

- If you are not already signed in, sign in to GitHub using the **Username/Email** and **Password** created before.
- Click on the top-right "avatar" icon and select "Your profile". Have a quick browse through your page.

<p align="center">
<img src=images/p2_1.png width="800">
</p>

- Click on the top-right "+" icon and select "New repository". **Verify your email address**. You should have just received an email from GitHub in the address provided above. Find this email and click on "Verify email address".

<p align="center">
<img src=images/p2_2.png width="400"> <img src=images/p2_3.png width="400">
</p>

- Create a new repository page. Fill in a "Repository name", e.g. my_first_repository or my_analysis_script. For now choose "Public" and select the box to initialize this repository with a README. Finally, click on "Create repository".

<p align="center">
<img src=images/p2_4.png width="800">
</p>

- You created your first repository! :rocket:



### Explore your first repository and GitHub account

#### Your first repository

- Click on **README.md** and go to the middle-right pencil "Edit this file". Type anything to change the file, e.g. "GitHub is fun!".

<p align="center">
<img src=images/p3_1.png width="800">
</p>

<p align="center">
<img src=images/p3_2.png width="800">
</p>

- Scroll down. Introduce a commit change message, e.g. "My first update", and select the radio button "Commit directly to the master branch". Then click on "Commit changes". Voilá!

<p align="center">
<img src=images/p3_3.png width="800">
</p>

- To view your **history of commits** for **README.md**, click on **README.md** and go to the middle-right "History" button.
- Alternatively, to view your **history of commits** for your first repository, click on the name of your repository and select the tab depicting a small clock and the number of commits next to it.

Bonus points:

- Try to create a new file
- In your new repository, have a look at the "Settings" tab, explore "Collaborators" and try to add the person sitting next to you.

#### Your GitHub account

- Click on your top-right "avatar" icon and select "Settings".

<p align="center">
<img src=images/p3_4.png width="800">
</p>

- Explore the tabs "Profile", "Account" and "Emails".


### Making changes using Git in the command-line

Install Git:


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



## Thanks for your attention! Enjoy GitHub! :octocat:

Feedback? Any other questions about the workshop/GitHub? Just email: sermarcue@gmail.com

## Additional reference materials

Books:
- [Happy Git and GitHub for the useR](http://happygitwithr.com/)

Courses:
- [GitHub On Demand Training](https://services.github.com/on-demand/)
- [Software Carpentry workshops](https://software-carpentry.org/workshops/)
- [A Friendly Introduction to GitHub](https://kirstiejane.github.io/friendly-github-intro/)
- [A quick introduction to Git and GitHub](http://www.datacarpentry.org/semester-biology/materials/git-in-30-minutes/)
- [Version Control with Git](https://swcarpentry.github.io/git-novice/)
- [Git Intro for Librarians](http://data-lessons.github.io/library-git/)

Help:
- GitHub [Help](https://help.github.com/)

Papers:
- Perez-Riverol et *al.* [Ten Simple Rules for Taking Advantage of Git and GitHub](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004947)

Videos:
- [GitHub Training & Guides](https://www.youtube.com/githubguides)
- [Git & GitHub tutorial for Beginners](https://www.youtube.com/watch?v=3RjQznt-8kE&list=PL4cUxeGkcC9goXbgTDQ0n_4TBzOO0ocPR)

Websites:
- [git](https://git-scm.com/)
- [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)



## License

This work is distributed under a [CC-BY license](https://en.wikipedia.org/wiki/Creative_Commons_license). Anyone may copy, distribute, display and perform the work and make derivative works and remixes based on it only if they give the author attribution.

<p align="center">
<img src=images/UniversityCambridge_logo.png height="50"> <img src=images/CRUKCI_logo.jpg height="50"> <img src=images/Jisc_logo.png height="50"> <img src=images/WellcomeTrust_logo.jpg height="50">
</p>
