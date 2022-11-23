---
sidebar_position: 3
---

The Node.js **file system** module allows you to work with the file system on your computer. The <font color="red"> Synchronous Mode </font> of file system module takes a ```single API``` request at a time. In Synchronous mode, the output is obtained line by line irrespective of time taken by each line of code.


## Include fs Module
To use **File System** module on your system, use <font color="red"> ```require('')``` </font> method :
``` 
const fs = require('fs')
```

## Writing in a File
```writeFileSync()``` method is used when you want to overwrite the already written text in the file. If there exits no such file then it creates a new file with the mentioned text.
```
fs.writeFileSync('file.txt', "message");
```

## Appending a File
```appendFileSync()``` method is used when you do not want to overwrite the text already present in the file rather you want to write something in the file just after the already present text.
```
fs.appendFileSync('file.txt', "message");
```

## Reading the File in Buffer Data Format
```Buffer Data``` means data in streams of <font color="red"> binary form </font>. For reading the file, we use ```readFileSync()``` method. To read the file in **Buffer** format: 
```
const data = fs.readFileSync('file.txt');
console.log(data);
```

## Reading the File in String Format
For reading the file, we use ```readFileSync()``` method. To read the file in **String** format we have two methods:<br/>
- **UTF-8** Method<br/>
``` UTF-8``` decodes any given UTF-8-encoded string (byteString) as UTF-8, and returns the UTF-8-decoded version of the string. It is used for converting the <font color="red"> buffer data to string data </font>
```
fs.readFileSync('file.txt', 'utf-8');
```
- **toString()** Method<br/>
```toString()``` method converts the <font color="red"> buffer data to string data </font>
```
const data = fs.readFileSync('file.txt');
console.log(data.toString());
```

## Renaming a File
```renameSync``` method is used to rename a file name to another name.
```
fs.renameSync('file.txt', 'new.txt');
```

## Deleting the text file
```unlinkSync``` method is used for deleting the <font color="red"> .txt file </font>.
```
fs.unlinkSync('file.txt');
```

