# About the website

This site is built with [Lektor](https://www.getlektor.com/).

It has a bunch of dependencies, so do `npm install` and then `npm run build`.

`grunt` will watch for changes to your SCSS files, and also icons (see [svgstore](https://github.com/FWeinb/grunt-svgstore)).

#### Editing

Since this is an organization Github page, the deploy has to be done on the master branch; therefore, all the edits have to be done on the *source* branch. To do so, after cloning the repo with `git clone`, enter the folder and run `git checkout source`.

#### Translations

In order to add a translation to the site, we need to:

- add the language to `project.lektorproject`;
- add the new language to `databags/languages.json`;
- add translations to `databags/global-content.ini` and `databags/main-nav.ini`.

Then, to translate the content we can:

- manually duplicate each `contents.lr` file in the `content/` folder (and its subfolders) and save it with the language code in the file name (like `contents+et.lr`), or
- use the `admin` interface when running the site locally, e.g. by running `lektor server` and opening `localhost:5000/admin` on a browser.

#### Deploying

**WARNING: since this is an organization Github page, this command will deploy on the *master* branch.** (See the [Editing](#editing) section for details).

`lektor deploy` will deploy to the master branch, putting changes live, if you have deploy permissions.

