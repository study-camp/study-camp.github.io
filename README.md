# Study Camp

This is the website and blog for a new initiative to support community-based competency-driven learning for career development in the software industry. It is inspired by the successes of my prior work with Google Developer Groups, running the _Android Study Jam_, _Android Camp_ and _Machine Learning Study Camp_ events in the past two years.

## Topics

The website will be updated with more topics in time. The following reflect my current interests, so expect articles or complete study-camp guides around the following topics:

 * Firebase
 * Progressive Web Apps
 * Python
 * Machine Learning
 * Deep Learning



## Theme & Process

The website and blog is based on the excellent [So Simple](https://mmistakes.github.io/so-simple-theme/) theme from [Michael Rose](https://github.com/mmistakes) (@mmistakes).

I am by no means a Jekyll expert but my goal was to get a static, responsive website running using GitHub pages, with the ability to support blog posts, search and simple navigation. This is one of the featured [free themes](https://jekyllthemes.io/#free) that I personally loved. 

A core tenet of Study Camps is that you always learn a technology or concept better by using it and applying it in real projects. In some sense, this blog is a perfect example of that. By using it frequently, I also hope to improve my own understanding of [Jekyll](https://jekyllrb.com/) and its related usage of [Markdown](https://daringfireball.net/projects/markdown/) and [Liquid](https://github.com/Shopify/liquid/wiki) templating markup.

To learn more about the _So Simple_ template, read [the theme's README](README.theme.md)

To update blog posts or content
 * follow the [theme setup](https://mmistakes.github.io/so-simple-theme/theme-setup/) guidelines
 * use ```bundle exec jekyll build``` to create the *_site* directory that contains the static build for the site. Then use ```bundle exec jekyll serve``` to serve that locally (e.g., for debugging)
 * to have this hosted on GitHub, simply commit changes to the content to a repository that is appropriate for a GitHub Pages endpoint. The build/serve process is transparent to you. GitHub simply rebuilds and deploys the site on each commit (once the *_config.yml* details are updated) 
 * simply commit changes to GitHub to have that site now hosted at the appropriate _gh-pages_ site.