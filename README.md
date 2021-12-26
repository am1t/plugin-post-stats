# Micro.blog Plugin - Posts Stats
A Micro.blog plugin that displays stats about all the published posts. A sample screenshot from an archive page displayed below.

![Plugin Posts Stats Screenshot](https://raw.githubusercontent.com/am1t/plugin-post-stats/main/static/images/posts-stats.png)

This plugin is built for Micro.blog by [@amit](https://micro.blog/amit).

### Pre-requisite

You need to set up a custom theme for using this plugin to include the section in the desired page. You can [follow the instructions here](https://help.micro.blog/t/custom-themes/59) to setup a custom theme.

PS: You can even clone the existing theme you are using. So, getting a custom theme is easier than it sounds.

### Installing the plug-in

1. Make sure you are signed in to [Micro.blog](https://micro.blog). Add new plugin to your custom theme by [following this link](https://micro.blog/account/themes/new?plugin=1). You can also go to `Design` → `Edit Custom Themes` → `New Plug-in`.

2. Enter a *Title* (like Posts Stats) and enter *Clone URL* as `https://github.com/am1t/plugin-post-stats`.

3. Choose the Site on which you want to install the plug-in.

4. Click "Add Plug-in"

5. The plug-in should be available in the plugins list now.

6. You can configure the `date` when you had published your first post. Go to "Plug-in" section and press ⚙️ Settings for the above added plugin.

### Include stats in the custom theme

1. Create a new custom themeby following [this link](https://micro.blog/account/themes/new). Or you can edit your existing custom theme by going to `Design` → `Edit Custom Themes` and click on your theme.

2. Open the template you want to add the stats to. For example, to add the stats to the archive page, click on the template `layouts/list.archivehtml.html`

3. Add this partial call as per your liking `{{ partial "posts_stats.html" . }}`.

4. Click *Update Template*. You should see a section added to the respective page.