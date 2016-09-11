---
layout: post
title: "Welcome to Jekyll!"
date: 2016-09-10 20:40:00 +0100
logo: birthday-cake
categories: general
---

Since reading a [post by Scott Hanselman](http://www.hanselman.com/blog/YourWordsAreWasted.aspx), creating a blog has been a distant goal. Granted it's taken me a little over 4 years but the lure of playing with [Jekyll](https://jekyllrb.com/) and its GitHub integration finally got me there.

The set-up was pretty straightforward:

1. Create a new repository for my [GitHub page](https://pages.github.com/) with a Jekyll `.gitignore`
2. Install Jekyll `gem install jekyll`
3. Create the site `jekyll new . --force`
4. Update the Gemfile and replace the Jekyll gem with the github-pages gem (both lines are in the file)

That's the basic set up and I could immediately run the site up to have a look. I did run into one 'gotcha', the need to prefix all jekyll commands with `bundle exec` or it would use the wrong version of Jekyll and error.

There are hundreds of themes to choose from but I liked the simplicity of [Trio](https://github.com/ankur-gupta/trio). If the blog sticks then I expect to slowly move towards my own theme. Publishing is as easy as `git push origin` which I can just about manage.

The only other problem I ran into was needing `site.url` to equal `https://davidamey.github.io` when published but `http://localhost:4000` when previewing locally. There are several proposed solutions to this, the best, in my opinion, is [discussed on stack](http://stackoverflow.com/questions/27386169/change-site-url-to-localhost-during-jekyll-local-development) but I opted to simply use `/` instead of `{% raw %}{{site.url}}{% endraw %}` in most places of the site.

Now to understand tags/categories/collections...