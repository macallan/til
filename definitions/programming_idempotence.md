# Programming Idempotence
Programming Idempotence is the idea that calling an idempotent function multiple times will not change the program state beyond the first call. 

> "It won't always be possible to define your operations on data in an idempotent way, but if you can, it will definitely help reduce the chances that your side effects will crop up to break your expectations when you least expect it." - Kyle Simpson

Idempotence is not always possible, but will reduce the likelyhood of bugs popping up. 

Source: [Functional-Light-JS](https://github.com/getify/Functional-Light-JS/blob/master/manuscript/ch5.md/#chapter-5-reducing-side-effects)
