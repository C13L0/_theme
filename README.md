###Jekyll, Compass, [SIngularitygs](http://singularity.gs/), [SMACSS](smacss.com)
---
###Dependencies

* [RVM](https://rvm.io/)
* [Jekyll](http://jekyllrb.com/docs/installation/)

###Instructions

* $`jekyll new sitename`
* $`jekyll serve --watch`
* git clone this folder into the root of your site
* Open another terminal window
* cd into _theme
* $`bundle install`
* $`compass watch`
* Open _includes/head.html and edit to use styles.css
* Open _layouts/default.html. Add under <!DOCTYPE html>
```<head>
    <!-- Custom default layout CSS -->
    <link rel="stylesheet" href="{{ "/css/layouts/default.layout.css" | prepend: site.baseurl }}">
</head>```

**Bundle install errors**
If any errors are produced at $ bundle install, you are probably missing a gem on your local. The top few lines will usually tell you which ones. Do *not* install any gems using sudo or rvm will not be able to manage them.

* $ `cd ~`
* $ `gem install missing-gem`

###Theme directory structure
