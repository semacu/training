# An introduction to GitHub

- Date: 10th July 2017, 6-7pm
- Location: Room [Plommer A](http://www.wolfson.cam.ac.uk/plommer-house), [Wolfson College](http://www.wolfson.cam.ac.uk/), University of Cambridge, UK
- Series: Data Science [Group](https://www.facebook.com/groups/395500144179243/), Wolfson College, University of Cambridge, UK



## Overview

- What is git? What is github? What is version control?
- How can it be useful for you?
- Practical: working with github



## What is github? What is git? What is version control?

[Github](https://en.wikipedia.org/wiki/GitHub) is a free and open source platform that can help you build projects that are collaborative, well documented, and version-controlled. In practical terms, it is a web-based git:

- git: version control system that enables you to store a set of files, as well the list of changes made to those files (https://git-scm.com/).
- web-based: internet hosting service

Changes are usually identified by a number named the *revision number*. Each revision is associated with a *timestamp* and the person making the change. Revisions can be compared, restored, and with some types of files, merged.

Version control systems are frequently used for groups writing software and code, but can be used for any kind of files or projects.

Another software for version control is subversion ([svn](https://en.wikipedia.org/wiki/Apache_Subversion)).


### Interfaces to github

- Directly [online](http://github.com/)
- via the command line using *git*
- Github [desktop](https://desktop.github.com/)


### Public (free) and private repositories

A user has to create an account in order to contribute content to the site, but public repositories can be browsed and downloaded by anyone.

Pricing of plans for [private repositories](https://github.com/pricing). Developer plan costs $7/month but is free, if you are a [student](https://education.github.com/pack).

There are alternatives to github, e.g. [gitlab](https://about.gitlab.com/), which uses a different business model with free private repositories and cost plans for public ones.


### Features

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


### Markdown

Github uses markdown, a lightweight markup language with plain text formatting syntax, to render pages. See examples of markdown syntax [here](https://en.wikipedia.org/wiki/Markdown)



## How can it be useful for you?

These are several ways how people use github:

### To release and distribute software

e.g. Heng Li's software package for mapping DNA sequences against a large reference genome, a.k.a [bwa](https://github.com/lh3/bwa)


### To share contents of a book

e.g. Vince Buffalo shares the data discussed in his book Bioinformatics Data Skills [book](http://shop.oreilly.com/product/0636920030157.do) using a dedicated github [page!](https://github.com/vsbuffalo/bds-files)


### To create your own personal website

e.g. Michael Love has created his own research [website](http://mikelove.github.io/) using the feature known as github [pages](https://pages.github.com/)


### To host slides and materials

e.g. Bérénice Batut uses github to share her research [slides](https://bebatut-slides.github.io/backofen_lab_retreat_04_17/#/)

also, I just started to use github to share materials from training [sessions](https://github.com/semacu/training) and [talks](https://github.com/semacu/talks)


### To share the research code from your paper/thesis

Some groups release the computer code associated to a paper when manuscripts are published, e.g. a Balasubramanian's group recent [paper](https://www.nature.com/articles/s41525-017-0007-6?WT.feed_name=subjects_molecular-biology) and associated github [page](https://github.com/sblab-bioinformatics/epigenetics-of-glioblastoma).



## Practical: working with github

### Create a new github account

Demonstrate by creating an account for our data group, e.g. wolfson-data

- Profile
- Account
- Email
- Student developer plan


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



## Wolfson College Data Science Group

Sign-up to our mailing list [here](https://lists.cam.ac.uk/mailman/listinfo/wolfson-data).



## Future events

List of upcoming meetings [here](https://docs.google.com/spreadsheets/d/1VGasQb0IFDW6XBjAb3bHQLmbZ5f2KtHChJ9taq3ngcM/edit#gid=0).



## License

This work is distributed under a [CC-BY license](https://en.wikipedia.org/wiki/Creative_Commons_license). Anyone may copy, distribute, display and perform the work and make derivative works and remixes based on it only if they give the author attribution.



## References and materials

Books:

- [Bioinformatics Data Skills](http://shop.oreilly.com/product/0636920030157.do), Reproducible and Robust Research with Open Source Tools, Chapter 5: Git for Scientist. Book's GitHub [page](https://github.com/vsbuffalo/bds-files)
- Happy Git and GitHub for the useR [book](http://happygitwithr.com/)


Courses:

- A Friendly Github Intro Workshop:
	- [Materials](https://kirstiejane.github.io/friendly-github-intro/)
	- Links to [course1](https://training.cam.ac.uk/event/2118546) and [course2](https://training.cam.ac.uk/event/1878054)

- Revision Control with Git [course](https://training.cam.ac.uk/event/1948859)



## TODO

- Include Octocat in intro
- Include CC-By icon
