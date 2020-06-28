class-3-09.md

# Concepts of Functional Programming in JS

Can't read since Medium (which I hardly ever use) is saying I have reached my limit. Interestingly, it allows me to read the following...suggesting perhaps a bug?

# Refactoring Javascrip for Performance and Readability

The short answer is to find middle ground between brevity and clarity - frankly a concept in writing normal english works too.

The only thing I easily can take away from this is to inline the return for a function that provides a basic check capability, such as the example provided:

```
function showProfile(user) {
  // People often inline such checks
  if (user.authenticated === false) { return; }
  // Stay at the function indentation level, plus less brackets
}
```

The second thing I took away is to use descriptive terms, (not a new concept, of course), specifically with loops, such as:

```
function searchGroups(name) {
  for (let i = 0; i < continents.length; i++) {
    const group = continents[i]; // This code becomes self-documenting
    for (let j = 0; j < group.length; j++) {
      const tags = group[j].tags;
      for (let k = 0; k < tags.length; k++) {
        if (tags[k] === name) {
          return group[j].id; // The core of this nasty loop is clearer to read
        }
      }
    }
  }
}
```

The third thing is to see if an API can provide the functionality you need.