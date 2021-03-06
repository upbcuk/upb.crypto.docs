This page uses jekyll with the [minimal mistakes theme](https://github.com/mmistakes/minimal-mistakes).

### Testing Site Locally

You can test the deployment locally by setting up jekyll and the plugins as follows:

1. Make sure you have Ruby 2.1.0 or higher installed by running `ruby --version`
2. Install the bundler gem via `gem install bundler`
3. Make sure you are in the root folder of the repository (where the Gemfile is) and install the dependencies via `bundle install`
4. Run the site locally via `bundle exec jekyll serve`
5. Preview the local site at `http://localhost:4000`

For more information, view [the github help page on this topic](https://help.github.com/en/github/working-with-github-pages/testing-your-github-pages-site-locally-with-jekyll).

To render the LaTex, we use MathJax Version 2 (there seemed to be some issues with MathJax Version 3 and Jekyll, but I have not tested that).
To enable MathJax rendering for a site, add `mathjax: true` to the YAML Front Matter of the corresponding markdown page.
The YAML Front Matter is the YAML code delimited by `---` at the top of a markdown page.

The Markdown partser used is [Kramdown](https://kramdown.gettalong.org).
Its documentation is helpful for looking up things such as what kind of Latex math delimiters are supported etc.

### Jupyter

The documentation contains a number of Jupyter notebooks.
To run these locally, you need to:

1. [Install Jupyter](https://jupyter.org/install)
2. [Install the IJava Jupyter Kernel](https://github.com/SpencerPark/IJava)

Then you can view the notebooks as usual via `jupyter notebook`.