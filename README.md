# Getting Started

## Callbacks

You will use node.js in this example.

1. Create a new file. The first line should be:

        const fs = require('fs');

2. Display a message (console.log) saying that the program is watching `myfile.txt` for changes.
3. Now use the `fs.watch` API call. This function takes two arguments: a file to watch for changes, and a callback that will be called whenever the file changes:

        fs.watch('myfile.txt', callback);

    Have the callback display a message on the console indicating that the file has changed.
4. Create the empty file ('myfile.txt'). Now run your program (node mywatcher.js). Ensure that the program displays a new message each time the file is changed.
Note that file or directory are not necessarily consistent between operating systems.

## Closures

### Create a Counter

To start with, you will create a function that works like this:

    var mycounter = counter(7);
    mycounter.increment();
    var next = mycounter.get();     // 8
    console.log(next);


1.	So `Counter` is a simple function. What kind of thing does it need to return?
2.	Where does it maintain its state (the current value of the counter)?
3.	Implement the Counter function and test it with the code above.


### Create a Fibonacci Sequence Generator

Create a Fibonacci sequence generator function. It should work like this:

```
var f = fibgen();
console.log(f);	// 1
console.log(f);	// 1
console.log(f);	// 3
console.log(f);	// 5
console.log(f);	// 8
...
```

### Fix this Bug

The following code has a bug. Find it and fix it.

```
<!DOCTYPE html>
<html>
<head>
<title>Test</title>
</head>
<body>
<section>
	<header>
		<h1>Closure Example</h1>
	</header>
	<ul>
		<li class="fruit">Apple</li>
		<li class="fruit">banana</li>
		<li class="fruit">pear</li>
	</ul>
	<p class="fruit">durian</p>

</section>
<script>

var fruit = document.getElementsByClassName('fruit');

for (var i = 0; i < fruit.length; i++) {
	fruit[i].addEventListener('click', function(e) {
		alert("Event listener number" + i);
	});
}

</script>
</body>
</html>
```

## Mountain Trail App

1.	Review the JavaScript content of your mobile app codebase. Analyze it for opportunities to refactor into simpler functions. Perform your refactoring.
2.	When would closures be appropriate for use in your app?




