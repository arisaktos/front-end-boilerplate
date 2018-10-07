## Template for developing front end websites

### Requirements: node, gulp

To initialize go to your directory and install all packages:

cd [your_directory] 

npm init 

npm install

### Packages included: 
gulp-sass - to compille sass to css 

browser-sync - for live-reloading

gulp-useref - concatenation of files  
Special markup is required to combine files:
```
    <!-- build:css css/combined.css -->
    <link href="css/one.css" rel="stylesheet">
    <link href="css/two.css" rel="stylesheet">
    <!-- endbuild -->
```

gulp-uglify - minifying JavaScript files 

gulp-if - to make sure only js/css is minified

gulp-cssnano - minifying css 

gulp-imagemin - optimizing images 

gulp-cache - so we don't optimize images that are already optimized 

del - for cleaning files (removes dist folder) 

run-sequence - to make sure tasks run in a correct order 


### Also includes:
- placeholder CSS Media Queries (responsive.scss)
- jquery cdn
- normalize.css cdn



### Folder structure:

[app]    
- [css]    
- [img]    
- [js]    
- [scss]    
- index.html 

[dist] 

### Commands to use:
- gulp - for starting watcher and live browser preview
- build - changes scss into css, combines files and minifies them, optimizes images, moves final versions to dist folder
