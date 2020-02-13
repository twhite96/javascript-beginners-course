# Strings

## String indices

Every string has a `.length` prop. You do not need to have parens around the `.length`. String length is also counts whitespace.

- .`length` is always one greater than the last index.
- Cannot change strings with reassignment; they are immutable.

## String methods

- Using a method on a string creates a reference to a new string; it does not mutate a string
- `.trim()` removes whitespace from leading and trailing spaces in strings
- `indexOf()` tells you what the index of a substring or character is
  - `indexOf()` only shows you the index of the first match
  - If the index is not found, it will return `-1`
- `.slice()` takes a slice of an existing string and gives you a piece of it
  - "baseball".slice(4) will start at index `0` to the fourth index, which will return `ball`
  - passing two indices: first parameter is the start of the slice, and the second parameter is where you want the slice to res.end();
    - The end of the slice is not inclusive so `"baseball".slice(0,4) gives us "base"

## Escape characters

- use a backslash before the single and double quotes to escape quotes: `"He said \"I ain't happy\""`

## Template literals

We can embed information inside template literals

- `${1+5}` evaluates to `6`
  - `You owe me ${100 + 50}` evaluates to "You owe me 150

```js
let animal = 'pig'
let sound = 'oink'

`${animal} says ${sound}`

// "pig says oink"
```

- Template literals avoid needing to concatenate strings
  - In other languages this is called *string interpolation*

Another example

```js
let item = apples
let price = 1.99
let quantity = 4

`You bought ${quantity} ${item}, total price: $${price*quantity}`;

// "You bought 4 apples, total price: $7.96"
```
