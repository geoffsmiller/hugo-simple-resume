# Simple Resume Theme

The Simple Resume theme for Hugo is a simple one-pager resume template, based on [digitalcraftsman's port](https://github.com/digitalcraftsman/hugo-strata-theme) of [HTML5UP](https://html5up.net/)'s Strata theme to Hugo. It's mostly a simplification of the Strata theme, along with a few minor tweaks and additions to make it suitable for easily converting a resume into a clean, responsive web page.

![Screenshot](https://raw.githubusercontent.com/geoffsmiller/hugo-simple-resume/master/images/screenshot.png)

## Installation

Inside the folder of your Hugo site run:

    $ git clone https://github.com/geoffsmiller/hugo-simple-resume.git

For more information read the official [setup guide](https://gohugo.io/overview/installing/) of Hugo.


## Getting started

After installing the Simple Resume Theme successfully it requires just a few more steps to get your site finally running.


### The config file

Take a look inside the [`exampleSite`](https://github.com/geoffsmiller/hugo-simple-resume/tree/master/exampleSite) folder of this theme. You'll find a file called [`config.toml`](https://github.com/geoffsmiller/hugo-simple-resume/blob/master/exampleSite/config.toml). Copy it to the root folder of your Hugo site. Feel free to customize this theme as you like.

### Sidebar

The sidebar provides a small overview of who you are. One of the first elements that will be spotted is the avatar in the sidebar. Replace it with a nice picture of you by either swapping the default [`avatar.jpg`](https://github.com/geoffsmiller/hugo-simple-resume/blob/master/static/images/avatar.jpg) or by setting a new path to an image in [`config.toml`](https://github.com/geoffsmiller/hugo-simple-resume/blob/master/exampleSite/config.toml):

```toml
[params.sidebar]
    avatar = "avatar.jpg"
```

The path is relative to [`./static/images`](https://github.com/geoffsmiller/hugo-simple-resume/tree/master/static/images).

Last but not least, you can add some other details such as your phone number, location, social media links (WordPress, GitHub, LinkedIn, etc.), and a link to a PDF copy of your resume.

### Build up your resume
The resume has four main sections that can be configured in [`config.toml`](https://github.com/geoffsmiller/hugo-simple-resume/blob/master/exampleSite/config.toml)

* Summary
* Skills
* Experience
* Education

For the most part, these are self explanatory. The Summary takes a single `content` attribute for its text. The other sections take headings, subheadings, bullet points, etc. Each section has its own partial layout in [`./layout/partials`](https://github.com/geoffsmiller/hugo-simple-resume/tree/master/layouts/partials). Edit as needed to suit your needs.

### Nearly finished

In order to see your site in action, run Hugo's built-in local server.

    $ hugo server

Now enter [`localhost:1313`](http://localhost:1313) in the address bar of your browser.

To be able to access your site from anywhere, use the following:

    $ hugo server --bind=[Your IP] --port=80 --baseURL=https://example.com --appendPort=false

## Changelog

All modifications to this theme are listed in the [Changelog](https://github.com/geoffsmiller/hugo-simple-resume/blob/master/CHANGELOG.md).

## Contributing

Did you find a bug? Do you have an idea for a new feature? Feel free to use the [issue tracker](https://github.com/geoffsmiller/hugo-simple-resume/issues) to let me know. Or simply make a [pull request](https://github.com/geoffsmiller/hugo-simple-resume/pulls).


## License

This theme is released under the Creative Commons Attribution 3.0 Unported  License. For more information read the [License](https://github.com/geoffsmiller/hugo-simple-resume/blob/master/LICENSE.md).


## Annotations

Thanks to

- [digitalcraftsman](https://github.com/digitalcraftsman) for porting the theme to Hugo.
- [HTML5UP](https://html5up.net/) for creating the original theme.
- [Steve Francia](https://github.com/spf13) for creating [Hugo](https://gohugo.io) and the awesome community around the project.
