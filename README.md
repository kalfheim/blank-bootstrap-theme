# Blank-Bootstrap

Blank scaffold for [OctoberCMS](https://github.com/octobercms/october) which includes [Twitter Bootstrap](http://getbootstrap.com/), [jQuery](https://jquery.com/) and [Font Awesome](https://fortawesome.github.io/Font-Awesome/). Built using [Less](http://lesscss.org/).

## Installation

`$ php artisan theme:install krisawzm.blank-bootstrap <theme-dir>`

Replace `<theme-dir>` with whatever fits the site you're building.

## Activating the theme

`$ php artisan theme:use <name>`

Where `<name>` is whatever you specified in `theme:install`.

## Post installation

You can choose for yourself how you add your own styling. My recommendation is creating a subdirectory in `assets/less` for the project you're building. This theme ships with `assets/less/site` - keep it or delete it.

### Customizing Bootstrap

Customize Bootstrap variables by adding them in `assets/less/twbs/custom-variables.less`

Choose which Less components you wish to include in `assets/less/twbs/custom-components.less`

### JavaScript

Choose which Bootstrap jQuery plugins you wish to include in the layout file (`layouts/default.htm`). To minimize the file size, you should only include the plugins you actually will be using.

This theme includes the `@framework` and `@framework.extras` JS assets in the layout file. They can be removed unless you actually will be using them.

### Removing Font Awesome

- Remove `@import` statement in `assets/less/app.less`
- Delete directory `assets/less/fa`
- Delete directory `assets/vendor/font-awesome`

### Other files

`README.md` may be deleted.

`version.yaml` may be deleted.

`theme.yaml` should be emptied (not deleted).

`assets/images/theme-preview.png` should either be deleted or replaced with a screenshot of your final theme.

This scaffold also includes the @jquery, @framework and @framework.extras JS assets in layouts/default.htm which can be removed unless you're planning on using them.

Consult the [official documentation](https://octobercms.com/docs/themes/development) for more information on theme development.
