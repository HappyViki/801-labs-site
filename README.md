# 801 Labs site
Contact me through [UtahJS Slack](https://utahjavascript.slack.com/) to hire me.

Current and future tools: HTML, CSS, JavaScript, [Bulma](https://bulma.io/) CSS framework, [Hugo](https://gohugo.io/) static site framework

# Guide

[Hugo Docs](https://gohugo.io/documentation/) | [Bulma Docs](https://bulma.io/documentation/)

Look at the site:
```
clone https://github.com/HappyViki/801-labs-site.git
cd 801-labs-site/hackerspace
hugo server
```
Go to http://localhost:1313/

## Page Structure
Location of pages: hackerspace/content

Location of new page structure: hackerspace/archetypes

### Create a page:

`hugo new [page-name.html]`

### Default (default.html) page:
```
---
title: "{{ replace .Name "-" " " | title }}" \\ Page Name
date: {{ .Date }} \\ Example: 2019-12-17T16:34:31-07:00
draft: true \\ This is default, change to 'false' when ready
---

<section class="section has-text-centered">
  <div class="container">
    <h1 class="title">{{ replace .Name "-" " " | title }}</h1> \\ Page Name
  </div>
</section>

<!-- Body Of Page -->
```
