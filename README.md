## Website Performance Optimization portfolio project

The objective of the project is to optimize [this portfolio](https://github.com/udacity/frontend-nanodegree-mobile-portfolio) for speed! The strategy, is to optimize the critical rendering path and make this page render as quickly as possible by applying the techniques picked up in the [Critical Rendering Path course](https://www.udacity.com/course/ud884).

### Website Running Instructions:

* Open `index.html` in a web browser (Preferably Google.chrome)
* This website is a template for simple portfolio developed by **Cameron Pittman** (_Udacity_ tutor). It showcases some of his projects and teaching work
* They are provided as _weblinks_ as follows:
  * Build your own 2048
  * Website Peformance Optimization
  * Mobile Web Development
  * Cam's Pizzeria
* Out of these, **Cam's pizzeria** has major functionality. It provides for ordering of Pizzas with good features of animation

### What I did to achieve the objective of this project:

* To get started, I downloaded the entire directory, **website optimization** and followed the below-mentioned methodology to optimize this web-site.

#### Page load speed optimization:

* Image compression: Images were rescaled and resized to suit to the final layout dimensions.
* Inline CSS: Styles are inlined and applied to the document immediately, instead of render-blocking and loading. This was done using online compression techniques.
* Defer alternative media CSS: A media attribute was added to print stylesheets to ensure that it would only be downloaded when printing.
* Minifying CSS and JavaScript : All CSS and JavaScript files were minified _but not obfuscated_ to ensure faster downloading.
* **Note:** Though minified, the original files are still present in the respective directories - without `.min` in the name - for study and clear understanding.

#### Frame rate optimization

* Unnecessary JavaScript operations were pulled out of for loops, whereever possible, in `views/js/main.js`.
* The number of pizzas to be displayed on the screen was made dynamic in `views/js/main.js`.
* The pizza size function was modified in `views/js/main.js`.

#### The output of page-speed insights and Average scripting time to generate last 10 frames are as follows:
* [Scripting Time](https://gvsrohita.github.io/website-optimization/SUPPORTING-DOCS/AVG-SCRIPTING-TIME-TO-GENERATE-LAST-10-FRAMES.png)
* [PageSpeed Insights - Desktop](https://gvsrohita.github.io/website-optimization/SUPPORTING-DOCS/pagespeed%20insight%20-%20Desktop.jpg)
* [PageSpeed Insights - Mobile](https://gvsrohita.github.io/website-optimization/SUPPORTING-DOCS/pagespeed%20insight%20-%20Mobile.jpg)

##### The Resources used for this project:

* [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/)
* [Optimize CSS Delivery](https://developers.google.com/speed/docs/insights/OptimizeCSSDelivery)
* [Learner, Meaner, Faster Animations with requestAnimationFrame](https://www.html5rocks.com/en/tutorials/speed/animations/)
