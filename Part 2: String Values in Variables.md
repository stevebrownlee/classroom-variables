# String Values in Variables

In the previous exercise, you worked with variables that represented numeric values. In this chapter, you are going to work with different kinds of values: strings.  A string value is a series of numbers, letters, and symbols surrounded by either a single quote `'` or a double quote `"`.

You are going to be using double quotes around all of your strings, just so that you can be consistent.

## Your First String Variable

Imagine that you want to use JavaScript to keep track of all of the electronic items that you have in your house for insurance purposes. For the first example, you want to record what the manufacturer, brand, and size of your TV is. 

```js
const tv = "50-inch Sony A9G Master Series"
```

That string contains numbers, a symbol _(the dash)_, and letters. Trust me, you only want to type all of that once in your code. That's why you reference that string with a variable of `tv`. Start off simple again, and put that variable declaration into the code editor, then use `console.log()` to output the string value to the console.

Now, go over to the code editor and define a variable to store a string that describes your refrigerator. What do you think would be a good variable name for storing that information? If you don't know anything about your refrigerator, you can make something up like "Samsung Super Freeze Ultra Edition!" or anything you want.

Then `console.log()` the value of your variable and make sure that the string shows up in the console at the bottom.

## String Interpolation

Yeah, we know it's a weird word. What it means is that you can insert a string value into another string by using the variable name. Here's a quick example of what it looks like.

Remember the `const` keyword? It means that I cannot change the value of the variable after it has been declared.

```js
const gameConsole = "Sony Playstation"
const computer = "2017 Macbook Pro"

// Interpolation example
const gameSystems = `I play games on my ${gameConsole} and my ${computer}`
console.log(gameSystems)
```

This would produce the output of the following string.

```html
I play games on my Sony Playstation and my 2017 Macbook Pro
```

It's important to note that the string that was assigned as the value for the `gameSystems` variable does not have single quotes around it. If you look closely, you'll notice that the character is slightly tilted. It's called the backtick. It's the key right beneath your ESCAPE key on your keyboard.

## Practice: Major Electronics

Now you can practice making a couple more variables that reference strings which describe other electronics in your house. So far you have created a variable with a string value for your refrigerator. Make three more.

* Your computer
* Your mobile phone
* Your television

Once you declare those variables and provide a string value for each one, you should have four string variables in total.

Then use string interpolation to define a fifth variable named `allEletronics` which will have the value of the following format. Your job is to make sure that the `xxx` parts of the string below are replaced with your string values for each electronic device.

```html
"I have the following electronic devices. My xxx television, my xxx computer, my xxx refrigerator, and my xxx phone"
```

Then use `console.log()` to output the value of the `allElectronics` variable to the console. Then click the "run >" button. If you get a green success message, submit your exercises and go back to the classroom to work on the next one.

## Want to Know More?

To learn more about variables, you can review the [https://javascript.info/variables](https://javascript.info/variables) content. There's no place to write code, but you can always come back here and try some of the things you learn in the code editor.
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTAwOTgzOTI3MF19
-->