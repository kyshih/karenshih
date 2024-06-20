# Building a personal website
I chose to use the static site generator, <a href="https://github.com/jekyll/jekyll?tab=readme-ov-file">Jekyll</a>. It works seamlessly with GitHub.
It is very customizable without being overly complicated. The Jekyll theme I use for my
website is adapted from <a href="https://github.com/imkaywu/minimal-folio?tab=readme-ov-file">minimal folio</a> by Kai Wu. See <a href="https://kyshih.github.io/karenshih/">my website</a>.

<hr/>

## Getting started
Jekyll is written in Ruby. You can find how to install Ruby <a href="https://www.ruby-lang.org/en/downloads/">here</a>. You would need ruby version manager <a href="https://github.com/rbenv/rbenv">rbenv</a> or <a href="http://rvm.io">RVM</a> in order to switch between the pre-installed Ruby on MacOS and the Ruby for your website. <a href="https://mac.install.guide/faq/do-not-use-mac-system-ruby/">This</a> goes into detail why we shouldn't use the MacOS system Ruby.

## Choose your favorite Jekyll theme
I am using <a href="https://github.com/imkaywu/minimal-folio?tab=readme-ov-file">minimal folio</a> by Kai Wu. But you can find many others <a href="https://jekyllthemes.io">here</a> or <a href="https://github.com/topics/jekyll-theme">here</a>.

Once you find your favoriate theme, fork the repo on GitHub and name your new repo for publishing your website.

## Testing site locally with Jekyll

````markdown
```
git clone your_repo
cd local_path_to_your_repo
rbenv local 3.3.3 # ruby version for your site
ruby -v # should return ruby 3.3.3
bundle install # install all other dependencies specified in your Gemfile
bundle exec jekyll serve # run your Jekyll site locally
```
````
You can now see you site at http://127.0.0.1:4000/.

## Add content to your site
You are now ready to add content to your site!

## Push commits to your GitHub repo
````markdown
```
git add .
git commit -m "first version of my website"
git push
```
````
New changes will be reflected in a couple of minutes!

## Below are the features of minimal folio

### Collections
This Jekyll theme implements collections to let you break up your work into categories. The example is divided into photoportfolio and portfolio, but easily revamp this into recipes, apps, short stories, limmericks, whatever your creative work is.

> To do this, edit the collections in the config file, create a corresponding folder, and update the portfolio and portfolio source files.

Two different layouts are included—the blog layout (`blog/index.html`), for more detailed descriptive list of entries, and the portfolio layout. The portfolio layout overlays a descriptive hoverover on a background image. If no image is provided, the square is auto-filled with the chosen theme color. Thumbnail sizing is not necessary, as the grid crops images perfectly.

> The thumbnail crop does NOT work as perfectly, will attempt to address in
> the future.

### Portfolio Specifics
You can easily add full pages for each of the projects in your portfolio. If you want one to link to an external website, create a file for it in `_portfolio`, and  fil in the YAML front matter as you would for another, but with a redirect, like so:

	---
	layout: post
	title: Project
	description: a project that redirects to another website
	img:
	redirect: https://otherpage.com
	--- 

### Theming
Six beautiful theme colors have been selected to choose from. The default is red, but quickly change it by editing the `_variables.scss` file. The color variable are listed there, as well.

### Photos
Photo formatting is made simple using rows of a 3-column system. Make photos 1/3, 2/3, or full width. Easily create beautiful grids within your blog posts and projects pages.

### Code Highlighting
This theme implements Jekyll's built in code syntax highlighting with Pygments. Just use a liquid tag to delineate your code:
{% highlight python %}
	code code code
{% endhighlight %}

### Blockquotes
Three types of blockquotes are included, which are NOTE, WARNING and ERROR, each colored by green, yellow, and red, respectively.

### Math Equations
Support fast math equation rendering supported by MathJax 3.


<hr/>
The MIT License (MIT)
Copyright (c) 2015 Lia Bogoev, 2023 Kai Wu

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
