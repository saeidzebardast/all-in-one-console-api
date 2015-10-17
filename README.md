# All in one Console API
This repository contains some samples of using the Console API. All the essential methods of Console API are included with a sample in [README.md](README.md) and [index.html](index.html).

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

### console.debug(object[, object, ...])
Writes a message to the console, including a hyperlink to the line where it was called.

### console.info(object[, object, ...])
Writes a message to the console with the visual "info" icon and color coding and a hyperlink to the line where it was called.

### console.warn(object[, object, ...])
Writes a message to the console with the visual "warning" icon and color coding and a hyperlink to the line where it was called.

### console.error(object[, object, ...])
Writes a message to the console with the visual "error" icon and color coding and a hyperlink to the line where it was called.

### console.assert(expression[, object, ...])
Tests that an expression is true.  If not, it will write a message to the console and throw an exception.

### console.clear()
Clears the console.

### console.dir(object)
Prints an interactive listing of all properties of the object.

### console.dirxml(node)
Prints the XML source tree of an HTML or XML element.

### console.trace()
Prints an interactive stack trace of JavaScript execution at the point where it is called.

The stack trace details the functions on the stack, as well as the values that were passed as arguments to each function.

### console.group(object[, object, ...])
Writes a message to the console and opens a nested block to indent all future messages sent to the console. Call <code>console.groupEnd()</code> to close the block.

### console.groupCollapsed(object[, object, ...])
Like <code>console.group()</code>, but the block is initially collapsed.

### console.groupEnd()
Closes the most recently opened block created by a call to <code>console.group()</code> or <code>console.groupCollapsed()</code>

### console.time(name)
Creates a new timer under the given name. Call <code>console.timeEnd()</code> with the same name to stop the timer and print the time elapsed.

### console.timeEnd(name)
Stops a timer created by a call to <code>console.time(name)</code> and writes the time elapsed.

### console.timeStamp(name)
Creates a time stamp.

### console.profile([title])
Turns on the JavaScript profiler.

### console.profileEnd()
Turns off the JavaScript profiler and prints its report.

### console.count([title])
Writes the number of times that the line of code where <code>count</code> was called was executed.

### console.exception(error-object[, object, ...])
Prints an error message together with an interactive stack trace of JavaScript execution at the point where the exception occurred.

### console.table(data[, columns])
Allows to log provided data using tabular layout.

----

## More info
* [developer.chrome.com](https://developer.chrome.com/devtools/docs/console-api)
* [developer.mozilla.org](https://developer.mozilla.org/en-US/docs/Web/API/Console)
* [getfirebug.com](https://getfirebug.com/wiki/index.php/Console_API)
