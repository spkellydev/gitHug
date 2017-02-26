Octogotcha powered by GitHug (Gulp, Jekyll, Pug, Sass, Particle, with AutoPrefixer &amp; BrowserSync)
=============================

This project utilizes front-end technologies with the Particle Photon Board. The user is able to send or recieve a hug digitally. The project was intended to create an anti-harassment program for buddy-clients of the Particle Photon

## System Preparation

To use this starter project, you'll need the following things installed on your machine.

1. [Jekyll](http://jekyllrb.com/) - `$ gem install jekyll`
2. [NodeJS](http://nodejs.org) - use the installer.
3. [GulpJS](https://github.com/gulpjs/gulp) - `$ npm install -g gulp` (mac users may need sudo)

## Local Installation

1. Clone this repo, or download it into a directory of your choice.
2. Inside the directory, run `npm install`.

## Usage

**development mode**

This will give you file watching, browser synchronisation, auto-rebuild, CSS injecting etc etc.

```shell
$ gulp
```

**jekyll**

As this is just a Jekyll project, you can use any of the commands listed in their [docs](http://jekyllrb.com/docs/usage/)

## Deploy with Gulp

You can easily deploy your site build to a gh-pages branch. First, follow the instructions at [gulp-gh-pages](https://github.com/rowoot/gulp-gh-pages) to get your branch prepared for the deployment and to install the module. Then, in `gulpfile.js` you'll want to include something like the code below. `gulp.src()` needs to be the path to your final site folder, which by default will be `_site`. If you change the `destination` in your `_config.yml` file, be sure to reflect that in your gulpfile.



```javascript
var deploy = require("gulp-gh-pages");

gulp.task("deploy", ["jekyll-build"], function () {
    return gulp.src("./_site/**/*")
        .pipe(deploy());
});
```
## GitHug Octogothcha

The Octogotcha, powered by GitHug, is a program for buddy-clients with Particle Photon boards. The project is intended to send hugs digitally to people whom broadcast that they need a hug with digital signals. Hack Harassment is a coalition of organizations and individuals who share in the common goal of building a more inclusive and supportive online community. We are attempting to bridge the gap between the solace associated with breadboard testing and the bullying that can come attached in some cases. 
