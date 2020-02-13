# Values of Data in Everyday Life

Software developers work with all kinds of data, produced by all kinds of people and processes. Medical records, food and drink sales, atmospheric condition, transportation patterns... these things all get produced from data.

## Going to the store

For example, imagine you make a trip to the grocery store this weekend. Here's what you buy.

1.  Four oranges
2.  One loaf of bread
3.  Two bags of chips
4.  One gallon of milk
5.  Three cans of tomato sauce

There are two ways to look at that data. First, you can describe the quantity of each thing you bought.

"I bought 4, 1, 2, 1, and 3 at the grocery store"

Of course, people would look at you funny. A better way would be to provide a label for what each of those numbers mean - which is how normal people talk.

"I bought 4 oranges, 1 loaf of bread, 2 bags of chips, 1 gallon of milk, and 3 cans of sauce."

An experienced software developer looks at that sentence very differently than you do. They see it as five, different data points about quantities. Each data point has two parts.

1.  The descriptive label for the quantity    
2.  The quantity itself (i.e. the value of the quantity)

The labels are "oranges", "bread", "bags of chips", "milk", "tomato sauce".
The values are 4, 1, 2, 1, 3

## Second trip to the store

Two weeks later, you need to make another trip to the store. However, on this trip, the data is different. You buy the same things, but in different quantities because you know your sister is coming over for the weekend.

1.  Seven oranges
2.  Two loaves of bread
3.  Three bags of chips
4.  One gallon of milk
5.  Six cans of tomato sauce

Again, the labels are still "oranges", "bread", "bags of chips", "milk", "tomato sauce".
This time, though, the values are 7, 2, 3, 1, 6.

Each time you go to the store, the labels will remain the same, but the values attached to those labels varies. This are what developers use variables for. Words that human beings can read and understand (the label) which can be assigned a value.

## Your First Variables

Variables are labels for values that vary over time.

Time to see your first variables in JavaScript to represent the first trip to the store.
  
```js
let oranges = 4
let breadLoaves = 1
let bagsOfChips = 2
let milk = 1
let tomatoSauce = 3
```

You use the keyword of `let` to "declare a variable". In other words, it tells JavaScript that the word immediately to the right is going to be a variable. Then you type an equal sign, and then finally what value you want to be assigned to the variable.

You can make the variable name ANYTHING YOU WANT. You are the software developer, so you have that power. One thing that confuses many beginners is that they think the variable name matters. It doesn't. JavaScript doesn't care - at all - what your variables are. All it cares about is the values.

However, other developers do care what you name your variables. Imagine how frustrated you would be if instead of using the descriptive names above for the variables, you saw this code instead.

```js
let o = 4 
let bl = 1 
let boc = 2 
let m = 1 
let ts = 3
```

The developer who wrote this code knew that "o" was an abbreviation for "oranges", but you would have no idea that it was. How annoying!

## Camel Case

Speaking of naming variables, it is a convention in the JavaScript developer community to name variables with camel case. This means that the variable starts with a lower-case letter, but each additional word in the variable name should start with a capital letter.

Bad variable naming
```js
let bagofdonuts = 2
```
Good variable naming
```js
let bagOfDonuts = 2
```
Good variable naming because it is a single word
```js
let cucumbers = 3
```
Bad variable naming
```js
let icecream = 1
```
Good variable naming
```js
let iceCream = 1
```

## Writing Your First Code

Regardless of what you name your variable, JavaScript doesn't care at all. All it cares about is the 4, 1, 2, 1, and 3.

You can prove it.

Over to the left, you will see two areas. 

1. The one at the top has a white background. This is going to be your code editor in repl.it. That is where you will type in your code. 
2. The one at the bottom has a black background. That's called the console. It is where the results, or output, of your code will be displayed.

Type `let oranges = 4` into the code editor, and then press your return key. Then type `console.log(oranges)` and press return. Translated to English, that is an instruction you give JavaScript to display the value of a variable in the console.

Click the "run >" button at the top of the code editor, and you will see the number 4 displayed displayed in the console at the bottom. It will be followed by the message of `=> undefined`, but that doesn't mean you made a mistake. You will see that message all the time in the console, and you can ignore it.

See? You - as the human - think of it as oranges, but JavaScript sees it as a 4.

![](https://storage.googleapis.com/replit/images/1580996423301_c401392b5aeee359cd2b9548ffb1c3b9.gif)

## Changing a Variable's Value

Remember that the main purpose of a variable declared with `let` is that the value varies. You can change the value assigned to all of the variables to reflect your second trip to the store.

```js
oranges = 7
breadLoaves = 2
bagsOfChips = 3
milk = 1
tomatoSauce = 6
```

In case you didn't notice the difference, there is no `let` keyword at the beginning of those lines of code. You are not declaring the variables any more. You already did that. This time you are changing the value of the variables. Once you write those lines of code and use the `console.log(oranges)` again, the output will be different.

Give it a shot. Change the value of the oranges variable to 10 in the code editor and log its value to the console again.

![](https://storage.googleapis.com/replit/images/1580996868099_043937a0e3661420480ff0f5fec43ad8.gif)

## Adding the Values in Variables

In this introduction, the values for each of your variables are numbers. In this case, they are integers. The variables are placeholders, or labels, for those values. What this allows you to do is perform mathematical operations on the numbers by using the variables.

Look at the values for your first shopping trip again.

```js
let oranges = 4
let breadLoaves = 1
let bagsOfChips = 2
let milk = 1
let tomatoSauce = 3
```

Now assume you want to know the total quantity of items that you bought at the store on that day. You can use the plus sign to add then all up.

```js
const total = oranges + breadLoaves + bagsOfChips + milk + tomatoSauce
```

It looks weird to be adding words, but you need to remember that you're not adding the variables. You are adding the values that those variables represent. JavaScript interprets that code as the following.

```js
const total = 4 + 1 + 2 + 1 + 3
```

Um, wait a second. What is that new keyword of `const`?

It's short for "constant value". This means that you can't change the value of the variable you are declaring. If you try to, JavaScript will be angry with you. You can try this out for yourself. In the  code editor, enter in the following two lines of code there, and click the "run >" button.

```js
const bananas = 4
bananas = 10
```

You will immediately see an angry, red message in the console below it with the message 
**SyntaxError: Assignment to constant variable: bananas**


![](https://storage.googleapis.com/replit/images/1580994909495_e370359bb817efb31f63f876698416be.gif)

* The `let` keyword for declaring variables will allow you to change the value.
* The `const` keyword for declaring variables will not allow you to change the value.

Why would you choose `const` instead of `let` for the `totalQuantity` variable? Well, that's a value that you don't want to be mistakenly change later in the code. Humans make mistakes all the time, and you don't want other code that you write to modify that total value.

## Output the Total

Now go to the code editor again and add all of the variables for your shopping trip.

```js
let oranges = 4
let breadLoaves = 1
let bagsOfChips = 2
let milk = 1
let tomatoSauce = 3
```

Then add them all together, and output the value of `total`.

```js
const total = oranges + breadLoaves + bagsOfChips + milk + tomatoSauce
console.log(total)
```

You should see the number `11` display in the console.

![](https://storage.googleapis.com/replit/images/1580998425819_63cbc1871e211fbb3ea4de02e84c75eb.gif)

## Your First Exercise

Now it is time for you to write your own code. Imagine that you want to determine what your  electric bill costs are for an entire year. You gather all twelve electric bills in front of you and want to add them together. Instead of just entering in the numbers, you are going to assign those numbers as values to variables. Each variable will represent a single month's electric bill charge.

Here's how you can start.

1. Delete any code that you already have in the code editor.
2. Place the following code in the editor.

```js
let januaryBill = 43.11
```

Your job is to write eleven more variables to represent the charges for February, March, April, May, June, July, August, September, October, November, and December. You are just going to make up each month's charge for this exercise. You can even imagine that in June, you had friends over for a few days to play video games, or watch movies, and the charge for that month was ridiculously high, say, 203.55.

After you have made all of your variables, declare one more at the end to store the total yearly charges. Remember that you can name the variable whatever you want.

Use the `const` keyword to declare this variable instead of `let`.

* total
* yearlyTotal
* totalCharges

JavaScript doesn't care what the name of the variable is. Humans do. Make sure your variable names are descriptive enough for another person to understand what value it represents.

After you have added all of the numbers, use `console.log()` to output the value of your total variable to the console.

Then move your mouse up the the "run >" button, but click the down arrow instead and choose the option of "run tests >". If your code correctly outputs a number, your will see a green message of "Outputs total yearly charges".

However, if you have a syntax error somewhere, or forgot to use `console.log()` at the end of your code, you will see a red, error message. If you see this, go back to your code and make sure you have the correct syntax for declaring all of your variables, that you spelled each variable the same when you are adding them, and that you have a `console.log()` at the end of your code.

If you were successful, click the green "Submit" button at the top right of the screen.

Once it is submitted, click the "< back to classroom" link in the top left of the screen and work on the next exercise.
<!--stackedit_data:
eyJoaXN0b3J5IjpbMjgzMDcyMjBdfQ==
-->