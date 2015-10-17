# All in one Console API
This repository contains some samples of using the Console API. All the essential methods of Console API are included with a sample in [README.md](README.md).

----

## What's Console API?

The Console API provides web applications with methods for writing information to the console, creating JavaScript profiles, and initiating a debugging session.

----

## Non-standard
see [developer.mozilla.org](https://developer.mozilla.org/en-US/docs/Web/API/Console)

>
This feature is non-standard and is not on a standards track. Do not use it on production sites facing the Web: it will not work for every user. There may also be large incompatibilities between implementations and the behavior may change in the future.".

----

## Methods

### console.log(object[, object, ...])
Writes a message to the console. You may pass as many arguments as you'd like, and they will be joined together in a space-delimited line.

```javascript
console.log('This is a sample log');
```


### console.debug(object[, object, ...])
Writes a message to the console, including a hyperlink to the line where it was called.

```javascript
console.debug('I am debug message');
```

### console.info(object[, object, ...])
Writes a message to the console with the visual "info" icon and color coding and a hyperlink to the line where it was called.

```javascript
console.info('I just want to share info!');
```

### console.warn(object[, object, ...])
Writes a message to the console with the visual "warning" icon and color coding and a hyperlink to the line where it was called.

```javascript
console.warn('Be quite! Big brother is watching you!');
```

### console.error(object[, object, ...])
Writes a message to the console with the visual "error" icon and color coding and a hyperlink to the line where it was called.

```javascript
console.error('Something goes wrong!');
```

### console.assert(expression[, object, ...])
Tests that an expression is true.  If not, it will write a message to the console and throw an exception.

```javascript
console.assert((2 + 3) === 5); // Assertation true
console.assert((2 * 1 * 0) === 3, 'It should be 0!'); // Assertation faild
```

### console.clear()
Clears the console.

```javascript
console.clear();
```

### console.dir(object)
Prints an interactive listing of all properties of the object.

```javascript
console.dir(document.body);
```


### console.dirxml(node)
Prints the XML source tree of an HTML or XML element.

```javascript
console.dirxml(document.body);
```

### console.trace()
Prints an interactive stack trace of JavaScript execution at the point where it is called.

```javascript
console.trace();
```

The stack trace details the functions on the stack, as well as the values that were passed as arguments to each function.

### console.group(object[, object, ...])
Writes a message to the console and opens a nested block to indent all future messages sent to the console. Call `console.groupEnd()` to close the block.

```javascript
console.group('Group log is started:');
```

### console.groupCollapsed(object[, object, ...])
Like `console.group()`, but the block is initially collapsed.

```javascript
console.groupCollapsed('Group log is started (collapsed):');
```

### console.groupEnd()
Closes the most recently opened block created by a call to `console.group()` or `console.groupCollapsed()`

```javascript
console.groupEnd();
```

### console.time(name)
Creates a new timer under the given name. Call `console.timeEnd()` with the same name to stop the timer and print the time elapsed.

```javascript
console.time('timer');
```

### console.timeEnd(name)
Stops a timer created by a call to `console.time(name)` and writes the time elapsed.

```javascript
console.timeEnd('timer');
```

### console.timeStamp(name)
Creates a time stamp.

```javascript
console.timeStamp('timeStamp');
```

### console.profile([title])
Turns on the JavaScript profiler.

```javascript
console.profile('my-profile');
```

### console.profileEnd()
Turns off the JavaScript profiler and prints its report.

```javascript
console.profileEnd('my-profile');
```

### console.count([title])
Writes the number of times that the line of code where `count` was called was executed.

```javascript
console.count('count this line!');
```

### console.table(data[, columns])
Allows to log provided data using tabular layout.

```javascript
console.table(["apples", "oranges", "bananas"]);
```

----

## More info
* [developer.chrome.com](https://developer.chrome.com/devtools/docs/console-api)
* [developer.mozilla.org](https://developer.mozilla.org/en-US/docs/Web/API/Console)
* [getfirebug.com](https://getfirebug.com/wiki/index.php/Console_API)
