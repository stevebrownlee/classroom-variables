# Multi-line Strings

So far you have used `console.log()` to produce strings of output in the console. Sometimes, developers want their output to be more attractive, especially if the output requires a multi-line format to be more readable.


Just a quick example to show you what happens when you tell JavaScript to output a multi-line string. Place the following code in the code editor and click the "run >" button. You will see a red error message in the console.

```js
console.log("
Line 1
Line 2
")
```

  
![](https://storage.googleapis.com/replit/images/1581101869412_66df4d6f2b43157ab55690d1fef4d3ac.gif)

## Backticks for Prettier Output

In the last two chapters, you used the backtick (`) character to do string interpolation - where you can inject one string into another one. The other benefit of the backtick character is to produce multi-line strings.

In your code, replace the double quote characters with backticks and run it again. JavaScript will no longer yell at you.
  
![](https://storage.googleapis.com/replit/images/1581101883981_b9f1bd1d23efc42b314101c2a8ea9d9a.gif)

## Exercise: Formatted Income Statement

You are going to practice adding and subtracting variables again, but this time, the ouput will be more readable.

* You have a monthly income of $5478.84
* Your wife has a monthly income of $4028.37
* Your monthly mobile phone bill is $254.91
* Your monthly mortgage is $2161.12
* Your monthly car insurance bill is $205.31
* Your monthly health insurance bill is $508.18

Here's what you need to output to the console. Replace the `xxx` text with the correct amount. Use addition and subtraction to come up with the right values. Use backticks to make the output readable in the following format.

```html
Our combined monthly income is xxx.
Our total monthly expenses are xxx.
Our net monthly income is xxx.
```



9507.21
3129.5199999999995
6377.689999999999
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE3NDk0OTYwMTAsLTU2ODkwNTI3Ml19
-->