# EJS

EJS stands for Embedded Javascript, and is a templating engine. 

To set it up, (after installing the npm package), requires setting up a folder named 'vews'. Files that are added to this folder, which will end in .ejs, are able serve as a template which exists on the server side. 

Here is how the code is executed:

```
let template = ejs.compile(str, options);
template(data);
// => Rendered HTML string

ejs.render(str, data, options);
// => Rendered HTML string

ejs.renderFile(filename, data, options, function(err, str){
    // str => Rendered HTML string
});
```

The options which it can use are the following: 

1. cache - Compiled functions are cached, requires filename
1. filename - Used by cache to key caches, and for includes
1. root - Set project root for includes with an absolute path (e.g, /file.ejs). Can be array to try to resolve include from multiple directories.
1. views - An array of paths to use when resolving includes with relative paths.
1. context Function execution context
1. compileDebug When false no debug instrumentation is compiled
1. client - Returns standalone compiled function
1. delimiter
1. openDelimiter
1. closeDelimiter '/li>
1. debug Outputs generated function body
1. strict When set to `true`, generated function is in strict mode
1. _with - Whether or not to use with() {} constructs. If false then the locals will be stored in the locals object. (Implies `--strict`)
1. localsName - Name to use for the object storing local variables when not using with Defaults to locals
1. rmWhitespace - Remove all safe-to-remove whitespace, including leading and trailing whitespace. It also enables a safer version of -%> line slurping for all scriptlet tags (it does not strip new lines of tags in the middle of a line).
1. escape - The escaping function used with <%= construct. It is used in rendering and is .toString()ed in the generation of client functions. (By default escapes XML).
1. outputFunctionName - Set to a string (e.g., 'echo' or 'print') for a function to print output inside scriptlet tags.
1. async - When true, EJS will use an async function for rendering. (Depends on async/await support in the JS runtime.

For more information, see: https://ejs.co/