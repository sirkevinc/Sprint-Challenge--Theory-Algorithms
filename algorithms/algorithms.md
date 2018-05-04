# Algorithms Exercises

## Exercise I

Give an analysis of the running time with respect to the input size n of each of the following:

- a. `O(n)`
- b. `O(log n)`
- c. `O(sqrt(n))`
- d. `O(n^2)`
- e. `O(n^3)`
- f. `O(n)`
- g. `O(n)`

## Exercise II

- a. 
```js
const maximumValue = (array) => {
  let max = array[0];
  let min = array[0];

  for (let i = 0; i < array.length; i++) {
    let value = array[i];

    if (value < min) {
      min = value;
    }
    if (value > max) {
      max = value;
    }
  }
  return max - min;
}
```

- b. Starting at the middle level of the building, and continuing to move down by half the levels until an egg breaks will allow you to determine the value of `f` while minimizing the amount of eggs that are dropped.

