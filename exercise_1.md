## Accessing an array item by index

Given an array:

```js
const names = [
    "George Walker Bush",
    "Angela Merkel",
    "Alexander Boris de Pfeffel Johnson",
];
```

We can access a specific item in the list using

```js
const first = names[0];
const last = names[2];
const lastForAnyArray = names[names.length - 1];
```

## The string `.split()` method

A `string` has a split method, which splits the string into an array of strings using a _delimiter_ as its first argument.

```js
const name = "Kristian Videmark Parkov";
const names = name.split(" ");

// ["Kristian", "Videmark", "Parkov"]
```

## The array `.length` property

Like a `string`, an `array` has a length property. In a string, `length` is equal to the number of characters in the string. In an array, `length` is equal to number of items in the array.

## The task

Given a list of names:

```js
const names = [
    "George Walker Bush",
    "Angela Merkel",
    "Alexander Boris de Pfeffel Johnson",
];
```

We want to output some infortion for each name. Each line should contain this information:

- The name.
- The length of the name.
- The number of names the person has ().
- Whether the person has any middle names (`true` if they have at least one middle name, `false` if not).
- The surname (last name) of the person.