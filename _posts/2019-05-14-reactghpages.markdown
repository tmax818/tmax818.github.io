---
layout: post
title: "How to get your React app on GitHub Pages"
subtitle: "The Short Version"
date: 2019-05-14 07:52:32 +0000
header-img: "img/day_twentythree/react.png"
excerpt_separator: <!--more-->
tags: [React, GitHub]
permalink: /day_twentythree
---

This is a quick how to get your React app on GitHub Pages.<!--more-->

## Step 1

### Create your project's directory

```bash
$ mkdir day23
$ cd day23
```

## Step 2

### Generate your React app

Now my working directory is day23. So, inside that directory I create a new React app:

```bash
$ create-react-app .
```

The `.` basically means 'here' so, instead of passing a name to the create-react-app command you are telling it to make the app inside the current directory.

## Step 3

### Remove the Service Worker!!!!

Skip this step at your peril! I don't know why, but the service worker that comes with `create-react-app` will keep your app from deploying to GitHub Pages. So, delete that shit!

{% include image.html url="/img/day_twentythree/servwkr.png" description="delete this file!!!" %}

Then delete any references in the `index.js` file.

{% include image.html url="/img/day_twentythree/indexjsdel.png" description="delete the highlighted text!!" %}

## Step 4

### Install the `gh-pages` npm package

```bash
$ npm i gh-pages
```

As long as you are using the current version of node and npm, you don't need the --save flag.

## Step 5

### Change the `package.json` file

DO NOT cut and paste the following:

<script src="https://gist.github.com/tmax818/ea1e7d4f4da264f5a5b89f634161f181.js"></script>

So `YOUR-WEBSITE` will most likely be `https://USERNAME.github.io/REPOSITORY-NAME` unless you set up GitHub to point to a domain that you own. So this is what my `package.json` file looks like:

<script src="https://gist.github.com/tmax818/b3d78244c4bc0854de176eae5281cfd4.js"></script>

## Step 6

### Push it to your Repo

If you don't know how to do this, check out this [post](/day_five). There are instructions for how to sign up for GitHub and creating a repository.

## Step 7

### Run `npm run deploy`

Run the following command from the root of your react app.

```bash
$ npm run deploy
```

{% include image.html url="/img/day_twentythree/day23site.png" description="finished product!" %}

I got half-way pissed off the first time I tried this. At this point you may have to `git push` again. From here, you can make any changes you want. All you have to do is repeat steps six and seven. Thanks for reading, and feel free to reach out to me if it doesn't work.
