## Synopsis

gally.js is a lightweight gallery management Javascript library, deployable as a means of attributing images dynamically entirely through client-side code.

## Code Example


gally.js will target and hyperlink HTML elements specified by their id and set said element’s text and href to appropriate attribution information as provided. Gally.js is client-side and is dependant on the file hierarchy information it is provided and requires numerical image file organization. For example:

    ├───/images/
    │   │
    │   ├───/hermes/
    │   │       1.jpg
    │   │       2.jpg
    │   │       3.jpg
    │   │
    │   ├───/hubert/
    │   │       1.jpg
    │   │       2.jpg
    |   |

By including the following in a `.html` file body:

    Background photo by: <a id="credit" class="active" href="#" >None</a>
    <script type="text/javascript">
        addAuthour("hermes", 3, "http://hermes.example", "Hermes Conrad");
        addAuthour("hubert", 2, "http://hubert.example", "Hubert Farnsworth");
        setBackgroundImage("credit");
    </script>

The webpage will choose an available image at random, set the image as the page background, and set the innerHTML and href of the hyperlink “credit” to the correct attribution name and website of the displayed image.

## Motivation

This project began as a one-time solution to dynamic landing page image attribution for randomly selected background images on [acorn30](http://acorn30.com/) subsidiary side [Neighbourhood Domains](http://neighbourhooddomains.com/). It was since expanded into a deployable Javascript library which can be freely and easily modified to support a variety of small-scale gallery applications entirely through client side code.

## Installation

Simply obtain the gally.js file from this GitHub repository and add it the appropriate Javascript containing folder on your site, or deploy directly via RawGit.

## API Reference

[View the documentation here.](https://rawgit.com/acorn30/gally/master/jsdoc/index.html)

## Tests

[A detailed series of examples are available on the acorn30labs blog post for gally.js.](http://acorn30.com/dynamic-image-attribution-javascript/)

## Contributors

Contributions welcome! Though initially developed entirely by [Elisha Sarkis](https://github.com/e-sarkis/) at [acorn30](http://acorn30.com/) internally, gally.js is an MIT lisence free and open source project as of this repository’s initialization.

## License

See LICENSE.
