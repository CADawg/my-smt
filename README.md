# MySMT

[![forthebadge](https://forthebadge.com/images/badges/powered-by-electricity.svg)](https://forthebadge.com) [![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](https://forthebadge.com) [![forthebadge](https://forthebadge.com/images/badges/built-by-developers.svg)](https://forthebadge.com) [![forthebadge](https://forthebadge.com/images/badges/contains-technical-debt.svg)](https://forthebadge.com) [![forthebadge](https://forthebadge.com/images/badges/uses-css.svg)](https://forthebadge.com) [![forthebadge](https://forthebadge.com/images/badges/uses-html.svg)](https://forthebadge.com) [![forthebadge](https://forthebadge.com/images/badges/uses-js.svg)](https://forthebadge.com) [<img src="https://steemitimages.com/p/3W72119s5BjWMGm4Xa2MvD5AT2bJsSA8F9WeC71v1s1fKfGkK9mMKuc3LcvF4KigbWg9UsrpENy2vPnRmG8ycCNPiMXfiADKLPkgAdPhCk89VwKTtjJwEv?format=match&mode=fit" alt="drawing" height="35px"/>](https://utopian.io)


MySMT is a fully customisable SMT site template created by [@cadawg](https://steemit.com/@cadawg), it follows the design principles from [this task request](https://steemit.com/@surpassinggoogle/utopian-based-task-request-kindly-help-us-building-the-landing-page-for-teardrops-smt-additional-bounty-of-100-steem), as I didn't get to do the task, but I wanted to make a site similar to it.

I hope this will be useful to someone creating a SMT site for their project.

### How To Build Custom SASS themes:

Edit `scss/custom.scss` like so:

```scss

@charset "utf-8";

/* Purple for this theme (Main Theme Color) */
$primary: #A349A4;

/* Other Custom Colours */
$danger: #ED1C24;
$success: #22B14C;
$info: #7092BE;


/* Use Bulma to build - Get the latest version from https://bulma.io and copy the contents of the bulma-x.x.x/sass folder into sass/bulma_styles */
@import "bulma.sass";

```

Then build the css, minify it and copy it to `bulma-custom.min.css`

Also, edit the last lines in `styles.css` like so:

```css
/*Customisable*/

.card-content.is-primary {
    background-color: #A349A4; /* Should match is-primary from bulma */
    color: #ffffff; /* Contrasting color to is-primary */
}
```

Then you can run it just by opening index.html.

Edit index.html to your liking - Just keep the licence entact and follow the terms of the [AGPL](https://www.gnu.org/licenses/agpl-3.0-standalone.html)!
