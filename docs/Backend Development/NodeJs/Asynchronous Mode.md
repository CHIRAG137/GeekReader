---
sidebar_position: 3
---

The Node.js file system module allows you to work with the file system on your computer.

## Include fs Module
``` 
const fs = require('fs')
```

## Writing in a File
```writeFile``` function overwrites the already written text in the file. If there exits no such file then it creates a new file with the mentioned text.
```
fs.writeFile('file.txt', "message",()=>{
    console.log("Operation completed Successfully");
});
```

## Appending a File
```appendFile``` does not overwrite the text in file.txt.
```
fs.appendFile('file.txt', "message",()=>{
    console.log("Operation completed Successfully");
});
```

## Reading the File
```
const data = fs.readFile('file.txt','UTF-8',(data)=>{
    console.log(data);
});
```

## Renaming a File
```rename``` is the function used to rename a file name.
```
fs.rename('file.txt', 'new.txt',()=>{
    console.log("Operation completed Successfully");
});
```

## Deleting the text file
```unlink``` is the function used for deleting the text file.
```
fs.unlink('file.txt',()=>{
    console.log("Operation completed Successfully");
});
```
