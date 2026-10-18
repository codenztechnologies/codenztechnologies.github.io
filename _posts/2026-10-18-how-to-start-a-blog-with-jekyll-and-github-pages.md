---
layout: post
title: How to Start a Blog with Jekyll and GitHub Pages
date: 2026-10-18
description: Learn how Codenz Test Blog uses Jekyll, Markdown, and GitHub Pages to publish posts from a Git repository.
---

Codenz Test Blog is a small blog built with Jekyll and hosted on GitHub Pages. It exists to test publishing articles automatically from a marketing platform into a Git repository. That makes it a practical example of a simple, file-based publishing workflow.

## What this blog is built for

The main goal of this blog is to check whether articles can move cleanly from a marketing platform into a Git repository. That kind of setup is useful when you want content to live in version control and be published through the same repository that stores the site.

Because the blog is built with Jekyll and hosted on GitHub Pages, the publishing path stays lightweight. There is no need for a separate database-backed blogging system in this setup. Instead, the site can be managed as static content in Git.

## How publishing works here

Every post on the blog is a Markdown file in the site’s `_posts` folder. The site rebuilds automatically on every commit to the `main` branch.

That means the workflow is straightforward:

1. Create or update a post as a Markdown file.
2. Commit the change to the repository.
3. Let GitHub Pages rebuild the site.
4. Review the published result.

This is a simple model, but it is also very clear. The repository is the source of truth, and the build happens from the files that are committed.

## Why Jekyll fits this setup

Jekyll is a static site generator designed for plain text content, static sites, and blogs. It turns Markdown content into a blog that can be served as static pages.

That matches the needs of a Git-based publishing workflow. Posts can be stored as text files, versioned in Git, and generated into a site without needing a more complex application stack.

GitHub Pages can host Jekyll-based sites directly from a GitHub repository. For this blog, that makes it a natural fit: content lives in Git, Jekyll handles the site generation, and GitHub Pages provides the hosting layer.

## What a new post needs

A new post belongs in the `_posts` directory. Jekyll posts use Markdown, and the file content starts with front matter that defines post metadata.

After that, the rest of the file is written in Markdown. This keeps article creation simple and predictable. The structure is file-based rather than form-based, so the publishing process stays close to the repository.

If you are setting up a similar blog, it helps to think in terms of files first:

- one file per post
- Markdown for the article body
- front matter for metadata
- commits as the publishing step

## A simple workflow for new articles

A Git-based publishing flow works well when the goal is automation. For Codenz Test Blog, the focus is on testing that articles can be published automatically from a marketing platform into the repository.

That kind of workflow supports a clear handoff between content creation and site generation. Once a post is committed, the site rebuilds automatically. This reduces the amount of manual work involved in getting a post live.

The benefit is not complexity; it is simplicity. The setup is easy to reason about because each article is just a Markdown file tracked in Git.

## What readers can learn from the setup

This kind of blog setup shows how a small Jekyll site on GitHub Pages can be used to test a publishing pipeline. It is a useful pattern when you want content to move through Git instead of being published through a separate CMS.

It also keeps the focus on the content workflow rather than infrastructure management. Jekyll handles the static generation, GitHub Pages provides hosting, and commits trigger the rebuild. That leaves the publishing process centered on writing, versioning, and automation.

For teams or individuals exploring how to start a blog with Jekyll and GitHub Pages, this approach offers a clean baseline: store posts as Markdown, commit them to the repository, and let the site regenerate automatically.
