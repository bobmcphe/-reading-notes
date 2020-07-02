# Javascript Callstack

Callstacks are synchronous - but this doesn't mean that you cannot have a parallel stack running due to an asynch call, such as you would have with AJAX. 

Keeping it simple, a callstack is simply a datastructure. It's like a basket, using a Last In, First Out method. While Javascript reads from top to bottom, it does not necessarily execute in that manner. Hence, the callstack. 

This brings up an interesting term and question: "What is a stack overflow?"

Charles Freeborn answers:

"A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error."

To summarize, a callstack is single-threaded, executing one function or line of code at a time; doing so in a synchronized manner; working in a Last In, First Out manner -- all of which resides in temporary memory. 

# Javascript Error Messages and Debugging

<img src="https://miro.medium.com/max/1000/1*LHpmsxV3f2znpxhuAFuIqA.png"
     style="float: left; margin-right: 10px;" />

This is a sample of an error, the green is the overall error message, the light blue is to note if the error was properly handled, the brownish (dark yellow) is the type of error and the red is the call stack

It is helpful to note that the following (sample) code was used to create the above error:

```
(function testing(){
  var obj = {
    add
  }
  function add(a, b) {
    var result = a + b
    return result.split('')
  }
  var stringResult = obj.add("1", "2")
  var result = obj.add(1, 2)
})()
```

It is important to note that the red is the callstack, which is why understanding the callstack is important for debugging.

You can get several different types of errors, as defined below:

1. syntax - Due to a typo or, as the example provided says, due to parsing something using JSON.parse that is not able to be parsed.
1. range - this can be due to providing an invalid length of, say, an array.
1. reference - when you refer to an item that is not yet declared or defined.
1. type - the item (number, string, boolean, object, etc), is not compatible with what is required, and is the most frequent issue


Javascript is not a 'compiled language' such as Java. Thus, you can only see the errors, (normally), after you execute the code. But, there are a few ways to get around this. For example, you could install and use Quokka, which checks your code as you type and/or eslint, a javascript linter which can help prevent errors.

Since being a coder means being able to debug and solve broken code, debugging is crucial. 