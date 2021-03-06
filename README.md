# Platform User Guidance
[![Build Status](https://travis-ci.org/moj-analytical-services/platform_user_guidance.svg?branch=master)](https://travis-ci.org/moj-analytical-services/platform_user_guidance)

View the user guidance here: https://moj-analytical-services.github.io/platform_user_guidance/

## To update

Make changes to ##-chapter.Rmd files in a branch and pull request into master to publish.

Travis will build the book for you automatically and check that each commit renders in bookdown. Travis will only publish changes on the `master` branch, which are committed to the `gh-pages` branch.

## To render book locally

From R:
```r
bookdown::render_book('index.Rmd', 'bookdown::gitbook')
```

or from shell/terminal `make` (requires GNU Make):

Rendered bookdown content will be in `/docs/`

### Notes on Travis
Auto building requires Travis to be set up with and encrypted SSH key - see [here](https://oncletom.io/2016/travis-ssh-deploy/).
