### Find the size of a file

Synchronously

```javascript
const fs = require("fs");

const path = "./test.txt";

console.log(fs.statSync(path)["size"]);
```

Asynchronously
```javascript
const fs = require("fs");

const path = "./test.txt";

fs.stat(path, (err, stat) => 
    err 
        ? console.log(err) 
        : console.log(stat["size"]));
```

This returns the file size in bytes

### Get working directory

```javascript
process.cwd();
```

The keyword `__dirname` returns the same output.

### 