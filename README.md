# e.nigma buttons

*e.nigma buttons* is a WordPress plugin that easily allows you to add buttons to your posts, pages etc.

[![Maintainability](https://api.codeclimate.com/v1/badges/23718d5d9155f120cb77/maintainability)](https://codeclimate.com/github/chemiker/e.nigma-buttons/maintainability) [![Build Status](https://travis-ci.com/chemiker/e.nigma-buttons.svg?branch=master)](https://travis-ci.com/chemiker/e.nigma-buttons)
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fchemiker%2Fe.nigma-buttons.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fchemiker%2Fe.nigma-buttons?ref=badge_shield)

## Shortcodes & Attributes
*e.nigma buttons* adds the shortcode `[button]` to your installation. The following options can be used to adjust the button for your needs:

* `label`: The label of your button
* `icon`: The icon of your button
* `link`: The link of your button
* `color`: The color of button
* `border`: yes (default) or no
* `size`: small, medium (default) or large
* `class`: Additional CSS classes that will be added to your buttons icon

### Colors
The following colors are avaible:
* green
* orange
* purple
* cyan
* white
* red
* black

### Icons
*e.nigma buttons* uses [Font Awesome](http://fontawesome.io/) as icon resource. [An overview over all available icons](http://fontawesome.io/icons/) can be found on their website.

## Usage
Most of the shortcodes attributes are self explaining. However, it must be noted that the `icon` attribute can be filled by using modififed [Font Awesome shortcodes](http://fontawesome.io/icons/).

For instance: If you want to use the GitHub icon you would search for that icon in the [list of all icons](http://fontawesome.io/icons/). What you will find is the corresponding CSS class. For *e.nigma buttons* the name of the icon (which is obtained if stripping the "fa-" in the beginning of the CSS class) is used. For GitHub the CSS class would be `fa-github`. Thus, `github` is your value for the `icon` attribute.

### Examples
`[button label="My GitHub account" icon="github" color="orange" link="https://github.com/chemiker"]`
Brings you an linked, medium-sized, orange button that has a GitHub icon and the label "My GitHub account".

`[button icon="github" color="orange" link="https://github.com/chemiker" size="large"]`
Brings you an orange, large-sized, linked GitHub icon.

## FAQ

See the FAQ in the repository [Wiki](https://github.com/chemiker/enigma-buttons/wiki).

## License & copyright
This project is released under the MIT license. 


[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fchemiker%2Fe.nigma-buttons.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fchemiker%2Fe.nigma-buttons?ref=badge_large)

### Icons / Fonts

The plugin uses [Font Awesome](http://fontawesome.io) icons which is a project by Dave Gandy. Font Awesome fonts (Copyright by Dave Gandy) are released under [SIL OFL 1.1](http://scripts.sil.org/OFL). Font Awesome CSS files (shipped as part of this plugin's CSS file) by Dave Gandy are released under [MIT license](https://opensource.org/licenses/MIT).

### Tests

This repository ships with tests. The tests are based on ["sample-plugin"](https://github.com/wp-cli/sample-plugin). The following files are part of the package which is released under GPLv2 (Copyright by Daniel Bachhuber) and have been modified:

* test/*
* bin/*
* .travis.yml
* phpcs.xml.dist
* phpunit.xml.dist

## Development
As the plugin this is real free software you are very welcome to fork this project and do whatever you want with it :)

### Requirements
* yarn

### Installation
1. Download the zip archive or clone the repository to your WordPress plugin directory
2. run `yarn install`
4. run `yarn run gulp dev` to continuously watch the (CSS/PHP) files and compile them if necessary

For distribution you can run `yarn run gulp make`. This will create a `dist/` folder ready for submission to the WordPress.org repository.