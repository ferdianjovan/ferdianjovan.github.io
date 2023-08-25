# Ferdian Jovan

This is the repository for my personal website (hosted by github).

## Misc

The site was built using [Hyde](https://github.com/poole/hyde), a theme for [Jekyll](http://jekyllrb.com/). Jekyll is static site generator that is used by [Github](http://github.com) to generate your own personal website. To create a site using this template is simple: 

- Fork the [Hyde](https://github.com/poole/hyde) theme;
- Edit the ```_config.yml``` by changing ```relative_permalinks: true``` to ```relative_permalinks: false```, and add ```plugins: [jekyll-paginate, jekyll-gists]``` to the ```_config.yml```;
- Edit [head.html](https://github.com/poole/hyde/blob/master/_includes/head.html) and change each occurrence of ```{{ site.baseurl }}``` to ```{{ "/" | relative_url }}```;
- Follow the [Creating your site](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site#creating-your-site) steps to enable github generate your site and which branch to use.

## Testing Locally

Jekyll can be installed on your local machine for you to test your site locally. You can follow [this page](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll) to install Jekyll and bundler in the prerequisite section. One side note, I was following [Jekyll Installation](https://jekyllrb.com/docs/installation/) for macOS. Another note, [Xcode](https://apps.apple.com/us/app/xcode/id497799835?mt=12) developer tools might be needed to have Jekyll installed properly. 

To test [Hyde](https://github.com/poole/hyde) theme on a local machine, you just need to git clone the repo (or your forked version), and run jekyll on the site directory with ```jekyll serve```.
Couple notes and prerequisites:

- redcarpet, as markdown processor, can not be used in Jekyll 4.0 and above. Install jekyll 3.9 ```gem install jekyll -v 3.9``` if you want to use this Hyde theme, and run the jekyll server with ```jekyll _3.9_ serve```.
- Install all necessary plugins / gems with ```gem install redcarpet pygments.rb jekyll-paginate jekyll-gist```.

You should now have your site locally which can be accessed at ```http://localhost:4000/```.
