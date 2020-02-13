# Mathematical Operations with Variables

We know. Math scares some people. Some people break out in hives just at the mention of math. It's ok. We're not going to be doing any advanced math. Just simple addition, subtraction, multiplication and division.

No calculus.

No algebra.

Simple stuff.

Oh, you're also going to using numeric values and string values so that you can see how they can work together.

## Adding

We'll start off with something that you've already done in a previous chapter. Use variables and the `+` sign to add two values together. Keep in mind that you are not adding two variables together here, you are adding two values. Those values are simply being represented by a human-readable word.

```js
const femaleChildren = 2
const maleChildren = 1
```

Assume you want to build an application that lets a parent provide data about how many female, and how many male, children he has. You then also want to display the total number of children he has. Therefore, you need to keep all three values stored in three different variables.

Here, then, is the third variable.

```js
const totalChildren = femaleChildren + maleChildren
```

See, nothing scary. Just simple addition.

There is another way to write that code, though. You are going to use a new operator. Instead of only using the `+` operator, you are going to use the `+=` operator. You are also going to use both the `let` and the `const` keywords for declaring variables.

Let's get started.

```js
let totalChildren = 0
const femaleChildren = 2
const maleChildren = 1
```

With the above code, you start the `totalChildren` variable with an initial value of 0, and then after the other two variables have been declared, you will need to add those values to the 0 one at a time. You will use the new `+=` operator.

```js
totalChildren += femaleChildren
totalChildren += maleChildren
```

Here's the `+=` operator translated into English.

"Take the current value assigned to the variable on the left, and add the value of the variable on the right. Take that sum and update value of the variable on the left."

In code, here's what happens.

```js
totalChildren = 0 + 2   // New value of totalChildren is 2
totalChildren = 2 + 1   // New value of totalChildren is 3
```

## Subtraction

Subtractions works much like you would expect. Take a look at the following code and reflect on if you can understand its purpose.

```js
let netIncome = 0
const monthlyIncome = 2308.56

const cableBill = 109.99
const electricBill = 58.04
const gasBill = 19.43
const waterBill = 39.93

netIncome = monthlyIncome - cableBill
netIncome -= electricBill
netIncome -= gasBill
netIncome -= waterBill
```

## Exercise: Combined Income and Expenses

Your turn to try adding and subtracting variables.

* You have a monthly income of $4388.12
* Your husband has a monthly income of $3512.98
* Your monthly internet access bill is $158.99
* Your monthly water bill is $68.33
* Your monthly electric bill is $129.03
* Your monthly car fuel expenses are $295.68
* Your monthly food expenses are $503.12

Here's what you need to output to the console. Replace the `xxx` text with the correct amount. Use addition and subtraction to come up with the right values. Use string interpolation to build the final output string.

Remember that string interpolation requires the backtick character and `${variableHere}` syntax to inject a variable's value into a string.

```html
Our combined monthly income is xxx. Our net monthly income is xxx.
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTcyNjYzNDYxN119
-->