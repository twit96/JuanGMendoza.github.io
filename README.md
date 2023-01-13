# juangmendoza.github.io

## TODO:
- [ ] Standardize "Research" Page
- [ ] Standardize "Writings" Page
- [ ] Sort "[unused]" Directory
- [ ] Remove Unused Assets within all pages.
- [ ] Code Cleanup and Polish


## Directory Structure
The root directory is structured so that each website page is nested within its own directory, and its HTML file is named "index.html". This is useful because it formats your links based on its location in the project and removes the HTML extension.

For instance, the about page is located at: "/about/index.html"
and so its public URL will be "https://juangmendoza.com/about/".

Within most page directories, there is an assets folder for images, videos, PDF's, and any other files linked to by that HTML page. This better organizes assets files by keeping them grouped with the page they correspond to, and shortens pathnames within each HTML files.

## CSS Files
There is a main CSS file called "main.css" at the root directory of the project. This file contains presets (e.g. color variables), default styles, and reused styles across the project.

Within some page directories, a supplementary CSS file called "index.css" is used to extend "main.css" or add styles that are only used on that page. These pages will link to both files in the "head" tag of their HTML.

## Writings Directory
Within the writings directory, each blog post (or any other entry) should have its own sub-directory, containing any necessary assets linked to within the article. The "YYYYMMDD-template" directory provides the template HTML file that should be used for each blog post.

## Includes Directory
Within the root directory, there is one special sub-directory named "includes". This folder contains a template "header" and "footer" JavaScript file which is used on all website HTML pages. Since these two components are prone to frequent updates, injecting them into the pages with a "script" tag makes the website more maintainable by preventing required copy/pastes on every HTML page when one of these components is updated.

To update the header or footer on every single website page in a single step, you need only update the corresponding file in this directory.

There is also a "blogpost_breadcrumbs" JavaScript file in this directory for use on all blog posts. Since this element will be pasted on every blog post, having it templated allows for easier changes down the road.
