## Introduction to Version Control with Git and GitHub

This lesson uses [The Carpentries Workbench][workbench] template.

### Build the lesson locally

To render the lesson locally, you will need to have [R][r] installed.
Instructions for using R with the Carpentries template is available on the
[Carpentries website](https://carpentries.github.io/workbench/#installation).
We recommend using the
[`{renv}`](https://rstudio.github.io/renv/articles/renv.html) package.

Easiest way I found was via [pixi](https://pixi.prefix.dev/latest/installation/):

```console
$ curl -fsSL https://pixi.sh/install.sh | sh
$ pixi init
$ pixi shell
$ R -e 'sandpaper::serve(quiet = FALSE, port = "3435")'
```

This will build the pages and start a local web-server in R and open it in your
browser. These pages are "live" and will respond to local file changes if you
save them.

You probably also need to install our [fork of
`varnish`](https://github.com/ResearchCodingClub/uoy-varnish), which you have to
do via `R`:

```r
> install.packages("remotes")
> remotes::install_github("ResearchCodingClub/uoy-varnish")
# or
> remotes::install_local("path/to/varnish")
```


[git]: https://git-scm.com
[r]: https://www.r-project.org/
[workbench]: https://carpentries.github.io/workbench/
