+++
title = 'prep'
description = 'You can use these notes to prepare for the first in-person session of the software development course'
layout = 'prep'
emoji= '📝'
menu_level = ['module']
weight = 1
backlog= 'Module-Induction'
backlog_filter= 'Induction'
+++

# Notes

## Learning objectives

Define a code base
Define a repository
Explain why we use Github
Given a remote or local repository, identify the number of commits
Given a remote or local repository, identify the author, time and message of a given commit
Given a remote or local repository, identify the files and folders from any commit in a version timeline
Describe the purpose of version control
Explain the difference between Git and Github
Get a local copy of a repository on your local machine
Given a local repository, make a local change and inspect the Source Control panel in VSCode
Given a local repository, make some local changes and commit those changes

## 📝 CYF blog

Imagine is someone is creating an educational content for a blog at CYF.

You can find a link to the blog here.

The blog is live here 👉 [CYF educational blog](https://git-demo-week1.netlify.app/)

{{<note type="definition" title="definition">}}
Live means an web application is up and running and available for use by users on the internet
{{</note>}}

{{<note type="exercise" title="exercise">}}
Try exploring the site above. Try clicking around different links on the site and check to see if they're working.
{{</note>}}

## 💾 Saving changes

You may have tried dealing with a project by creating multiple copies of a file. You may have ended up with something that looks like this.

Instead we can develop applications using different versions.

{{<note type="activity" title="activity">}}

Try explaining why we try the person above has tried to manage their file in this way. Describe some of the problems that occur when we try managing versions of a document in this way.

{{</note>}}

## Different versions

We have a need for a way of creating and managing different versions of our project over time.

{{<note type="exercise" title="exercise">}}

Here are some links to the different versions of the same CYF educational backlog

[Version A educational blog](https://64b6fd80d14d510008aab4aa--git-demo-week1.netlify.app)
[Version B educational blog](https://64b6f8e6044ccc0742386430--git-demo-week1.netlify.app/)
[Version C educational blog](https://64b6fd80d14d510008aab4aa--git-demo-week1.netlify.app/)

Answer the following questions:
a) What is the difference between Version A and Version B on the README page.

{{</note>}}

## 📜 Code base

Today our lives depends on countless applications that we access on digital devices. These applications run on these devices, and in order to carry out their tasks they make use of software ( or instructions for machines ). A code base is defined as the all code required to implement an application. So a code base is a collection of files and folders that represent all the code we need for a particular application.

## 🗃️ Repository

A repository is a place where we store files and folders used to build a software project.W
We can now think about the

## 🗄️ Storing repositories

Github is a web-based platform used to store repositories. Github is a place where repositories are **hosted**. IN other words, a repository for a project is available over a network. THis means a Github repository can be accessed by multiple developers across a network where they can collaborate on the project.

{{<note type="exercise" title="Exercise 1.1">}}

Follow the link below: figure out the answer to the following questions.
Follow the link to the project.

Answer the following questions:

a) Look at the README.md. Read the instructions on there
b) How many folders are there in the project?
c) How many files are there in the project?

{{</note>}}

## 📸 Different versions

Building software is difficult: it is easy for developers to make errors and program computers to do the wrong thing.
Imagine a situation where we're making changes to a single file.
We might want to make a change so we have to edit this file and then to fix a mistake. We then save the changes.
This means the old version of the file is overwritten and we're left with the newly saved file.

{{<note type="exercise" title="Exercise 2.1">}}

Why is it important to build up different versions of a project over time?
If we build up a collection of different versions in our project?

{{</note>}}

Imagine if you want to track the growth of a plant over time.
You could start by taking a photo at the very beginning.You could then add water to the plant to help it grow and then take another photo of the plant. You could continue taking photos this way. Each photo is a snapshot: a record of the plant at a given moment in time.
In a similar way, we want to build up snapshots of our project's repository over time.
can think of a **commit** as a snapshot of our project at a given moment in time.

{{<note type="definition" title="Definition">}}

A **commit** is a version of our code base at a particular point in time: in other words, a commit is a snapshot

{{</note >}}

{{<note type="exercise" title="Exercise">}}

🔍 In this activity, you'll need to figure out how to do something.

Go to the REPO_URL

Head to Github, on the web page, find the place where it tells you the number of commits and then visit this page.
On this page, try figuring out the following:

a) What is the URL for this page?
b) When was the first commit created (this is the earliest version of the project)
c) Who was the author of the most recent commit?
d) What is the title of commit "786
d) What **change** was introduced in the second commit?
e) What problem did commit "dfef8" solve? What change was introduced to solve this problem?

{{</note>}}

## 🔍 Check out a commit

What is _in_ a commit? We can recall that a commit is a snapshot of a codebase. Therefore, we should be able to check out the codebase at a given point in the timeline and look at the files and folders there. We can use the Github website to not only see the different **commits** in our project - we can also check out the files and folders at a given point in the history.

{{<note type="exercise" title="Exercise 4.1">}}

Go back to this page GITHUB_REPO_URL to look at the following:

and look at one of the commit with hash "d3567h" and then look for the icon that that says "Browse the repository at this point in the history".

Do the same but for the commit "edf89".

{{</note>}}

## 🍴 Forking a repository

Often we want to take an existing project and start working on it independently: in other words, we start making our own versions of the project separate from the original project.

{{<note type="exercise" title="Exercise 5.1">}}

Visit the following GITHUB_REPO_URL and create a fork of the repository to your local account.

{{</note>}}

## 💻 Working locally

We can use Github to view and manage repositories. However, we can also work with repositories locally. **Locally** means taking a copy of a repository on Github and downloading it on to our local machine where we can look around and make changes without being on Github.

{{<note type="exercise" title="Exercise 6.1">}}

🔍 Figure it out - in this exercise, you'll need to figure out how to do something. Even though it is a little unfamiliar.

Firstly,

1. Open a terminal on your computer.

For each of the steps below, you'll need to use your terminal to carry out the commands below.
You can use the [documentation](https://www.techrepublic.com/article/16-terminal-commands-every-user-should-know/)

2. Print your current working directory.
3. List the files and folders in your current working directory.

You'll need a place to store the repositories you'll use on the CYF course.

4. Make a new directory called `cyf` in your home directory.
5. Change directory into the `cyf` directory.
6. Using the terminal, use a command to create a new directory called "CYF". You'll use this directory to store the files and folders in your project.
7. Change your working directory to the "CYF" directory.

{{</note>}}

## Version control software

**Version control software** is software that allows developers to create and manage the versions of a codebase. **Git** is a particular tye of version control software. **Github** is built using Git. However, we can also Git on our local machine to perform similar tasks as we do on Github. The first task we have is This

> ? How can we get a local copy of an existing Github repository on our local machine.

In other words, we need to get a copy of the codebase on Github on to our device.

{{<note type="exercise" title="Exercise">}}

🔍 Figure it out - in this exercise, you'll need to figure out how to do something. Even though it is a little unfamiliar.

1. Research a command you can use to get a local copy of a repository on your local machine.
   Use this command to check

{{</note>}}

## 📘 Viewing the files

Once you've got a local copy of a codebase on your local machine you can start to view the files and folders in that codebase. You can use a code editor like VSCode; VSCode is an application that enables developers to view and edit files on their local machine.

{{<note type="exercise" title="Exercise">}}

Figure out how to open the cloned repository on your local machine in VSCode. Explore the repository in VSCode and use the code editor to look at the various files and folders.

{{</note>}}
