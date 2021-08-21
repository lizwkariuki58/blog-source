---
title: "How to Host a Hugo Site for Free on Github Pages"
date: 2021-08-21T11:33:21+03:00
draft: false

tags: ["hugo", "github-pages"]
categories: ["Web Development"]

description: "Find out how to create a Hugo site and host it on Github Pages for free."
resources:
- name: "featured-image"
  src: "featured-image.jpg"
---
Find out how to create a Hugo site and host it on Github Pages for free.

<!--more-->

## 1 Introduction
So you want to create your first personal website? You have probably heard of Content Management Systems(CMSs) like Wordpress or Website Builders like Wix. But unless you are building a very complex website,you don't need the complications, risks and costs that come with the above options. CMSs create heavy websites that are slow, prone to security risks and costly to host. Static site generators overcome this problem by generating static html files which are light, secure fast and cheap(even free) to host.  

## 2 Why use Hugo
There are lots of static generators you can use to generate your website. Examples include: [Hugo](https://gohugo.io/), [Gatsby](), [Jekyll](),[Next.js](),[Pelican]() etc. I chose Hugo for the following reasons:
- It is well-documented with a large community of users and library of themes and templates.
- It is fully free and open source.
- Posts are written in Markdown which allows for powerful formatting and is transferrable.
- It has a very fast build time.
- It is SEO Friendly.

## 3 Why Use Github Pages
Github pages is a hosting service offered by Github to let creators showcase their work for free. There are 2 types of Github pages websites: organizational pages and project pages. The default url is in the format username.github.io but you could also configure the site to show on your custom domain.

There are two ways to get your site on Github pages. You could use Github to host only the static files required to build your site. These are typically found in the 'public' folder in Hugo. This option gets the work done but the code used to generate the site itself is not tracked and stored via Git. The second option or what I call 'the right way' lets you track the static pages, the hugo code and the theme in separate submodules. Let's get started.

## 4 Set Up Hugo Site and Push to Github
To build a site with Hugo, you must first install Hugo on your local machine. Check [this](https://gohugo.io/getting-started/installing/) page on how to install hugo on your Operating System. Once Hugo is installed:

1. Create a new site by running :

```shell
hugo new site my_website
cd my_website
```
2. Create a Github repository for the site and initiate it without a README file. 
3. In your website root directory, initialize git, add remote repository, add the files, commit the changes and push to origin. 

```shell
git init
git remote add origin *url*
git add .
git commit -m "Initial commit"
git push -u origin master
```
4. Create a second repository on Github to host the public html files. If this is an 'organization' site on Github, name the repository '''username.github.io'''.
5. At the project root folder add this repository as a submodule in a folder called public.

```shell
git submodule add -b master *repo url* public
````
6. Run the command ```hugo``` to build the site.
7. In the public folder, add and commit the changes.

```shell
cd public
git add .
git commit -m "initial commit of public files"
```
8. Go back to the project root, add and commit all the changes and most important, push both repositories as shown below:

```shell
cd ..
git add .
git commit -m "Commit both repositories"
git push -u origin master --recurse-submodules=on-demand
```
9. Go to the settings page on the public Githup repository, and turn on the site. Your site is now live but it does not have any content or a theme.

## 5 Adding a Theme to Your Site.
We shall be using a submodule to add a theme to your project for the following reasons:
- You shall be able to track changes you have made to the theme code separately.
- You can still easily update your theme with changes made by the theme's creator.

To begin with you need to choose a theme. Hugo has a diverse selection of themes to fit your every need be it blogging, documentation, displaying a portfolio etc. You can use [this resource](https://awesomeopensource.com/projects/hugo) to pick a theme. After choosing a theme fork its repository to your Github profile so that you can make any changes you need. To add the forked repository as a submodule to your project, go to the website root folder and run:

```shell
git submodule add *forked repo url* themes/theme-name
```
## 6 Set up Website
1. Edit the config.toml file to set up the theme and base url.

```
baseURL = 'https://username.github.io/'
title = 'Site Title'
theme = 'theme-name'
```
2. To create your first post, run the following command:
```shell
hugo new first_post.md
```
3. Run the command 'hugo' to build the site.
4. Run the command 'hugo server' to preview the site locally.
5. Once you are satisfied by the site, add and commit the changes and push them to Github as follows.
```shell
cd public
git add .
git commit -m "Commit first post"
cd ..
git add .
git commit -m "Commit first post and theme"
git push -u origin master --recurse-submodules=on-demand
```

## 7 Conclusion
Congratulations on building your first Hugo site and hosting it on Github Pages! To help you along this journey, here are some additional resources:
- [Getting Started with Hugo](https://gohugo.io/getting-started/)
- [Github Pages Documentation](https://docs.github.com/en/pages)
