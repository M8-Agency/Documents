# M8 Agency Development Stack Guide

## HTML

* Semantic HTML - Learn the concept of semantics and the semantic meaning of most HTML tags. Learn the main structure tags, `header`, `main`, `footer`, `section`, `aside`, etc. We write our HTML in the most semantic way possible.

* Advanced HTML5 forms: learn the new HTML5 `input` tags and their browser support, and how to change their styling in CSS and detect their values in JavaScript.

* Learn about the new HTML5 video element, the major supported video codecs on browsers and how to manipulate the video element with CSS.

* What are data attributes? We use them quite often to store miscellaneous data that can't be displayed to the user but is used on JavaScript.


## SVG

* Learn what [SVGs](https://developer.mozilla.org/en-US/docs/Web/SVG/Tutorial/Introduction) are and their advantages over bitmaps.

* We use the [SVG symbols](https://css-tricks.com/svg-symbol-good-choice-icons/) spritesheet technique to hold all our SVGs. Learn more: [Icon system](https://css-tricks.com/svg-sprites-use-better-icon-fonts/), [External SVG file](https://css-tricks.com/svg-use-external-source/).

* Research how SVG images can be modified with CSS with fills, strokes, etc.


## CSS/Sass

* Understand the [Cascade](https://developer.mozilla.org/en-US/docs/Web/CSS/Cascade) part of CSS (Cascading Style Sheets). Read up on CSS specificity and how the browser chooses what CSS to apply when there are multiple rules in different classes.

* Understand the CSS box-model. Learn how the browser calculates dimensions by default with the default `content-box` box-model, and its difference with the `border-box` box model. All of our sites use the `border-box` box model so dimensions are calculated differently than normal. [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/box_model), [CSS Tricks](https://css-tricks.com/the-css-box-model/)

* Understand the CSS Flexible Box (or flexbox) layout mode. Child elements in a flexbox can be laid out in any direction and can have flexible dimensions to adapt to the display space. [Using CSS Flexible Boxes at MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Using_CSS_flexible_boxes)

* Pseudo-elements, `::after` and `::before`. They are sprinkled throughout all of our projects, sometimes for really major visual elements.  Learn how to use them to minimize unsemantic markup for presentational purposes.

* Vendor prefixes. We automate the prefixing process with [Autoprefixer](https://github.com/postcss/autoprefixer), but this is basic knowledge for front-end CSS development. You should know their purpose and why automating the process is ideal.

* The BEM class syntax. Most of our CSS is written with BEM classes and looks fugly at first sight, so it's important you understand what's going on. [CSSWizardry](http://csswizardry.com/2013/01/mindbemding-getting-your-head-round-bem-syntax/)

* Learn the basics of the Sass preprocessor, and what are mixins, functions and map lists.

* We seek to adhere strictly to these master documents of [CSS](http://cssguidelin.es/) and [SASS](https://sass-guidelin.es/) guidelines.

* More important stuff
    * [When to use @extend; when to use a mixin](http://csswizardry.com/2014/11/when-to-use-extend-when-to-use-a-mixin/)
    * [The specificity graph](http://csswizardry.com/2014/10/the-specificity-graph/)


## JavaScript

* JavaScript Libraries and Frameworks to study:
  - Currently in-use for production work:
      - [AngularJS](https://angularjs.org/)
      - [Angular](https://angular.io/)
      - [Sails](http://sailsjs.com/)
  - Our future:
      - [React](https://facebook.github.io/react/)
      - [React Native](https://facebook.github.io/react-native/)
      - [Redux](http://redux.js.org/)

* Let's seek to use vanilla JavaScript exclusively for most of our projects unless heavy DOM manipulation is required. This means we are moving away from jQuery. We're doing this because we believe JavaScript is the future and we want to understand it better, even if it's more tedious and will produce more lines of code. [You don't need jQuery](http://blog.garstasio.com/you-dont-need-jquery/), [You might not need jQuery](http://youmightnotneedjquery.com/)

* We're also using [ES6](https://babeljs.io/docs/learn-es6/) features like classes, modules, template strings, and compiling our scripts through [Babel](https://babeljs.io/) to ES5/ES6/ESbugher7.

* We often work with AJAX requests, using `jQuery.ajax` and now using soon-to-be native `window.fetch`. See the [polyfill](https://github.com/github/fetch).


## Performance

* "Images are evil". Understand why they are the number 1 reason websites are slow and bloated. A front-end developer should always have a bias towards doing presentational things with CSS if at all possible, only resorting to images if there is no other choice.

* Learn about page rendering, how images, stylesheets and scripts block it and what is the optimal place to include these files in an HTML document.

* Learn about CSS and JavaScript minification and compression on the server for production. We have this process automated.

* Learn the basic ways of optimizing images, starting with compression levels on Photoshop, optimization software like `optipng`, `jpegtran`, etc.

* Understand how [browser caches](https://developers.google.com/speed/docs/insights/LeverageBrowserCaching) work and how they improve page performance.

* Research about HTTP2, what it means for the web and what best practices that apply to HTTP no longer apply to this new protocol. Our new servers are all HTTP2 enabled, which affects how we optimize our front-end stack.

## Backend

### NodeJS

Need to write some stuff about our NodeJS usage.

### PHP
* We use the [Laravel](http://laravel.com/) PHP framework for most of our projects. For front-end development purposes, learn Laravel's [Blade templates](http://laravel.com/docs/5.4/templates), how to create a [route](http://laravel.com/docs/5.4/routing), a [controller](http://laravel.com/docs/5.4/controllers) method that is called through that route, and how to render a [view](http://laravel.com/docs/5.4/views#basic-usage) through a controller method.

### Python

Need to write some stuff about our Python usage.


## Tools

- [NPM](https://www.npmjs.com/)
- [Yarn](https://yarnpkg.com/en/)
- [Bower](http://bower.io/) to easily install front-end dependencies that are not on npm.

### Scaffolding
- [Yeoman](http://yeoman.io/)
- [Brunch](http://brunch.io/)


### Task Runners
- [Webpack](https://webpack.js.org/)
- [Gulp](http://gulpjs.com/)

## Culture

# CCDA
- **Communication**
- Collaboration
- Discipline
- Agility


## Credits

Most of the credit for this guide goes to my friend [Waldemar Figueroa](https://github.com/waldemarfm), who wrote the original stack guide in our past life.





