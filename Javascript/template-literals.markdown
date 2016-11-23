# Template literals

A common task in any programming language is to concatenate and format strings. 

You have probably found yourself writing code similar to the following many times: 

```javascript
var greeting = "Hi " + name;
```

Template Literals provide a mode succinct and readable form allowing us to specify values to be replaced within the string by surrounding it with curly braces and a dollor sign.

Note how the string itself is also enclosed with the backtick characters instead of ' or ":

```javascript
var name = "Enki";
var greeting = `Hello ${name}`;
//"Hello Enki"
```

We can also use template literals to spread our declaration across mulitiple lines: 

```javascript 
var name = "Enki"; 
var greeting = `Hellp ${name}
Enki
Enki`; 

/*
"Hello Enki
Enki
Enki"
*/
```

We can even use expressions within the placeholders: 

```javacript
var x=1;
var y=2; 
var test = `Hello ${x + y}`;
//Hello 3
```

Note if for some reason you wanted to use a backtick in your expression this can be done by escaping it with a backslash e.g. 

```javascript 
var greeting - `hello \``;
```
