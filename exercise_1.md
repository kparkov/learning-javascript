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
// The first item is always index 0.
const first = names[0];

// This is only the last in an array of three
const last = names[2];

// This is the last element in any array
const lastForAnyArray = names[names.length - 1];
```

## The string `.split()` method

A `string` has a split method, which splits the string into an array of strings using a _delimiter_ as its first argument. The delimiter is the "split point", and will be excluded from the resulting array.

```js
const name = "Kristian Videmark Parkov";
const names = name.split(" ");

// ["Kristian", "Videmark", "Parkov"]
```

## The array `.length` property

Like a `string`, an `array` has a length property. In a string, `length` is equal to the number of characters in the string. In an array, `length` is equal to number of items in the array.

```js
const fruits = ["Apple", "Orange", "Banana"];

const numberOfFruits = fruits.length;
```

## The task

Create a new project in your learning repository.

Copy this code to your program as the first statement:

```js
const names = [
    "George Walker Bush",
    "Angela Merkel",
    "Alexander Boris de Pfeffel Johnson",
];
```

We want to loop through all the names, outputting some information about each entry:

- The full name.
- The length of the name.
- The number of names the person has in total.
- Whether the person has any middle names (`true` if they have at least one middle name, `false` if not).
- The surname (last name) of the person.

All of the information above should automatically update if we change the contents of the array.