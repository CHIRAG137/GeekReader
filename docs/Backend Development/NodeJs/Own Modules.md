---
sidebar_position: 5
---

# Own Modules
You can also create your own modules with the help of NodeJs. For creating your own module, follow the following steps:

**Step : 1**<br/>
Create two different Javascript files in a folder📂 - one for creating your own module and another for importing that module in order to perform operations.

**Step : 2**<br/>
Once the two files are created, open the file where you want to make your own module and start creating your own module. Let us suppose name of your own module file is ```module.js``` and that of your main file is ```index.js```.

``` 
const add = (a, b) => {
    return a + b;
};
const sub = (a, b) => {
    return a - b;
};
module.exports = { add, sub };
```

**Step : 3**<br/>
Once the module is created, now you need to import that module inorder to use that module in the main file.
```
const { add, sub } = require("./module");
console.log(add(3, 4));
console.log(sub(4, 3));
```

**Step : 4**<br/>
Your own module has been created and is ready to use😎.