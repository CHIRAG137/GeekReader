---
sidebar_position: 4
---

## Include the OS Module
```
const os=require('os');
```

## Architecture of the Operating System
```
console.log(os.arch());
```

## Free memory of the Operating System
```
const freemem = os.freemem();
console.log(`${freemem}` / 1024 / 1024 / 1024);
```

## Total Memory of the Operating System
```
const totmem = os.totalmem();
console.log(`${totmem}` / 1024 / 1024 / 1024);
```

## Finding the Temporary Directory
```
console.log(os.tmpdir());
```

## Type of the Operating System
```
console.log(os.type());
```

## Platform of the Operating System
```
console.log(os.platform());
```

## Hostname of the Operating System
```
console.log(os.hostname());
```