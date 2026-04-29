## Introduction to Version Control with Git and GitHub

This lesson uses [The Carpentries Workbench][workbench] template.

### Build the lesson locally

To render the lesson locally, you will need to have [R][r] installed.
Instructions for using R with the Carpentries template is available on the
[Carpentries website](https://carpentries.github.io/workbench/#installation).
We recommend using the
[`{renv}`](https://rstudio.github.io/renv/articles/renv.html) package.

After cloning the repository, you can set up `renv` and install all packages with:

``` r
renv::init()
# Optionally update packages
renv::update()
```

Once you have installed the dependencies, you can render the pages locally by
starting R in the project root and running:

``` r
sandpaper::serve()
```

When building the site subsequently, you may need to run `renv::activate()` first.

This will build the pages and start a local web-server in R and open it in your
browser. These pages are "live" and will respond to local file changes if you
save them.


[git]: https://git-scm.com
[r]: https://www.r-project.org/
[workbench]: https://carpentries.github.io/workbench/
