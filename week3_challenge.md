# Problem - The Snail
![Snail](https://media.giphy.com/media/n17GyE4DbZfbO/giphy.gif)
Given an n x n array, write a method that returns the array elements arranged from outermost elements to the middle element, traveling clockwise.

A good way to visualize this is to picture the spiral shell of a snail! 

## JS Example
```js
const arrayMatrix = [
  [1, 2, 3],
  [4, 5, 6],
  [7, 8, 9]
];

snail(arrayMatrix) #=> [1, 2, 3, 6, 9, 8, 7, 4, 5]
```

## Ruby Example
```rb
arrayMatrix = [
  [1, 2, 3],
  [4, 5, 6],
  [7, 8, 9]
];

snail(arrayMatrix) #=> [1, 2, 3, 6, 9, 8, 7, 4, 5]
```

# Instructions

1. Copy this markdown and paste in your own, private gist
2. In your private gist, fill out the questions below
4. Submit by the due time as instructed in Zoom

Do not publish your code on a public repl.it or repo or other public means.

## Rewrite the question in your own words:


## What assumptions will you make about this problem if you cannot ask any more clarifying questions? What are your reasons for making those assumptions?

# What information has been provided, and what information am I lacking?  Can make assumptions on these unknowns and what would the reasoning be?


## What are your initial thoughts about this problem? (high level design, 2-3 sentences)

# An array of arrays can be sent to a method/function to have it's perimeter numbers returned as seen spiraling inward in an array.
# This will take me some time to figure out.

## How would you identify the elements of this problem?

- [ ] Searching of Data
- [x] Sorting of Data
- [x] Pattern Recognition
- [x] Build/Navigate a Grid
- [x] Math
- [ ] Language API knowledge
- [ ] Optimization


## Which data structure(s) do you think you'll use? What pros/cons do you see with that choice?

# I think only arrays will be needed.  Pros would be that both the input and expected output are arrays.  I don't see any cons.

## Write out a few lines of initial pseudocode: (mid-level design, NOT REAL CODE)

# Send array to method for sorting `snail(arrayMatrix)` 
# Count rows of arrays (number of arrays nested in array)
# Through logic begin taking the integers of of the arrays and put into a new array as the problem describes.
# The first "row" can be mapped directly to the array, this first row will no longer be looked at.
# Each of the "middle rows" will initially have their last integer stored in this new array.
# The last row will have its contents put into this new array in reverse. This first row will no longer be looked at.
# Going back up, we'll take the first integer of the middle rows.
# On the new top row, we'll take each integer except for the last one, which was already retrieved above.
# Repeat these steps until the center is reached.

## Write out any implementation code OR link to repl

## What is the Big O complexity of your solution?
