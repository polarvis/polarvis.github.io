# Web site of the PolarVis project

This repository is used to generate the [Web site of the PolarVis project](https://polarvis.github.io). It is based on [Jekyll](http://jekyllrb.com/) and the [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) Jekyll
theme.

More details about the theme are available from the
[theme repository](https://mmistakes.github.io/minimal-mistakes/).
This README file contains a short manual for project members who want to modify the site, or other people
looking at this repository as an example.

## Updating the site

Every change made to the repository is automatically reflected in the Web site when the change is pushed to 
the main branch. 

Before pushing changes to GitHub, you can check the result locally. This can be done installing
Jekyll and Bundler, and running the following command, that will create a local server where the new site
can be checked:

    bundle exec jekyll serve
    
This is however not necessary: one can also commit and push changes and wait for GitHub to update the sites online (it takes one or a few minutes).

## Adding a page

All pages are located inside `_pages/`, except the home page, generated from the top-level file `index.md`.
A new page can be added by creating a new file inside this directory.
The new page can be added to the top menu by modifying the file `_data/navigation.yml`.

## Modifying the content

To modify the content of a page it may be necessary to change multiple files:

- The page itself.
- The style file `_sass/uuinfolab.scss`, containing the css styles added to the ones provided by mmistakes, if one wants for example to create new classes for <div>, <p>, etc.
- The data files in `_data/` from which part of the page content may be automatically generated, e.g., lists of people, publications, projects, ...
- General page content such as the logo, the links to social media at the bottom, etc. can be specified in the file `config.yml`.
- Images and other resource files are stored in `assets/`. 
