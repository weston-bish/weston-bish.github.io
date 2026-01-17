<!--
title: Still - A Simple Static Site Generator
date: 2026-01-17
-->

# Still - A Simple Static Site Generator

## What is Still?

**still** is a super-minimal static site generator designed for small personal blogs.

It converts Markdown files into simple HTML pages using Python's `markdown` module and combines them with a header and footer to produce fast, portable, brutally minimal websites.

The goal of still is to make it as simple as possible to publish a blog.

**Features include**:

- Minimal — just Markdown, HTML, and a build script
- Fast — builds in milliseconds
- Simple file structure
- Front-matter-style metadata for posts (title, date)
- Auto-generated homepage with post list
- Static output to /public (ready to upload anywhere)
- Bring-your-own CSS
- Optional RSS feed generation

## How I Built This Site with Still & GitHub Actions

It is easy to use still to generate a website of your own and host it on [GitHub Pages](https://docs.github.com/en/pages) for free. Below I will walk through the steps of how I did this in less than 10 minutes.

### 1. Generate a New Repository Using Still as Template

Go to the [still repo](https://github.com/weston-bish/still) and click on "Use this template" followed by "Create a new repository", which will preconfigure your own still repo with pre-configured files and the still project structure.

From here, you are free to edit the various markdown files, the header.html, footer.html, and style.css.If you would like, you may configure the necessary global variables in `still.py` for optional RSS feed generation.

### 2. Configure GitHub Actions for CI/CD

> CI/CD (Continuous Integration/Continuous Delivery) is a DevOps practice that automates the software development lifecycle using a pipeline to build, test, and release software more frequently and reliably.
> Google

Basically, whenever you push a change to your remote repo, GitHub actions will automatically test that the site builds correctly in a container and then deploy it to GitHub Pages. This means that in order to write a new post or update the site, all one must do is make changes to their local repo and push it to remote.

**WORK IN PROGRESS**
