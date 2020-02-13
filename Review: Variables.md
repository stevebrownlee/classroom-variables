# Review of Variables

You are going to have to come up with your own variable names and values in this review. You will likely need to go back to previous exercises to review the concepts and look at the code that you have already written. That is highly encouraged, because that's what professional software developers do. No experienced developer will tell you that all of the information is memorized. They review their previous code all the time in order to apply it in new situations.

You will be using the following concepts in this exercise:

* Variables and their values
* Integer values
* String values
* Boolean values
* Mathematical operations
* Multi-line strings for output
* If/Else blocks for conditional logic
* `>=`, `<`, `>`, and `&&` operators

## Exercise: Family Photo Album

> We will provide some initial ideas for variable names. Feel free to change them to suit your own style. All that matters is their value.

You inherited a collection of family photos from your grandparents. They are currently stored in several envelopes of varying sizes. You decide that you have three options.

1. If there are more than 110 photos, then you decide that you need to purchase a large photo album and put them in it.
2. If there are less than 110, but 50 or more, you will purchase a shoe box and put all of the photos in it.
3. If there are less than 50, you will keep them in envelopes.

```js
let photoStorage = "Envelopes"
```

You are also going to categorize the photos into picture of the men in the family, and the women in the family. You want to keep track of those categories and the total.

```js
let totalPhotos = 0  // To start off with
const femalePhotos = 52
```

If there are more women than men in the photos, you will buy a plum photo album. If there are more men than women, you will buy a gray photo album.

```js
let albumColor = ""
```

When your logic is done, you need to check if it is correct.

* Change the number of photos of men and women to different amounts to verify that all three storage types are used in the right conditions.
* Have more male photos and check the logic
* Have more female photos and check the logic

### Expected Output

Our test will assume that there are 124 photos, and will have a majority of pictures of women.

```html
There are xxx total photos
There are xxx photos of women
There are xxx photos of men
Photos will be stored in a xxx colored xxx
```


<!--stackedit_data:
eyJoaXN0b3J5IjpbNTA5NjMxMzQ3XX0=
-->