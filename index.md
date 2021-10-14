# [Jekyll](https://jekyllrb.com/)

---
## What is Jekyll?

Jekyll is a static site generator. It takes text written in your favorite markup language and uses layouts to create a static website. You can tweak the site’s look and feel, URLs, the data displayed on the page, and more.

---
## Installation - Ubuntu

```shell
sudo apt-get install ruby-full build-essential zlib1g-dev
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc 
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc 
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc 
source ~/.bashrc
```

---
## Make new project

```shell
jekyll new my-portfolio
```

---
## Start the server

For the first time,
```shell
bundle exec jekyll serve
```

Post the first time,
```shell
jekyll serve
```

---
## Directory architecture

Directory / File | Purpose
---|--
*_site* | Holds the final version of the website to serve it (Don't modify - It will be automatically updated)
*_posts* | Our posts to be posted
*_configure.yaml* | Config file
*Gemfile* | Used to story all dependencies (uses ruby)
about.md | About page
index.md | Home page
404 html | DEfault 404-page

If you just want a simple blog up and running, follow the below steps,

1) Change the contents of *index.md* and *about.md* 
2) Make a new file in *_posts* for every new post. Ensure the file name is the following format,
> YEAR-MONTH-DAY-title.MARKUP

---
## Front matter

- Details about a page in our website
- Can be written in YAML or JSON format
- Front matter variables
	- *Default variables*
		- layout: template or skeleton for the page 
		- title
		- date
		- categories
	- *Custom varibles*

> Note: All pages should have front matter

</br>

You can see the front matter surrounded by, "---"

```
--- 
layout: post 
title: "Welcome to Jekyll!" 
---
```

---
## Themes

> Jekyll supports gem-based themes (default theme: Minima)

In case of Minima, your Jekyll site's directory structure would be,

```
. 
├── Gemfile 
├── Gemfile.lock 
├── _config.yml 
├── _posts 
│ └── 2016-12-04-welcome-to-jekyll.markdown 
├── about.markdown 
└── index.markdown
```

You can easily choose from a list of [themes](https://jekyllrb.com/docs/themes/#pick-up-a-theme) 

---
# And you just built your blog!!! 
---

## Futher study

Refer to the [Jekyll documentation](https://jekyllrb.com/docs/) to see Jekyll in full action.

Refer to [Mika Dane's Jekyll series](https://www.youtube.com/watch?v=T1itpPvFWHI&list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB&index=1) for video tutorials on how to get a blog up and running with Jekyll!

---
## Happy blogging :)
