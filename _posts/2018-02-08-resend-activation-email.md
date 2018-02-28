---
date: 2017-01-16
title: Resend activation email
categories:
  - account
description: How to request another activation email
type: Document
---
After register on Roburst.co, if you haven't received any email from us within 10 minutes, you can do the following steps to check for your activation email.

## Check your Spam/Junk inbox

Some email providers may treat the activation email as a spam, you can check for this mail at you Spam/Junk inbox. If there is nothing there, you can continue the next resolution.

## Request new activation email

To request new activation email, go to this link 

## Basic usage

The Jekyll gem makes a `jekyll` executable available to you in your Terminal window. You can use this command in a number of ways:

~~~ bash
$ jekyll build
# => The current folder will be generated into ./_site

$ jekyll build --destination <destination>
# => The current folder will be generated into <destination>

$ jekyll build --source <source> --destination <destination>
# => The <source> folder will be generated into <destination>

$ jekyll build --watch
# => The current folder will be generated into ./_site,
#    watched for changes, and regenerated automatically.
~~~

## Directory structure

Jekyll is, at its core, a text transformation engine. The concept behind the system is this: you give it text written in your favorite markup language, be that Markdown, Textile, or just plain HTML, and it churns that through a layout or a series of layout files. Throughout that process you can tweak how you want the site URLs to look, what data gets displayed in the layout, and more. This is all done through editing text files; the static web site is the final product.

A basic Jekyll site usually looks something like this:

~~~ bash
.
├── _config.yml
├── _data
|   └── members.yml
├── _drafts
|   ├── begin-with-the-crazy-ideas.md
|   └── on-simplicity-in-technology.md
├── _includes
|   ├── footer.html
|   └── header.html
├── _layouts
|   ├── default.html
|   └── post.html
├── _posts
|   ├── 2007-10-29-why-every-programmer-should-play-nethack.md
|   └── 2009-04-26-barcamp-boston-4-roundup.md
├── _sass
|   ├── _base.scss
|   └── _layout.scss
├── _site
├── .jekyll-metadata
└── index.html # can also be an 'index.md' with valid YAML Frontmatter
~~~

## Front matter

The front matter is where Jekyll starts to get really cool. Any file that contains a YAML front matter block will be processed by Jekyll as a special file. The front matter must be the first thing in the file and must take the form of valid YAML set between triple-dashed lines. Here is a basic example:

~~~ html
---
layout: post
title: Blogging Like a Hacker
---
~~~

Between these triple-dashed lines, you can set predefined variables (see below for a reference) or even create custom ones of your own. These variables will then be available to you to access using Liquid tags both further down in the file and also in any layouts or includes that the page or post in question relies on.

![Example image](https://images.unsplash.com/photo-1481487196290-c152efe083f5?ixlib=rb-0.3.5&q=80&fm=jpg&crop=entropy&cs=tinysrgb&w=1920&h=1080&fit=crop&s=80308172730757a7db0434987fa985f3)

## Where additional pages live

Where you put HTML or Markdown files for pages depends on how you want the pages to work. There are two main ways of creating pages:

* Place named HTML or Markdown files for each page in your site’s root folder.
* Place pages inside folders and subfolders named whatever you want.

Both methods work fine (and can be used in conjunction with each other), with the only real difference being the resulting URLs. By default, pages retain the same folder structure in `_site` as they do in the source directory.