# Class 10 Reading Notes

## Ch. 10 - Error Handling & Debugging
Debugging code is easier when we break down the 'execution contexts' into two categories or stages, and stacks. This will make the process of deduction easier. Specifically, we can use the `try`, `catch` and `finally` statements to help us. 

We should use the `try` statement if we think we know the area that might throw an error. However, if an error is thrown, we need a corresponding `catch` block to than 'catch' it. If we do not use a `catch` statement, then we must use a `finally`, although it is possible to use both. It should also be noted that these are not the only statements we can use, for example, we can also use the `continue` statement. 

The `catch` block is essentially like an ` if else ` statement, where as the `finally` is like an `else`, in that the `finally` runs no matter what, at the end, regardless of whether or not the `catch` statement does or does not execute; regardless of whether or not the code throws and error. Another option not mentioned is the `throw` statement. 

When looking at a meta-approach, or 'workflow' of debugging, we first need to look at where the problem seems to be, and then what kind of problem it seems to be. Breakpoints are extremely helpful to this end. In fact, taking small chunks of code for testing is an excellent technique. Using the console, we can:

1. check if objects exist
1. call functions to see their return value
1. write and check values

There are exactly 7 types of errors within JavaScript, each one assigned its own object. These inlcude:

1. TypeError
1. ReferenceError
1. SyntaxError
1. RangeError
1. URIError
1. NaN
1. EvalError

There is, however, in addition to this, the generic error, which might constitute an 8th type. Finally, it is worth mentioned that the code executes not only top down by lines, yes, but also by execution contexts. Thus, particular lines or blocks may be waiting while others are 'stacked' on top. These execution contexts break down into three different categories, as follows:

1. Global Context
1. Function Context
1. Eval Context

Reference errors can be due to one (or more) of three possibilities. The object cannot be referenced, which we are trying to referenced, because it has not been declared, it has been declared wrong, (ie. typo) or it is null. 

The following can throw a syntax error:

```js

var dale = 'dale';

function() {
    console.log(dale; //notice the missing parenthesese....
}


Range errors can happen when trying to access an index in an array that is beyond the array\'s length