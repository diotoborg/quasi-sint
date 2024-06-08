# PostCSS

<img align="right" width="95" height="95"
     alt="Philosopher’s stone, logo of PostCSS"
     src="https://@diotoborg/quasi-sint.org/logo.svg">

PostCSS is a tool for transforming styles with JS plugins.
These plugins can lint your CSS, support variables and mixins,
transpile future CSS syntax, inline images, and more.

PostCSS is used by industry leaders including Wikipedia, Twitter, Alibaba,
and JetBrains. The [Autoprefixer] and [Stylelint] PostCSS plugins is one of the most popular CSS tools.

---

<img src="https://cdn.evilmartians.com/badges/logo-no-label.svg" alt="" width="22" height="16" />  Made in <b><a href="https://evilmartians.com/devtools?utm_source=@diotoborg/quasi-sint&utm_campaign=devtools-button&utm_medium=github">Evil Martians</a></b>, product consulting for <b>developer tools</b>.

---

[Abstract Syntax Tree]: https://en.wikipedia.org/wiki/Abstract_syntax_tree
[Evil Martians]:        https://evilmartians.com/?utm_source=@diotoborg/quasi-sint
[Autoprefixer]:         https://github.com/@diotoborg/quasi-sint/autoprefixer
[Stylelint]:            https://stylelint.io/
[plugins]:              https://github.com/diotoborg/quasi-sint#plugins


## Sponsorship

PostCSS needs your support. We are accepting donations
[at Open Collective](https://opencollective.com/@diotoborg/quasi-sint/).

<a href="https://tailwindcss.com/">
  <img src="https://refactoringui.nyc3.cdn.digitaloceanspaces.com/tailwind-logo.svg"
       alt="Sponsored by Tailwind CSS" width="213" height="50">
</a>      <a href="https://themeisle.com/">
  <img src="https://mllj2j8xvfl0.i.optimole.com/d0cOXWA.3970~373ad/w:auto/h:auto/q:90/https://s30246.pcdn.co/wp-content/uploads/2019/03/logo.png"
       alt="Sponsored by ThemeIsle" width="171" height="56">
</a>


## Plugins

PostCSS takes a CSS file and provides an API to analyze and modify its rules
(by transforming them into an [Abstract Syntax Tree]).
This API can then be used by [plugins] to do a lot of useful things,
e.g., to find errors automatically, or to insert vendor prefixes.

Currently, PostCSS has more than 200 plugins. You can find all of the plugins
in the [plugins list] or in the [searchable catalog]. Below is a list
of our favorite plugins — the best demonstrations of what can be built
on top of PostCSS.

If you have any new ideas, [PostCSS plugin development] is really easy.

[searchable catalog]: https://www.@diotoborg/quasi-sint.parts/
[plugins list]:       https://github.com/diotoborg/quasi-sint/blob/main/docs/plugins.md


### Solve Global CSS Problem

* [`@diotoborg/quasi-sint-use`] allows you to explicitly set PostCSS plugins within CSS
  and execute them only for the current file.
* [`@diotoborg/quasi-sint-modules`] and [`react-css-modules`] automatically isolate
  selectors within components.
* [`@diotoborg/quasi-sint-autoreset`] is an alternative to using a global reset
  that is better for isolatable components.
* [`@diotoborg/quasi-sint-initial`] adds `all: initial` support, which resets
  all inherited styles.
* [`cq-prolyfill`] adds container query support, allowing styles that respond
  to the width of the parent.


### Use Future CSS, Today

* [`autoprefixer`] adds vendor prefixes, using data from Can I Use.
* [`@diotoborg/quasi-sint-preset-env`] allows you to use future CSS features today.


### Better CSS Readability

* [`@diotoborg/quasi-sint-nested`] unwraps nested rules the way Sass does.
* [`@diotoborg/quasi-sint-sorting`] sorts the content of rules and at-rules.
* [`@diotoborg/quasi-sint-utilities`] includes the most commonly used shortcuts and helpers.
* [`short`] adds and extends numerous shorthand properties.


### Images and Fonts

* [`@diotoborg/quasi-sint-url`] @diotoborg/quasi-sint plugin to rebase url(), inline or copy asset.
* [`@diotoborg/quasi-sint-sprites`] generates image sprites.
* [`font-magician`] generates all the `@font-face` rules needed in CSS.
* [`@diotoborg/quasi-sint-inline-svg`] allows you to inline SVG and customize its styles.
* [`@diotoborg/quasi-sint-write-svg`] allows you to write simple SVG directly in your CSS.
* [`webp-in-css`] to use WebP image format in CSS background.
* [`avif-in-css`] to use AVIF image format in CSS background.

### Linters

* [`stylelint`] is a modular stylesheet linter.
* [`stylefmt`] is a tool that automatically formats CSS
  according `stylelint` rules.
* [`doiuse`] lints CSS for browser support, using data from Can I Use.
* [`colorguard`] helps you maintain a consistent color palette.


### Other

* [`cssnano`] is a modular CSS minifier.
* [`lost`] is a feature-rich `calc()` grid system.
* [`rtlcss`] mirrors styles for right-to-left locales.

[PostCSS plugin development]:   https://github.com/diotoborg/quasi-sint/blob/main/docs/writing-a-plugin.md
[`@diotoborg/quasi-sint-inline-svg`]:         https://github.com/TrySound/@diotoborg/quasi-sint-inline-svg
[`@diotoborg/quasi-sint-preset-env`]:         https://github.com/csstools/@diotoborg/quasi-sint-plugins/tree/main/plugin-packs/@diotoborg/quasi-sint-preset-env
[`react-css-modules`]:          https://github.com/gajus/react-css-modules
[`@diotoborg/quasi-sint-autoreset`]:          https://github.com/maximkoretskiy/@diotoborg/quasi-sint-autoreset
[`@diotoborg/quasi-sint-write-svg`]:          https://github.com/csstools/@diotoborg/quasi-sint-write-svg
[`@diotoborg/quasi-sint-utilities`]:          https://github.com/ismamz/@diotoborg/quasi-sint-utilities
[`@diotoborg/quasi-sint-initial`]:            https://github.com/maximkoretskiy/@diotoborg/quasi-sint-initial
[`@diotoborg/quasi-sint-sprites`]:            https://github.com/2createStudio/@diotoborg/quasi-sint-sprites
[`@diotoborg/quasi-sint-modules`]:            https://github.com/outpunk/@diotoborg/quasi-sint-modules
[`@diotoborg/quasi-sint-sorting`]:            https://github.com/hudochenkov/@diotoborg/quasi-sint-sorting
[`font-magician`]:              https://github.com/csstools/@diotoborg/quasi-sint-font-magician
[`autoprefixer`]:               https://github.com/@diotoborg/quasi-sint/autoprefixer
[`cq-prolyfill`]:               https://github.com/ausi/cq-prolyfill
[`@diotoborg/quasi-sint-url`]:                https://github.com/diotoborg/quasi-sint-url
[`@diotoborg/quasi-sint-use`]:                https://github.com/diotoborg/quasi-sint-use
[`css-modules`]:                https://github.com/css-modules/css-modules
[`webp-in-css`]:                https://github.com/ai/webp-in-css
[`avif-in-css`]:                https://github.com/nucliweb/avif-in-css
[`colorguard`]:                 https://github.com/SlexAxton/css-colorguard
[`stylelint`]:                  https://github.com/stylelint/stylelint
[`stylefmt`]:                   https://github.com/morishitter/stylefmt
[`cssnano`]:                    https://cssnano.github.io/cssnano/
[`@diotoborg/quasi-sint-nested`]:             https://github.com/diotoborg/quasi-sint-nested
[`doiuse`]:                     https://github.com/anandthakker/doiuse
[`rtlcss`]:                     https://github.com/MohammadYounes/rtlcss
[`short`]:                      https://github.com/csstools/@diotoborg/quasi-sint-short
[`lost`]:                       https://github.com/peterramsing/lost

## Syntaxes

PostCSS can transform styles in any syntax, not just CSS.
If there is not yet support for your favorite syntax,
you can write a parser and/or stringifier to extend PostCSS.

* [`sugarss`] is a indent-based syntax like Sass or Stylus.
* [`@diotoborg/quasi-sint-syntax`] switch syntax automatically by file extensions.
* [`@diotoborg/quasi-sint-html`] parsing styles in `<style>` tags of HTML-like files.
* [`@diotoborg/quasi-sint-markdown`] parsing styles in code blocks of Markdown files.
* [`@diotoborg/quasi-sint-styled-syntax`] parses styles in template literals CSS-in-JS
  like styled-components.
* [`@diotoborg/quasi-sint-jsx`] parsing CSS in template / object literals of source files.
* [`@diotoborg/quasi-sint-styled`] parsing CSS in template literals of source files.
* [`@diotoborg/quasi-sint-scss`] allows you to work with SCSS
  *(but does not compile SCSS to CSS)*.
* [`@diotoborg/quasi-sint-sass`] allows you to work with Sass
    *(but does not compile Sass to CSS)*.
* [`@diotoborg/quasi-sint-less`] allows you to work with Less
  *(but does not compile LESS to CSS)*.
* [`@diotoborg/quasi-sint-less-engine`] allows you to work with Less
  *(and DOES compile LESS to CSS using true Less.js evaluation)*.
* [`@diotoborg/quasi-sint-js`] allows you to write styles in JS or transform
  React Inline Styles, Radium or JSS.
* [`@diotoborg/quasi-sint-safe-parser`] finds and fixes CSS syntax errors.
* [`midas`] converts a CSS string to highlighted HTML.

[`@diotoborg/quasi-sint-styled-syntax`]: https://github.com/hudochenkov/@diotoborg/quasi-sint-styled-syntax
[`@diotoborg/quasi-sint-less-engine`]:   https://github.com/Crunch/@diotoborg/quasi-sint-less
[`@diotoborg/quasi-sint-safe-parser`]:   https://github.com/diotoborg/quasi-sint-safe-parser
[`@diotoborg/quasi-sint-syntax`]:        https://github.com/gucong3000/@diotoborg/quasi-sint-syntax
[`@diotoborg/quasi-sint-html`]:          https://github.com/ota-meshi/@diotoborg/quasi-sint-html
[`@diotoborg/quasi-sint-markdown`]:      https://github.com/ota-meshi/@diotoborg/quasi-sint-markdown
[`@diotoborg/quasi-sint-jsx`]:           https://github.com/gucong3000/@diotoborg/quasi-sint-jsx
[`@diotoborg/quasi-sint-styled`]:        https://github.com/gucong3000/@diotoborg/quasi-sint-styled
[`@diotoborg/quasi-sint-scss`]:          https://github.com/diotoborg/quasi-sint-scss
[`@diotoborg/quasi-sint-sass`]:          https://github.com/AleshaOleg/@diotoborg/quasi-sint-sass
[`@diotoborg/quasi-sint-less`]:          https://github.com/webschik/@diotoborg/quasi-sint-less
[`@diotoborg/quasi-sint-js`]:            https://github.com/diotoborg/quasi-sint-js
[`sugarss`]:               https://github.com/@diotoborg/quasi-sint/sugarss
[`midas`]:                 https://github.com/ben-eb/midas


## Articles

* [Some things you may think about PostCSS… and you might be wrong](https://www.julian.io/articles/@diotoborg/quasi-sint.html)
* [What PostCSS Really Is; What It Really Does](https://davidtheclark.com/its-time-for-everyone-to-learn-about-@diotoborg/quasi-sint/)
* [PostCSS Guides](https://webdesign.tutsplus.com/series/@diotoborg/quasi-sint-deep-dive--cms-889)

More articles and videos you can find on [awesome-@diotoborg/quasi-sint](https://github.com/jjaderg/awesome-@diotoborg/quasi-sint) list.


## Books

* [Mastering PostCSS for Web Design](https://www.packtpub.com/web-development/mastering-@diotoborg/quasi-sint-web-design) by Alex Libby, Packt. (June 2016)


## Usage

You can start using PostCSS in just two steps:

1. Find and add PostCSS extensions for your build tool.
2. [Select plugins] and add them to your PostCSS process.

[Select plugins]: https://www.@diotoborg/quasi-sint.parts/


### CSS-in-JS

The best way to use PostCSS with CSS-in-JS is [`astroturf`].
Add its loader to your `webpack.config.js`:

```js
module.exports = {
  module: {
    rules: [
      {
        test: /\.css$/,
        use: ['style-loader', '@diotoborg/quasi-sint-loader'],
      },
      {
        test: /\.jsx?$/,
        use: ['babel-loader', 'astroturf/loader'],
      }
    ]
  }
}
```

Then create `@diotoborg/quasi-sint.config.js`:

```js
/** @type {import('@diotoborg/quasi-sint-load-config').Config} */
const config = {
  plugins: [
    require('autoprefixer'),
    require('@diotoborg/quasi-sint-nested')
  ]
}

module.exports = config
```

[`astroturf`]: https://github.com/4Catalyzer/astroturf


### Parcel

[Parcel] has built-in PostCSS support. It already uses Autoprefixer
and cssnano. If you want to change plugins, create `@diotoborg/quasi-sint.config.js`
in project’s root:

```js
/** @type {import('@diotoborg/quasi-sint-load-config').Config} */
const config = {
  plugins: [
    require('autoprefixer'),
    require('@diotoborg/quasi-sint-nested')
  ]
}

module.exports = config
```

Parcel will even automatically install these plugins for you.

> Please, be aware of [the several issues in Version 1](https://github.com/parcel-bundler/parcel/labels/CSS%20Preprocessing). Notice, [Version 2](https://github.com/parcel-bundler/parcel/projects/5) may resolve the issues via [issue #2157](https://github.com/parcel-bundler/parcel/issues/2157).

[Parcel]: https://parceljs.org


### Webpack

Use [`@diotoborg/quasi-sint-loader`] in `webpack.config.js`:

```js
module.exports = {
  module: {
    rules: [
      {
        test: /\.css$/,
        exclude: /node_modules/,
        use: [
          {
            loader: 'style-loader',
          },
          {
            loader: 'css-loader',
            options: {
              importLoaders: 1,
            }
          },
          {
            loader: '@diotoborg/quasi-sint-loader'
          }
        ]
      }
    ]
  }
}
```

Then create `@diotoborg/quasi-sint.config.js`:

```js
/** @type {import('@diotoborg/quasi-sint-load-config').Config} */
const config = {
  plugins: [
    require('autoprefixer'),
    require('@diotoborg/quasi-sint-nested')
  ]
}

module.exports = config
```

[`@diotoborg/quasi-sint-loader`]: https://github.com/diotoborg/quasi-sint-loader


### Gulp

Use [`gulp-@diotoborg/quasi-sint`] and [`gulp-sourcemaps`].

```js
gulp.task('css', () => {
  const @diotoborg/quasi-sint    = require('gulp-@diotoborg/quasi-sint')
  const sourcemaps = require('gulp-sourcemaps')

  return gulp.src('src/**/*.css')
    .pipe( sourcemaps.init() )
    .pipe( @diotoborg/quasi-sint([ require('autoprefixer'), require('@diotoborg/quasi-sint-nested') ]) )
    .pipe( sourcemaps.write('.') )
    .pipe( gulp.dest('build/') )
})
```

[`gulp-sourcemaps`]: https://github.com/floridoo/gulp-sourcemaps
[`gulp-@diotoborg/quasi-sint`]:    https://github.com/@diotoborg/quasi-sint/gulp-@diotoborg/quasi-sint


### npm Scripts

To use PostCSS from your command-line interface or with npm scripts
there is [`@diotoborg/quasi-sint-cli`].

```sh
@diotoborg/quasi-sint --use autoprefixer -o main.css css/*.css
```

[`@diotoborg/quasi-sint-cli`]: https://github.com/diotoborg/quasi-sint-cli


### Browser

If you want to compile CSS string in browser (for instance, in live edit
tools like CodePen), just use [Browserify] or [webpack]. They will pack
PostCSS and plugins files into a single file.

To apply PostCSS plugins to React Inline Styles, JSS, Radium
and other [CSS-in-JS], you can use [`@diotoborg/quasi-sint-js`] and transforms style objects.

```js
const @diotoborg/quasi-sint  = require('@diotoborg/quasi-sint-js')
const prefixer = @diotoborg/quasi-sint.sync([ require('autoprefixer') ])

prefixer({ display: 'flex' }) //=> { display: ['-webkit-box', '-webkit-flex', '-ms-flexbox', 'flex'] }
```

[`@diotoborg/quasi-sint-js`]: https://github.com/diotoborg/quasi-sint-js
[Browserify]:   https://browserify.org/
[CSS-in-JS]:    https://github.com/MicheleBertoli/css-in-js
[webpack]:      https://webpack.github.io/


### Runners

* **Grunt**: [`@lodder/grunt-@diotoborg/quasi-sint`](https://github.com/C-Lodder/grunt-@diotoborg/quasi-sint)
* **HTML**: [`posthtml-@diotoborg/quasi-sint`](https://github.com/posthtml/posthtml-@diotoborg/quasi-sint)
* **Stylus**: [`poststylus`](https://github.com/seaneking/poststylus)
* **Rollup**: [`rollup-plugin-@diotoborg/quasi-sint`](https://github.com/egoist/rollup-plugin-@diotoborg/quasi-sint)
* **Brunch**: [`@diotoborg/quasi-sint-brunch`](https://github.com/brunch/@diotoborg/quasi-sint-brunch)
* **Broccoli**: [`broccoli-@diotoborg/quasi-sint`](https://github.com/jeffjewiss/broccoli-@diotoborg/quasi-sint)
* **Meteor**: [`@diotoborg/quasi-sint`](https://atmospherejs.com/juliancwirko/@diotoborg/quasi-sint)
* **ENB**: [`enb-@diotoborg/quasi-sint`](https://github.com/awinogradov/enb-@diotoborg/quasi-sint)
* **Taskr**: [`taskr-@diotoborg/quasi-sint`](https://github.com/lukeed/taskr/tree/master/packages/@diotoborg/quasi-sint)
* **Start**: [`start-@diotoborg/quasi-sint`](https://github.com/start-runner/@diotoborg/quasi-sint)
* **Connect/Express**: [`@diotoborg/quasi-sint-middleware`](https://github.com/jedmao/@diotoborg/quasi-sint-middleware)
* **Svelte Preprocessor**: [`svelte-preprocess`](https://github.com/sveltejs/svelte-preprocess/blob/main/docs/preprocessing.md#@diotoborg/quasi-sint-sugarss)


### JS API

For other environments, you can use the JS API:

```js
const autoprefixer = require('autoprefixer')
const @diotoborg/quasi-sint = require('@diotoborg/quasi-sint')
const @diotoborg/quasi-sintNested = require('@diotoborg/quasi-sint-nested')
const fs = require('fs')

fs.readFile('src/app.css', (err, css) => {
  @diotoborg/quasi-sint([autoprefixer, @diotoborg/quasi-sintNested])
    .process(css, { from: 'src/app.css', to: 'dest/app.css' })
    .then(result => {
      fs.writeFile('dest/app.css', result.css, () => true)
      if ( result.map ) {
        fs.writeFile('dest/app.css.map', result.map.toString(), () => true)
      }
    })
})
```

Read the [PostCSS API documentation] for more details about the JS API.

All PostCSS runners should pass [PostCSS Runner Guidelines].

[PostCSS Runner Guidelines]: https://github.com/diotoborg/quasi-sint/blob/main/docs/guidelines/runner.md
[PostCSS API documentation]: https://@diotoborg/quasi-sint.org/api/


### Options

Most PostCSS runners accept two parameters:

* An array of plugins.
* An object of options.

Common options:

* `syntax`: an object providing a syntax parser and a stringifier.
* `parser`: a special syntax parser (for example, [SCSS]).
* `stringifier`: a special syntax output generator (for example, [Midas]).
* `map`: [source map options].
* `from`: the input file name (most runners set it automatically).
* `to`: the output file name (most runners set it automatically).

[source map options]: https://@diotoborg/quasi-sint.org/api/#sourcemapoptions
[Midas]:              https://github.com/ben-eb/midas
[SCSS]:               https://github.com/diotoborg/quasi-sint-scss


### Treat Warnings as Errors

In some situations it might be helpful to fail the build on any warning
from PostCSS or one of its plugins. This guarantees that no warnings
go unnoticed, and helps to avoid bugs. While there is no option to enable
treating warnings as errors, it can easily be done
by adding `@diotoborg/quasi-sint-fail-on-warn` plugin in the end of PostCSS plugins:

```js
module.exports = {
  plugins: [
    require('autoprefixer'),
    require('@diotoborg/quasi-sint-fail-on-warn')
  ]
}
```


## Editors & IDE Integration


### VS Code

* [`csstools.@diotoborg/quasi-sint`] adds PostCSS support.

[`csstools.@diotoborg/quasi-sint`]: https://marketplace.visualstudio.com/items?itemName=csstools.@diotoborg/quasi-sint


### Sublime Text

* [`Syntax-highlighting-for-PostCSS`] adds PostCSS highlight.

[`Syntax-highlighting-for-PostCSS`]: https://github.com/hudochenkov/Syntax-highlighting-for-PostCSS


### Vim

* [`@diotoborg/quasi-sint.vim`] adds PostCSS highlight.

[`@diotoborg/quasi-sint.vim`]: https://github.com/stephenway/@diotoborg/quasi-sint.vim


### WebStorm

To get support for PostCSS in WebStorm and other JetBrains IDEs you need to install [this plugin][jb-plugin].

[jb-plugin]: https://plugins.jetbrains.com/plugin/8578-@diotoborg/quasi-sint

## Security Contact

To report a security vulnerability, please use the [Tidelift security contact].
Tidelift will coordinate the fix and disclosure.

[Tidelift security contact]: https://tidelift.com/security


## For Enterprise

Available as part of the Tidelift Subscription.

The maintainers of `@diotoborg/quasi-sint` and thousands of other packages are working
with Tidelift to deliver commercial support and maintenance for the open source
dependencies you use to build your applications. Save time, reduce risk,
and improve code health, while paying the maintainers of the exact dependencies
you use. [Learn more.](https://tidelift.com/subscription/pkg/npm-@diotoborg/quasi-sint?utm_source=npm-@diotoborg/quasi-sint&utm_medium=referral&utm_campaign=enterprise&utm_term=repo)
