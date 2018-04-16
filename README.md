Gulp frontend boilerplate
---
(based on [Una Kravets' gulp boilerplate](https://github.com/una/gulp-starter-env))

What's set up here:

- Sass (LibSass)
- Autoprefixer
- CSS Minification
- JSHint
- Scss Lint (based on [this](https://github.com/causes/scss-lint/blob/master/config/default.yml) config)
- HTML Minification
- BrowserSync
- Image Minification
- GH-Pages deployment from dist/ folder
- Twig Templates

## To Get Started:

1. Install node and make sure npm (Node Package Manager) is also [installed](http://blog.nodeknockout.com/post/65463770933/how-to-install-node-js-and-npm)
2. Clone this repo with `git clone https://github.com/una/gulp-starter-env <your-project-name>` to build this repo into your own project or download the zip
3. In terminal, `cd` (change directory) to the folder containing your project.
4. Run `rm -rf .git` to remove the Git file from the repo and `git init` for a clean history
4. `npm install` to download dependancies
5. In the terminal, enter `gulp` to make everything run
6. Take note of the Access URLs provided in your terminal. Your web page should pop up at `http://localhost:3000`. You can access this same page on your various devices in the same wifi network with the provided External URL. You can share the External URL with coworkers and they'll see whats on your screen.
7. Edit your Sass code inside of the scss folder. You can make subfolders inside of that to better organize your code. Prefix your sass files with an underscore. More info on using @import to organize your files [here](http://sass-guidelin.es/#main-file)
8. Your minified files will be automagically created and updated in `dist/`. It will create your optimized css, html, and javascript files for you. Never edit files within the `dist/` folder. (Dist stands for Distribution)
9. Twig templates and partials are stored in `src/` and are rendered out the server docroot `dist`.
10. Keep gulp running while you're making changes. When you want to close out of the gulp task, in the terminal, hit `ctrl + C`

## Notes on using Twig.js for Gulp
1. Twig.js for gulp uses a subset of features from Twig for PHP. Differences are [listed here](https://github.com/twigjs/twig.js/wiki/Implementation-Notes)