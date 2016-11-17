# Writing Gulp Tasks 

The first step when using *gulp* is to require gulp in the *Gulpfile*. The require statement tells Node to look in the `node_modules` folder for a package named *gulp*. 

```javascript
var gulp = require('gulp');
```

The `gulp` variable is used to create a *gulp* task:

```javascript
gulp.task('task name goes here', function() {
	// task code goes here...
});

For example: 

```javascript 
gulp.task('enki_task', function() {
	console.log('Enki does gulp!');
});
```

The above code is ran on the command line by: 

`gulp enki_task`

Outputs to the console: 

`Enki does gulp!`

from [**Enki**](https://www.enki.com/)