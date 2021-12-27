# Micro.blog Plugin - Posts Stats
A Micro.blog plugin that adds a `/stats` page to your site to display the stats about all the published posts. A sample screenshot of the stats page is displayed below. And there's a lot more, [demo here](https://www.amitgawande.com/stats/).

![Plugin Posts Stats Screenshot](https://raw.githubusercontent.com/am1t/plugin-post-stats/main/static/images/poststats.png?raw=true)

This plugin is built for Micro.blog by [@amit](https://micro.blog/amit).

### Installing the plug-in

Here are the steps to add the plugin to your Site. Note that once the plugin is added to the Micro.blog directory, this would not be required.

1. Make sure you are signed in to [Micro.blog](https://micro.blog). Add new plugin to your custom theme by [following this link](https://micro.blog/account/themes/new?plugin=1). You can also go to `Design` → `Edit Custom Themes` → `New Plug-in`.

2. Enter a *Title* (like Posts Stats) and enter *Clone URL* as `https://github.com/am1t/plugin-post-stats`.

3. Choose the Site on which you want to install the plug-in.

4. Click "Add Plug-in"

5. The plug-in should be available in the plugins list now.

### Word Count and Post Count as Shortcodes

The plugin also publishes you words count and posts count as shortcodes. You can use `{{< wordcount >}}` or `{{< postcount >}}` annywhere on your markdown pages. These would be replaced by the respective values.


### Include stats in the custom theme (one liner)

You can also include a one-liner as part of your custom theme on any page (screenshot below).

![Plugin Posts Stats Screenshot Short](https://raw.githubusercontent.com/am1t/plugin-post-stats/main/static/images/posts-stats.png?raw=true)

1. Create a new custom themeby following [this link](https://micro.blog/account/themes/new). Or you can edit your existing custom theme by going to `Design` → `Edit Custom Themes` and click on your theme.

2. Open the template you want to add the stats to. For example, to add the stats to the archive page, click on the template `layouts/list.archivehtml.html`

3. Add this partial call as per your liking `{{ partial "posts_stats.html" . }}`.

4. Click *Update Template*. You should see a section added to the respective page.

5. You can style this stats section by adding a rule for class `post-stats` in your `.css`. A reference is shown below.

```
.post-stats {
	background: yellow;
}
```

### Planned Features

* [ ] Include stats for posts with images, audio
* [ ] Chart for posts by year
