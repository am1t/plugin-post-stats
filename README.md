# Micro.blog Plugin - Posts Stats
A Micro.blog plugin that adds a `/stats` page to your site to display the stats about all the published posts. A sample screenshot of the stats page is displayed below. And there's a lot more, [demo here](https://www.amitgawande.com/stats/).

![Plugin Posts Stats Screenshot](https://raw.githubusercontent.com/am1t/plugin-post-stats/main/static/images/poststats.png?raw=true)

This plugin is built for Micro.blog by [@amit](https://micro.blog/amit).

### Installing the plug-in

The plugi-in is avialble in the Micro.blog Plug-in directory. Just make sure you are logged in to your account, go to the "Plug-ins" section and click "Find Plug-ins". Install "Posts Stats by @amit".

Once installed, you should see a new Menu entry for "Stats" pointing to `/stats`. **Note** that the first run may take some time to display the correct stats.

### Word Count and Post Count as Shortcodes

The plugin also publishes you words count and posts count as shortcodes. You can use `{{< poststats/wordcount >}}` or `{{< poststats/postcount >}}` annywhere on your markdown pages. These would be replaced by the respective values.

### Removing Stats from menu

There is no configuration as of now to not show the new page in the Menu. However, you can achieve that by either of the two ways.

1. "On the web, logged in to your blog go to the design section and click the Edit Custom Themes button. The next page should show a list of themes and plugins. Click on Post Stats plugin. Then you'll see all the associated files. Click on content/stats.md . Edit the menu line to remove the word between speech marks, so you end up with: menu: ''" - [h/t Miraz Jordan](https://micro.blog/Miraz/12310468)
2. "Add [custom CSS](https://help.micro.blog/t/custom-css/54): `nav a[href='/stats/'] { display: none; }`" - [h/t Sven Dahlstrand](https://micro.blog/sod/12310306) 

### Planned Features

* [x] Include stats for posts with images, audio (handled by category)
* [x] Chart for posts by year

### Change Log

**Version 1.1:** Released 26th January, 2022
- Added a line chart for posts by year (based on Chart.js)
- Added support of category cloud (h/t: [Mert Bekir](https://mertbakir.gitlab.io/about/))
- Added stat to show the longest post
- Fixed minor styling issues 

**Version 1.0.1:** Released 28th December, 2021
- Display larger number with commas (digits grouped on thousands)

**Version 1.0:** Released 27th December, 2021
- First version with a sperate Stats page
- Includes stats summary and posts stats grouped by year and category
