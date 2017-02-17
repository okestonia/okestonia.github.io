# About the website

This site is built with [Lektor](https://www.getlektor.com/).

It has a bunch of dependencies, so do `npm install` and then `npm run build`.

`grunt` will watch for changes to your SCSS files, and also icons (see [svgstore](https://github.com/FWeinb/grunt-svgstore)).

#### Deploying

**WARNING: since this is an organization Github page, the deploy has to be done on the master branch; therefore, all the edits have to be done on the *source* branch.**

`lektor deploy` will deploy to the master branch, putting changes live, if you have deploy permissions.

#### Translations

To translate the site we need to duplicate the `contents.lr` file, and save with the language code in the file name, like `contents+et.lr`.

We also need to add translations to `global-content.ini` and `main-nav.ini`.

If we are adding new language to the site we also need to:

- Add the new language to `languages.json`;
- Add the language to `project.lektorproject`.

