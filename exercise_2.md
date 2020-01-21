## Functions 101

A function takes zero or more _arguments_, which is input values it uses to produce and output or _return value_.

```js
// This function adds the Danish VAT to a price and returns the total.
function withAddedVat(amount) {
    const vat = 0.25;
    const priceVat = amount * vat;
    const total = amount + priceVat;
    
    return total;
}

const basePrice = 8.00;
const priceWithVat = withAddedVat(basePrice);

// priceWithVat should be 10.
```

The declaration of a function has no immediate effect on the execution of the program. Only when it is **called** does the code inside get executed. It gets executed anew everytime it is called.

## Exercises

- Create a function that adds two numbers, x and y, to produce a sum.
- Create a function that takes a name as a string, and returns only the last name.
- Create a function that any three items, x, y and z, and produces an array containing all three.
- Create a function that takes an array of numbers, and returns the sum total of those.