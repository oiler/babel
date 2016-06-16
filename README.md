# babel
for writing es6, a basic install of babel &amp; gulp

## how we got there
1. `git init babel`
2. `npm init`
3. `npm install --save-dev babel-preset-es2015`
4. create .babelrc `{ "presets": ["es2015"] }`
5. `npm install --save-dev gulp`
6. `npm install --save-dev gulp-babel`
7. create gulpfile.js
```
const gulp = require('gulp');
const babel = require('gulp-babel');
gulp.task('default', function() { 
    // source to dist
    gulp.src("src/*.js")
        .pipe(babel())
        .pipe(gulp.dest("dist"));
});
```

## what to do next
1. write your es6 code in any js file inside the `src` folder (src/*.js)
2. run `gulp`
3. review your es5 code inside the corresponding `dist` folder (dist/*.js)

