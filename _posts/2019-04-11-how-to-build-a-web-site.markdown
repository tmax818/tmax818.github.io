---
layout: post
title: "How to Build a Web Site"
date: "2019-04-11 08:08:56 -0700"
header-img: "img/webdev.jpg"
excerpt_separator: <!--more-->
tags: [180]
permalink: day_five
---

In under a minute...or so...<!--more-->

Okay, to follow along with this tutorial, you need three things:

1. a GitHub account
2. a Bash terminal
3. a local version of git

Type `git --version` into your terminal and you should see somthing like this;

```Bash
$ git --version
git version 2.19.1
```

If you don't, you need to install git on you system. There are plenty of tutorials for this. For the sake of brevity I will leave this to you as an exercise.

All these items are free and if you're on a Mac or Linux machine, you already have the second item. A GitHub account is as easy as this:

{% include image.html url="/img/day_five/github.png" description="Google GitHub and sign up!" %}

Once you have an account, create a new repository.

{% include image.html url="/img/day_five/greenbutton.png" description="Click the green button!" %}

I always name the repository the same as the root directory(folder) on my computer to avoid confusion.

{% include image.html url="/img/day_five/type.png" description="Type website in the box!" %}

GitHub gives you the commands to type into your terminal. We are going to alter these commands slightly as we don't need a `README.md` file.

{% include image.html url="/img/day_five/newrepo.png" description="You are now the proud owner of your own repo! Call your mom!" %}

So back in our terminal we write our game-changing web page!

```Bash
mkdir website
cd website
touch index.html
echo "Hello World!" > index.html
```

Okay, that's it! The website is finished. Now, we need to get it on the live web. GitHub has "GitHub Pages" that allows you to host static websites for free. First we have to put(push) our site onto GitHub.

```Bash
git init
git add .
git commit -m "init commit"
git remote add origin https://github.com/[YOUR USER NAME]/website.git
git push -u origin master
Username for 'https://github.com': [TYPE USERNAME]
Password for 'https://tmax818@github.com': [TYPE PASSWORD]
```

If everything works, and that can be a big 'if', you should see something like the following:

```Bash
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 230 bytes | 230.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/[YOUR USERNAME]/website.git

- [new branch] master -> master
  Branch 'master' set up to track remote branch 'master' from 'origin'.

```

Refresh your GitHub page and you should see this:

{% include image.html url="/img/day_five/ghsuc.png" description="Click on 'Settings'" %}

Click 'Settings' and scroll down to the 'GitHub Pages' section:

{% include image.html url="/img/day_five/ghp.png" description="Find the GitHub Pages section almost at the bottom of the page." %}

Click the drop-down that says 'None' and select 'master branch':

{% include image.html url="/img/day_five/selgh.png" description="Change 'None' to 'master branch'." %}

Your page should reload and you will see a link to your website:

{% include image.html url="/img/day_five/nghp.png" description="Your website will be different from mine! Click the link." %}

You did it! It may take a few minutes for the page to process.

{% include image.html url="/img/day_five/end.png" description="Great Success!!" %}

Congratulations on your first web site. You now have a website on the live web! You can watch the video [tutorial](https://youtu.be/WrIKvc8_x1o) on YouTube!
