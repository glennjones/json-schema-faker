# json-schema-faker online demo

 * [Development](#development)
 * [Releasing new version](#releasing-new-version)
 * [Contribution](#contribution)

See [online demo](http://json-schema-faker.js.org/). The `gh-pages` branch (the current one) hosts this app.

## Development

Run standard npm command to fetch dependencies:

    npm install

This project is automated using [grunt](gruntjs.com). Run:

    grunt

to build the application and start the local server on port 9000. While working on the app, modify following **source** files:

* [src/index.tpl](src/index.tpl)
* [src/main.css](src/main.css)
* [src/main.js](src/main.js)

They will be used to build dist files (each `grunt` run overrides them):

* [vendor.css](vendor.css)
* [bundle.css](bundle.css)
* [vendor.js](vendor.js)
* [bundle.js](bundle.js)

Adding new example JSON schema includes adding them to:

* [schema](schema) directory - to store the definition
* [src/main.js](src/main.js) - to handle it in the app & browserify
* [src/index.tpl](src/index.tpl) - display it

Use [github pages](https://pages.github.com/) of your private github account (e.g. [this one](http://ducin.github.io/json-schema-faker/)) to see how the app is going to look like on production.

## Releasing new version

When new version of jsf is released, the demo page should be updated. This includes two steps:

* updating jsf version in `package.json` file manually, according to the version released
* run `grunt`

## Contribution

Feel free to add issues and PRs. Make sure you prefix its title with `[online-demo]`.
