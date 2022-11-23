---
sidebar_position: 2
---

## What is REPL?
REPL stands for Read-Evaluate-Print-Loop.
- **R** stands for reading operations. It reads the user inputs, parses the input into js data structure and stores in memory.
- **E** stands for eval operations. It takes and evaluates the data structure.
- **P** stands for return or printing the output. It prints the output.
- **L** stands for looping. It loops above command until user presses ctrl+C twice.

Use the REPL mode
```bash
> node
```

Once REPL mode is opened now you can perform operations like
- js expressions
- Multiline loops
- Editor mode

### js expressions
Mathematical operations such as addition, subtraction, multiplication etc can be performed very easily in REPL mode.
```
> 5+6
11
> 6-2
4
```

### Multiline loops
REPL mode can also be used when we need to run a multiline loop.
```
> i=0
... while(i<10){
        console.log(i)
        i=i+1
... }
```

### Editor mode
Run editor mode
```
> .editor
```

Now you can use your terminal as an editor.
```
> i=0
while(i<10){
    console.log(i)
    i=i+1
}
```

To run the **editor program** press ```ctrl+D``` and for leaving the **editor mode** press ```ctrl+C```.

Exit the REPL mode
```
.exit
```

