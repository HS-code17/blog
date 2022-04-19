---
layout: "post"
title: "Random code snippets"
---

"Instead of if (x === true), just write if (x).

Instead of if (x === false), just write if (!x) ('if not x').

Your third console.log can't happen, so I'd delete it.

Here's how I'd write the code (different approach; not necessarily better):
let currentPlayer = this.state.xIsNext ? "X" : "O";
console.log("Player ${currentPlayer} has taken a turn.`);"
@strager

"https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Conditional_Operator"

{% highlight javascript %}

function getFee(isMember) {
  return (isMember ? '$2.00' : '$10.00');
}

console.log(getFee(true));
// expected output: "$2.00"

console.log(getFee(false));
// expected output: "$10.00"

console.log(getFee(null));
// expected output: "$10.00"

// Second example

let greeting = person => {
    let name = person ? person.name : `stranger`
    return `Howdy, ${name}`
}

console.log(greeting({name: `Alice`}));  // "Howdy, Alice"
console.log(greeting(null));             // "Howdy, stranger"

// Third example

function example(…) {
    return condition1 ? value1
         : condition2 ? value2
         : condition3 ? value3
         : value4;
}

// Equivalent to:

function example(…) {
    if (condition1) { return value1; }
    else if (condition2) { return value2; }
    else if (condition3) { return value3; }
    else { return value4; }
}

{% endhighlight %}


