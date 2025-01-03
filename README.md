A Github Pages template for academic websites. This was forked (then detached) by [Stuart Geiger](https://github.com/staeiou) from the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/), which is © 2016 Michael Rose and released under the MIT License. See LICENSE.md.

I think I've got things running smoothly and fixed some major bugs, but feel free to file issues or make pull requests if you want to improve the generic template / theme.

### Note: if you are using this repo and now get a notification about a security vulnerability, delete the Gemfile.lock file. 

# Instructions

1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section
1. (Optional) Use the Jupyter notebooks or python scripts in the `markdown_generator` folder to generate markdown files for publications and talks from a TSV file.

See more info at https://academicpages.github.io/

## To run locally (not on GitHub Pages, to serve on your own computer)

1. Clone the repository and made updates as detailed above
1. Make sure you have ruby-dev, bundler, and nodejs installed: `sudo apt install ruby-dev ruby-bundler nodejs`
1. Run `bundle clean` to clean up the directory (no need to run `--force`)
1. Run `bundle install` to install ruby dependencies. If you get errors, delete Gemfile.lock and try again.
1. Run `bundle exec jekyll liveserve` to generate the HTML and serve it from `localhost:4000` the local server will automatically rebuild and refresh the pages on change.

# Changelog -- bugfixes and enhancements

There is one logistical issue with a ready-to-fork template theme like academic pages that makes it a little tricky to get bug fixes and updates to the core theme. If you fork this repository, customize it, then pull again, you'll probably get merge conflicts. If you want to save your various .yml configuration files and markdown files, you can delete the repository and fork it again. Or you can manually patch. 

To support this, all changes to the underlying code appear as a closed issue with the tag 'code change' -- get the list [here](https://github.com/academicpages/academicpages.github.io/issues?q=is%3Aclosed%20is%3Aissue%20label%3A%22code%20change%22%20). Each issue thread includes a comment linking to the single commit or a diff across multiple commits, so those with forked repositories can easily identify what they need to patch.

# Maintenance

## Add info

Use `_config.yml` to add primary information such as your name and affiliation that will appear on the sidebar. This file is also used to define collections, which are types of information to be processed by the program

For example, `publications` is a collection. All `.md` files assigned to this collection will be formatted in the same way. In fact, all my collections currently have the same format, they only differ in the section they appear.

## Add items

To add a project or a publication, create a `.md` file in the associated folder (e.g. `_publications`) and fill out the paper info. For example, this is the `.md` file associated with one of my publications:

```
---
title        : "Female Labor Force Participation and Economic Growth"
collection   : publications
permalink    : /publication/gender_bonus
doilink      : "https://doi.org/10.1016/j.econlet.2021.109740"
journal      : 'Economics Letters'
year         : "2021"
coauthors    : {"Stephen L. Parente" : "https://publish.illinois.edu/parente/",
                "Eduardo Rios Neto"}
buttons      : 
    wppdf    : "/files/genderbonus.pdf"
    srrn     : 
    bibtex   : "/files/bibtex/genderbonus_cite.txt"
abstract     : "Borrowing from the demographic dividend literature, this paper examines whether there is a gender bonus, namely an increase in the average living standard associated with increases in female labor force participation (FLFP) rates. Translating a per worker production function into a per capita one, it derives a linear dynamic model, the coefficient of which can be used to test for the existence of a gender bonus, and the reasons for this bonus. Using an international panel and applying a system GMM approach, it finds a positive and statistically significant effect of the growth of FLFP on economic growth and a positive but not statistically different from zero effect of the initial FLFP on economic growth. Importantly, we cannot reject the hypothesis that either of these effects is merely an accounting effect, namely a consequence of having more workers in the economy and more aggregate output. It finds no support for a secondary bonus through education or population growth."    
---
```
`coauthors` is a dictionary where the second element is the website of the coauthor. `buttons` takes different links to versions of the paper (`wppdf`, `srrn`, and `repec`), a text file with bibtex info (`bibtex`), and a button with links to replication files (`repfiles`). One can also add the presentations as list/dictionary.

# Customization

The key files to customize the output are `_pages/_about.md`, `assets/css/main.scss`, `_sass/_variables.scss`, and `_includes/archive-single.html`. 

`_pages/_about.md` is the main (and only) page in the website. To add pages, edit `_data/navigation.yml`. 

Use `assets/css/main.scss` to add customized css code. In my case, I have the accordion feature defined in that code. 

`_sass/_variables.scss` allows you to change colors and fonts. 

`_includes/archive-single.html` produces the pages given the inputs in the collection folders. 

## Other details

* add the header in `_sass/_masthead.scss`.



