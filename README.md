# [P2P Economy](https://economy.p2p.org/)
Welcome to the P2P Economy blog repo! [Contributions, typo fixes and pull requests are welcome](https://github.com/p2p-org/economy/new/master/post) :thumbsup:

## Table of Contents
<!-- ⛔️ AUTO-GENERATED-CONTENT:START (TOC:collapse=true&collapseText=Click to expand) -->
<details>
<summary>Click to expand</summary>

  * [1. Write your content in markdown!](#1-write-your-content-in-markdown)
  * [2. Name your post file name](#2-name-your-post-file-name)
  * [3. In your post, include post meta information:](#3-in-your-post-include-post-meta-information)
- [Post Heading](#post-heading)
- [Post SubSection](#post-subsection)
  * [4. Add your author bio](#4-add-your-author-bio)
  * [5. Add your company](#5-add-your-company)
  * [6. Submit a PR to the repository](#6-submit-a-pr-to-the-repository)
  
- [Including Custom Scripts](#including-custom-scripts)
- [Markdown Resources](#markdown-resources)
- [Recommended Writing Apps](#recommended-writing-apps)

</details>
<!-- AUTO-GENERATED-CONTENT:END -->


### 1. Write your content in markdown!

> New to markdown? [Read this](https://guides.github.com/features/mastering-markdown/)

> Need Content ideas? [Read this](./writers-guide.md)

---

### 2. Name your post file name

`YYYY-MM-DD-blog-post-name.md` :point_right: `2016-01-27-post-title-here.md`

> [handy tool for slugifying titles](https://blog.tersmitten.nl/slugify/)

---

### 3. In your post, include post meta information:

Include the post metadata at the top:


```
---
title: My awesome post title
description: "This post is about awesome stuff!"
date: 2016-07-25
thumbnail: 'http://url-to-thumbnail.jpg'
layout: Post
authors:
  - FirstnameLastname
---
```

Below the post meta, add your markdown:

<pre>
# Post Heading

This is an awesome paragraph!

## Post SubSection

[Link example](http://my-full-url-with-http-at-the-front.com)

* List item 1
* List item 2
* List item 3

```js
// code snippet example with javascript (js) syntax highlighting
console.log('JS code')
```
</pre>

> Questions about formatting? [See a complete post example] *Нужно вставить ссылку с примером

---


### 4. Add categories

Choose appropriate categories for the blog post from the list of categories available [here](./categories.json). Multiple categories can be assigned to a blog post.

The values that are supplied for categories for the blog post must match any of the keys in the (categories.json)[./categories.json]

If you want to add a new category, you can add another entry at `categories.json` and use it in the blog post.

```yml
---
layout: Post
title: David's Amazing Post
categories:
  - guides-and-tutorials
  - user-stories
---
```

### 4. Add your author bio

If you haven't created an author bio in the `/authors` folder. Go ahead and do that now.

The name of the file should be the same as the name field used in the blog post meta data. Format: `FirstnameLastname` (note the caps and no space!)

Example `authors/DavidWells.json` and `DavidWells` in the `authors` field below are the same name and capitalization.

```yml
---
layout: Post
title: David's Amazing Post
authors:
 - DavidWells # references data in authors/DavidWells.json file
---
```
### 5. Add your Company 

If you haven't created an Company in the `/company` folder. Go ahead and do that now.

The name of the file should be the same as the name field used in the blog post meta data. Format: `Companname` (note the caps and no space!)

Example `company/P2PEconomy.json` and `P2PEconomy` in the `company` field below are the same name and capitalization.

```yml
---
layout: Post
title: David's Amazing Post
authors:
 - DavidWells # references data in authors/DavidWells.json file
company:
 - P2PEconomy # references data in company/P2PEconomy.json file
---
```

### 6. Submit a PR to the repository

**P2P Economy team members**

> [click here to add a post](https://github.com/p2p-org/economy/new/master/post) or submit a PR.

We will review and publish your post with our audience on [economy.p2p.org](https://economy.p2p.org/) and share it all around the web!

Ping us with any questions on [Twitter](https://twitter.com/P2Peconom) or [post an issue](https://github.com/p2p-org/economy/issues/new) and we will get back with you shortly.

---

## Updating featured posts

The file [featured-blogs.json](./featured-blogs.json) contains a list of file names(excluding date and extension) of the blog posts to be featured on the website.

If the blog file name is `2016-06-28-p2peconomy-v1-0-alpha-release-1.md`, then the file name to be added in the `featured-blogs.json` file is: `p2peconomy-v1-0-alpha-release-1`.

The order of the file names in this file defines the order of featured posts on the website.

## Including Custom Scripts

**Note:** For security purposes, all scripts referenced are vetted and hosted via our s3 bucket.

If you need to include a custom script for demo purposes, you will need to send the script over to us for review.

```yml
# blog post frontmatter
layout: Post
title: David's Amazing Post
scripts:
  - https://link-to-custom-js-in-s3-bucket.js
  - http://link-to-custom-js-two-in-s3-bucket.js
inlineJS: |
  console.log('hi')
  console.log('this is a multiline inline JS that will run in the post')
```

## Markdown Resources

Our blog posts are written in markdown and support standard [Github flavored markdown](https://guides.github.com/features/mastering-markdown/). If you are new to markdown, don't fret, check out this handy [how to guide on writing in markdown](https://blog.ghost.org/markdown/)

Need a markdown editor? Give [stackedit.io](https://stackedit.io/editor), [Byword](https://bywordapp.com/) or [typora](https://www.typora.io/) a spin.

Need to convert a Google doc to markdown? [Install this chrome extension](https://chrome.google.com/webstore/detail/export-as-markdown/hbojhdcnbcondcdfpfocpkjkfkbnbdad)

Need to convert HTML to markdown? You can use [this handy html to markdown converter](https://domchristie.github.io/to-markdown/)

Need to convert Word to markdown? You can use [this handy Word to Markdown Converter](https://word-to-markdown.herokuapp.com/)

## Recommended Writing Apps

[hemingwayapp](http://www.hemingwayapp.com/desktop.html) - Hemingway helps you write with power and clarity by highlighting adverbs, passive voice, and dull, complicated words
