---
sidebar_position: 3
---
File System Module is used for accessing the file in a directory.

## Include fs Module
``` 
const fs = require('fs')
```

## Writing in a File
```writeFileSync``` function overwrites the already written text in the file. If there exits no such file then it creates a new file with the mentioned text.
```
fs.writeFileSync('file.txt', "message");
```

## Appending a File
```appendFileSync``` does not overwrite the text in file.txt.
```
fs.appendFileSync('file.txt', "message");
```

## Reading the File in Buffer Text Format
```
const data = fs.readFileSync('file.txt');
console.log(data);
```

## Reading the File in String Format
**Method - 1**
```
fs.readFileSync('file.txt', 'utf-8');
```
**Method - 2**
```
const data = fs.readFileSync('file.txt');
console.log(data.toString());
```

## Renaming a File
```renameSync``` is the function used to rename a file name.
```
fs.renameSync('file.txt', 'new.txt');
```

## Deleting the text file
```unlinkSync``` is the function used for deleting the text file.
```
fs.unlinkSync('file.txt');
```
