### How to run the website locally?
bundle exec jekyll serve --livereload

### Useful guides
- [Install guide](https://jekyllrb.com/docs/installation/macos/)
- [Setup of a new Jekyll project gist](https://gist.github.com/MichaelCurrin/3e5e063a89196eca997cac34e7678c77)
- [Jekyll Quick start guide](https://jekyllrb.com/docs/)

### Where is the first page
`index.html` that is at the root of the folder which is for the homepage. It uses the `default` layout from `_layouts\default.html`.
The other pages are in `_pages`. 

There is a `_include\posts.html` which I believe get hooked by jekyll from `_posts` automatically.

### What is `_includes/` folder
The _includes folder in Jekyll is a directory where you can store reusable HTML code snippets that can be included in your Jekyll pages and posts using the Liquid templating engine. 

# Argon Theme
Jekyll Argon Theme: https://jekyllthemes.io/theme/argon-jekyll-theme
Original Argon Theme: https://demos.creative-tim.com/argon-design-system/index.html


### Where is menu items stored
`_data/settings.yml`. This file is also holds theme specific settings.

### Where is the navigation stored?
The navigation is stored in the `_includes/header.html` folder.

### What is homepage made of by default?
`_includs/home-sample.html` and by default `_includes/blogsHome.html`

### What is `_config.yml` file
This file allows you to specify important site-wide settings such as the site title, description, URL, timezone, and more.

 You can also configure how Jekyll processes your content, such as setting defaults for front matter variables, specifying which files and directories to exclude from the build, and defining collections of content.

 ### Different code snippets
 `page.url != "/"` 

 ### css styles classes
 .text-center
 .mt-3
 .pt-5

 ### How to add a new page with menu item
 New page: 
    _pages folder 👉 add new page
 Menu item: 
    settings.yml 👉 add to `menu_items`
 
 ### What is going on with type on Contact page
 Contact page was setting `type: contact` in it's metadata which/ is used on default.html in an in statement `page.type != "contact`
