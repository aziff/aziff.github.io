---
layout: post
title:  "Resources to Create a Website with GitHub and Jekyll"
date:   2021-11-21 
author: Anna Ziff
categories: jekyll
---

_Updated: December 20, 2021_

I created this website using Github pages and Jekyll. I document the steps I followed with some links that I found particularly helpful for my setup. 

_Disclaimer:_ This post is as much for my own reference as it is for sharing resources. It is not a detailed tutorial, but rather an overview of setting up a website and corresponding resources. It focuses on MacOS. As I learn more, I will add information!

## Setting Up a Website
1. I found an example of a [website created in Jekyll][stevemiller] that I liked. Thankfully, this researcher made his own [Jekyll template][ngvb]. I also enjoyed perusing the lists of Jekyll themes at the below links.
* [GitHub #jekyll-theme][github-jekyll]
* [Jamstack Themes][jamstack-themes]

2. I forked the repository of the theme on GitHub, naming it `aziff.github.io`. I then cloned the repository to get a local copy. I suggest reading the `README.md` file associated with your chosen theme to follow any additional steps that may be required. 

3. I set up Ruby and associated software (e.g., Homebrew) on my computer. Even though Apple computers come with a system Ruby, [it is advised to set up a separate Ruby][use-diff-ruby] to help manage libraries/versions. 
* I followed Steps 1-8 outlined in [this very detailed guide][ruby-guide]. It includes separate instructions for Intel or M1 chips and has some advice for troubleshooting common issues. 

4. I set up Jekyll following [this general advice for Jekyll on macOS][jekyll-macOS]. Note that the [guide][ruby-guide] suggested in step 3 has directions to use `asdf` rather than `rbenv`. I also installed bundler.


5. I followed all the steps in the section "Add the github pages gem" [in this guide](https://idratherbewriting.com/documentation-theme-jekyll/mydoc_publishing_github_pages.html). 


## Updating a Website

I edit the files in my repository to customize and update my website. To test changes, I use the first line and navigate to `http://localhost:4000`. Once I am ready to publish changes, I use the second line. 

{% highlight bash %}
bundle exec jekyll serve
bundle exec jekyll build
{% endhighlight %}


## Other Resources

* [Using Academicons and Font Awesome in Jekyll](https://www.janknappe.com/blog/Integrating-Academicons-with-Fontawesome-in-the-Millennial-Jekyll-template/)



[jekyll-macos]: https://jekyllrb.com/docs/installation/macos/
[ruby-guide]: https://mac.install.guide/ruby/index.html
[use-diff-ruby]: https://www.freecodecamp.org/news/do-not-use-mac-system-ruby-do-this-instead/
[stevemiller]: http://svmiller.com
[ngvb]: https://github.com/svmiller/steve-ngvb-jekyll-template
[github-jekyll]: https://github.com/topics/jekyll-theme
[jamstack-themes]: https://jamstackthemes.dev/ssg/jekyll/

