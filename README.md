# Ember-baseline

I love Ember and I love the skel-baseline framework built by [n33](https://github.com/n33)
So I thought I would create a repo with an ember app with [skel-baseline](https://github.com/n33/skel-baseline) already built into it

I came acros a few problems implemenintng *skel-baseline* into *Ember* first of all, I use grunt to compile *baselines* sass files.
the install skel-baseline package breaks the Ember javascript so I installed jquery and wraped the contents of `bower_components/baseline/assets/js/main.js` in a `$(document).ready(function(){ ... contents of main here ... });`

## Prerequisites

You will need the following things properly installed on your computer.

* [Git](http://git-scm.com/)
* [Node.js](http://nodejs.org/) (with NPM)
* [Bower](http://bower.io/)
* [Ember CLI](http://www.ember-cli.com/)
* [PhantomJS](http://phantomjs.org/)

## Installation

* `git clone https://github.com/olde86/ember-baseline.git my-new-project`

## Rename the application
* `cd my-new-project`

*open package.json*
and change the name to whatever you called the application folder i.e. `my-new-project`
```
{
  "name": "my-new-project",
  ...
```

# Re initiate ember
* `ember init`
* Now you will promted with a very hard quiz.. here are the anwsers
```
[?] Overwrite README.md? No, skip
[?] Overwrite app/index.html? Yes, overwrite
[?] Overwrite app/templates/application.hbs? No, skip
[?] Overwrite bower.json? No, skip
[?] Overwrite config/environment.js? Yes, overwrite
[?] Overwrite ember-cli-build.js? No, skip
[?] Overwrite package.json? No, skip
[?] Overwrite tests/index.html? Yes, overwrite
...
ember does alot of stuff
```

## Hey.. more installation
* `npm install`
* `bower install`

## Fix a bug
* open up `bower_components/baseline/assets/js/main.js`
```
// Wrap everything in main.js in a document ready function

$(document).ready(function () {

  //Contents of main.js goes here

});

```

## Run grunt in a new tab
* `sudo grunt`

## Running / Development

* `ember server`
* Visit your app at [http://localhost:4200](http://localhost:4200).

### Code Generators

Make use of the many generators for code, try `ember help generate` for more details

### Running Tests

* `ember test`
* `ember test --server`

### Building

* `ember build` (development)
* `ember build --environment production` (production)

### Deploying

Specify what it takes to deploy your app.

## Further Reading / Useful Links

* [ember.js](http://emberjs.com/)
* [ember-cli](http://www.ember-cli.com/)
* Development Browser Extensions
  * [ember inspector for chrome](https://chrome.google.com/webstore/detail/ember-inspector/bmdblncegkenkacieihfhpjfppoconhi)
  * [ember inspector for firefox](https://addons.mozilla.org/en-US/firefox/addon/ember-inspector/)

