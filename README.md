# Web site of the Uppsala University Information Laboratory

This repository is used to generate the [Web site of the UU-InfoLab](https://uuinfolab.github.io). It is based on [Jekyll](http://jekyllrb.com/) and the [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) Jekyll
theme.

More details about the theme are available from the [theme repository](https://mmistakes.github.io/minimal-mistakes/).
This README file contains a short manual for the lab members who want to modify the site, or other people
looking at this repository as an example.

## Updating the site

Every change made to the repository is automatically reflected in the Web site when the change is pushed to the main
branch, which is the only one we use. 

All pages are located inside the `_pages` directory.  A new page can be added by
creating a new file inside this directory.  The pages directly accessible through the main menu are
stored directly inside the directory, while other pages are stored in subfolders. In case a new main-menu page is 
added, which would normally not happen without having discussed this first, it can be added to the menu by 
modifying the file `_data/navigation.yml`.
