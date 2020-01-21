## Boolean expressions

A boolean expression is an expression that can be _reduced_ to a boolean value.

In an `if/else` statement, we only accept boolean expressions.

```js
const isAdult = true;

if (isAdult) {
    console.log('You may drink a beer.');
} else {
    console.log('The bar cannot serve you.');
}
```

In the above example, `isAdult` needed no reduction, as it was in fact a boolean value. We produce boolean expressions using _boolean operators_.

```js
const age = 25;
const isAdult = age >= 18;
```

The boolean comparison operator here is `>=`, which means "greater than or equal to". The other boolean operators are:

```js
const is25loose = age == 25;           // is equal to 25 or "25"
const is25strict = age === 25;         // is equal to 25, but not "25" (strict equality)
const isNot25loose = age != 25;        // not equal to 25 or "25".
const isNot25strict = age !== 25;      // is not equal to 25 (strict inequality).
const higherThan20 = age > 20;         // is higher than, and not including 20.
const lowerThan20 = age < 20;          // is lower than, and not including 20.
const higherThanOrEqual20 = age >= 20;
const lowerThanOrEqual20 = age <= 20;

const negated = !(age == 25);          // any expression can be negated using exclamation

const isAdult = true;
const isNotAdult = !isAdult;           // no parentheses needed when prefixing a boolean
```

Beside comparisons, a boolean expression can also consist of conjunctions (AND) and disjunctions (OR), as well as parentheses.

```js
const money = 8.00;
const age = 21;
const isVisiblyDrunk = false;

const cheapestDrinkInBar = 9.50;

// Bar will serve you if you are of minimum age, have money and you are not visibly drunk
const barWillServeYou = age >= 18 && cheapestDrinkInBar <= money && !isVisiblyDrunk;
```

However, the bar will always serve a famous person, no matter what.

```js
const isFamous = true;
const barWillServeYou = (age >= 18 && cheapestDrinkInBar <= money && !isVisiblyDrunk) || isFamous;
```

The expression can be built from multiple stages of variable assignments. This is true for any variable declaration, not just boolean ones.

The order of boolean evaluation will not matter unless it produces side effects (which is a more advanced topic).

```js
const isOldEnough = age >= 18;
const hasEnoughMoney = cheapestDrinkInBar <= money;

const barWillServeYou = isFamous || isOldEnough && hasEnoughMoney && !isVisiblyDrunk;
```

In the above example, if the person is famous, the evaluation will be _short-circuited_, which means that the rest of the expression will not be evaluated.

## Tasks

The frightening theme park ride "Hellcoaster" have several strict requirements that need to be met in order to ride it.

- You must be 10 years of age or in the company of an adult.
- Even if you are in the company of an adult, you cannot ride if you are less than 8 years of age.
- Minimum height requirements are 100 cm for all riders.
- You cannot be visibly intoxicated when entering the ride.

**Implement the function that tests if a given person can ride on Hellcoaster. Name it well, and make sure it takes all required arguments.**

Test the function on this set of candidates:

- Mark, with his adult wife, 36 years, 176 cm, visibly intoxicated.
- Thomas, riding alone, 10 years of age, 99 cm, appears sober.
- Lisa, riding alone, 6 years of age, 112 cm, appears sober.
- Sara, with her husband, 23 years of age, 164 cm, appears sober.
- William, with his mother, 9 years of age, 129 cm, appears sober.