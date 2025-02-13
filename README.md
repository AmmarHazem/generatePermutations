# Permutations in JavaScript

This repository contains JavaScript functions for generating all permutations of an array and finding the next permutation in lexicographical order.

## Functions

### `permute(arr)`
Generates all possible permutations of an array.

#### **Usage:**
```js
const permutations = permute([1, 2, 3]);
console.log(permutations);
```

#### **Output:**
```js
[
  [1, 2, 3],
  [1, 3, 2],
  [2, 1, 3],
  [2, 3, 1],
  [3, 1, 2],
  [3, 2, 1]
]
```

---

### `nextPermutation(nums)`
Finds the next lexicographical permutation of an array.

#### **Usage:**
```js
const nextPerm = nextPermutation([1, 2, 3]);
console.log(nextPerm);
```

#### **Output:**
```js
[1, 3, 2]
```

---

### `generatePermutations(arr)`
A helper function that recursively generates all permutations of an array.

#### **Usage:**
```js
const myArray = [1, 2, 3, 4, 5];
const allPermutations = generatePermutations(myArray);
console.log(allPermutations);
```

#### **Output:**
Generates all possible permutations of `[1, 2, 3, 4, 5]` and prints them.

---

## How It Works
1. The `permute` function uses a recursive approach with backtracking to generate all possible permutations of an input array.
2. The `generatePermutations` function follows a similar recursive approach but works with filtering.
3. The `nextPermutation` function finds the next lexicographical permutation by:
   - Generating all permutations of the given array.
   - Finding the index of the current permutation.
   - Returning the next permutation in the sorted order.

## Running the Code
To execute the script, simply run:
```sh
node script.js
```