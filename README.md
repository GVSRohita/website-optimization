## Website Performance Optimization portfolio project

The objective of the project is to optimize [this portfolio](https://github.com/udacity/frontend-nanodegree-mobile-portfolio) for speed! The strategy, is to optimize the critical rendering path and make this page render as quickly as possible by applying the techniques picked up in the [Critical Rendering Path course](https://www.udacity.com/course/ud884).

### How to run:

To get started, download the entire directory, **website optimization**, and run it in a browser locally to achieve a page speed score of above 90 on desktop as well as mobile.

#### Page load speed optimization:

* Image compression: Images were rescaled and resized to the final layout dimensions.
* Inline CSS: Styles are inlined and applied to the document immediately instead
 of blocking loading. This was done using online compression techniques.
* Defer alternative media CSS: A media attribute was added to print stylesheets
 to ensure that it would only be downloaded when printing.
* Minifying CSS and JavaScript : All CSS and JavaScript files were minified
 _but not obfuscated_ to ensure faster downloading. The formatted and indented
 files are still present in their respective directories, without the
 `.min` extensions to their filenames.

#### Frame rate optimization

* Unnecessary JavaScript operations were pulled out of for loops where possible,
 in `views/js/main.js`.
* The number of pizzas to be displayed on the screen was made dynamical in `views/js/main.js`.
* The pizza size function was modified in `views/js/main.js`.

##### Furthur areas of improvement

* Browser caching, could have reduced page loading time.
* Using a CDN for Bootstrap files could have reduced page loading time as well,
 but was minified for the purposes of this exercise.

##### Resources

* [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/)
* [Optimize CSS Delivery](https://developers.google.com/speed/docs/insights/OptimizeCSSDelivery)
* [Learner, Meaner, Faster Animations with requestAnimationFrame](https://www.html5rocks.com/en/tutorials/speed/animations/)
