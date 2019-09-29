+++
title = "Reading & Writing Files (fs)"
date = "2019-09-29"
draft = false
pinned = false
image = "/img/fs.png"
+++
## File System
The Node.js file system module allows us to work with the file system on our computer.
To include the File System module, use the require() method:
``` javascript
const fs = require('fs');
```
**All file system operations have synchronous and asynchronous forms.**    
> The asynchronous form always takes a completion callback as  its last argument. The arguments passed to the completion callback depend on the method, but the first argument is always reserved for an exception. If the operation was completed successfully, then the first argument will be null or undefined.
### Here is an example of the asynchronous version:
``` javascript
const fs = require('fs');

fs.unlink('/tmp/hello', (err) => {
  if (err) throw err;
  console.log('successfully deleted /tmp/hello');
});
```

### Common use for the File System module:

* Read files
* Create files
* Update files
* Delete files
* Rename files
## Read Files
The `fs.readFile()` method is used to read files on your computer.

```javascript
var fs = require('fs');

fs.readFileSync('readMe.txt', 'utf8');
console.log(readMe)
```
### Here is the synchronous version:

```javascript
const fs = require('fs');

fs.unlink('/tmp/hello', (err) => {
  if (err) throw err;
  console.log('successfully deleted /tmp/hello');
});
```