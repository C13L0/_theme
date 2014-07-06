###A starter theme directory for Jekyll which uses compass, singularitygs, and SMACSS
---
###Dependencies

* [RVM](https://rvm.io/)
* [Jekyll](http://jekyllrb.com/docs/installation/)

###Installation
* $ `jekyll new sitename`
* cd to your newsite
* $ `jekyll serve --watch`
* Open another terminal window
* cd to your newsite
* $ `git clone git@github.com:C13L0/_theme.git`
* $ `cd _theme`
* $ `bundle install`
* $ `compass watch`
* In a text editor, open _includes/head.html and edit the href under <!-- Custom CSS --> to use styles.css
```
<!-- Custom CSS -->
    <link rel="stylesheet" href="{{ "/css/styles.css" | prepend: site.baseurl }}">
```
*  In a text editor, open _layouts/default.html. Add the following code under <!DOCTYPE html>

```
<head>
    <!-- Custom default layout CSS -->
    <link rel="stylesheet" href="{{ "/css/layouts/default.layout.css" | prepend: site.baseurl }}">
</head>
```
*  Navigate to css folder and delete main.css
*  Refresh your browser

###Set up completed
If _theme set-up is successful, the site will still look like the original starter jekyll site. Your new site will now be using sass/compass, singularity for grid layouts, and breakpoint for media-queries.


###Trouble shooting
>**Bundle install errors**
If any errors are produced at $ bundle install, you are probably missing a gem on your local. The top few lines will usually tell you which ones. Do *not* install any gems using sudo because rvm will not be able to manage them.
* $ `cd ~`
* $ `gem install missing-gem`

