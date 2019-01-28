# Web-Dev-Starter-Pack
This is a simple file structure and development workflow, using the taskrunner GULP.JS. Download this starter-pack and you'll have a basic starting point for a small project!

# How to use?

### Step 1
Downloaded these files from github and unzip/unpack!

### Step 2
Assuming you have Node and NPM installed and up to date, once you have the files downloaded and unzipped, you will need to 'npm install' from your command line or terminal. (make sure you execute this command from inside the proper directory!)

Take a look at the package.json file to see all the dev dependencies that are used! Once you use 'npm install' the node package manager will download all the required packages to your local machine!

### Step 3
From a fresh terminal or command line, type 'gulp watch' and hit enter. This will initialize a live server on your local host and you can start developing! Gulp will watch all the files necessary and render your new code live in real time!

## The File Structure
The expected way to use this stucture is as follows: You have 2 main folders in this structure. The SRC folder and the BUILD folder. The SRC folder is where all your SASS, Javascript, and Images begin. This is where you code from!  Once you deploy your app, all you need is the BUILD folder!

Once the gulpfile.js notices changes in any SASS or JS in the SRC folder(upon save) it will compile and minify it and put it into a new file in the BUILD folder. The BUILD folder consists of CSS, JS, IMG and you can see that the files are suffixed with a '.min' which indicates that they are minified! 

The GULP FLOW will automatically compile and compress all SASS and JS (and also minify your images) and put them in the appropriate place in the BUILD folder. An easy way to think about it is, you build in the BUILD folder and serve it up from the SRC folder. The index.html file is located in the build folder of course and is already linked to the 'main.min.css' and 'main.min.js' so al lyou have to do is write your code in the SRC folder and gulp does the rest! 

## Workflow Notes (Gulp)
There is a pretty nice gulp workflow I set up for this project so feel free to use it! It does not have source maps or anything fancy because this project is pretty simple. You can easily add it however. My workflow will compile sass in real time, minify all images, javascript(es6 compatible), and css, then render on a live browser through local host! Check out the gulpfile.js to see it!