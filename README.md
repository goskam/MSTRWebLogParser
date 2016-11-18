# MicroStrategy Web log parser

This is a simple browser-based parser built to process and browse through the log files generated by MicroStrategy Web, under MSTRWeb/WEB-INF/log/. This parser should also be able to process log files from the MicroStrategy Mobile server.

This specific project is built with:
* AngularJS + various submodules
* Bootstrap 3

# Live Demo
A live demo of this website can be seen here:
https://tiagosiebler.github.io/MSTRWebLogParser/build/

This demo is a live implementation of the latest code in this repository.

# Basic Usage
## Development 
Installs dependencies and launches development instance in default browser. Any file-changes automatically update browser instance.

1. Install gulp dependencies

	```
	$ npm install -d
	```
2. Run with gulp

	```
	$ gulp
	```


## Production Build
The production build produces a zip file, or can be accessed directly via the build directory.

1. Install gulp dependencies

	```
	$ npm install -d
	```
2. Build with gulp

	```
	$ gulp build
	```


# Project Structure
##### src
Contains all source code that is modified and should be optimized in any way:
* HTML
* JavaScript modules
* CSS

##### build
Contains production-ready project with heavy code optimization.

##### dev
Contains development instance of project with minimal code processing for easier debugging. Debugger statements are not removed here.

##### gulpfile.js
Gulp tasks used to automate build & optimization process. 
* Clean project (e.g .DS_Store files)
* Minify HTML
* Concatenate and minify JS resources into two files
* Concatenate, optimize and minify custom CSS files
* Archive production-ready zip of project

For information on gulp refer to: https://github.com/gulpjs/gulp

##### package.json
npm depencenies for project.

Screenshots
-----------
To be added later.

![Alt text](https://raw.githubusercontent.com/tiagosiebler/repo/master/screenshots/screen1.png "Main Interface")

![Alt text](https://raw.githubusercontent.com/tiagosiebler/repo/master/screenshots/screen2.png "Versions Interface")