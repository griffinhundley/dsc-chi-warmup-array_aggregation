*Import tests*


```python
from tests import MultiplyTest, ArrayTest
```

# For today's warmup, please solve the following code problems:

## Exercise #1

The function below doesn't work. Figure out why and fix the code.


```python
def multiply(a, b):
    return a * b
```

*Run the cell below to see if your code is successful!*


```python
evaluate = MultiplyTest()
evaluate.run(multiply)
```


## Passed!
 >*3 tests passed*

--------------- 
 
 <details><summary>Test Results</summary>

✅ Test 1 passed!

✅ Test 2 passed!

✅ Test 3 passed!
</details>

Once you have passed the above tests, run the cell below to test your code on 100 randomly generated tests


```python
evaluate.run(multiply, random=True)
```


## Passed!
 >*3 tests passed*

--------------- 
 
 <details><summary>Test Results</summary>

✅ Test 1 passed!

✅ Test 2 passed!

✅ Test 3 passed!</details>
### Randomly Generated Tests –– Passed
 >*100 tests passed.*

--------------- 

<details><summary>Random Tests Results</summary>

✅ Random Test 0 passed!

✅ Random Test 1 passed!

✅ Random Test 2 passed!

✅ Random Test 3 passed!

✅ Random Test 4 passed!

✅ Random Test 5 passed!

✅ Random Test 6 passed!

✅ Random Test 7 passed!

✅ Random Test 8 passed!

✅ Random Test 9 passed!

✅ Random Test 10 passed!

✅ Random Test 11 passed!

✅ Random Test 12 passed!

✅ Random Test 13 passed!

✅ Random Test 14 passed!

✅ Random Test 15 passed!

✅ Random Test 16 passed!

✅ Random Test 17 passed!

✅ Random Test 18 passed!

✅ Random Test 19 passed!

✅ Random Test 20 passed!

✅ Random Test 21 passed!

✅ Random Test 22 passed!

✅ Random Test 23 passed!

✅ Random Test 24 passed!

✅ Random Test 25 passed!

✅ Random Test 26 passed!

✅ Random Test 27 passed!

✅ Random Test 28 passed!

✅ Random Test 29 passed!

✅ Random Test 30 passed!

✅ Random Test 31 passed!

✅ Random Test 32 passed!

✅ Random Test 33 passed!

✅ Random Test 34 passed!

✅ Random Test 35 passed!

✅ Random Test 36 passed!

✅ Random Test 37 passed!

✅ Random Test 38 passed!

✅ Random Test 39 passed!

✅ Random Test 40 passed!

✅ Random Test 41 passed!

✅ Random Test 42 passed!

✅ Random Test 43 passed!

✅ Random Test 44 passed!

✅ Random Test 45 passed!

✅ Random Test 46 passed!

✅ Random Test 47 passed!

✅ Random Test 48 passed!

✅ Random Test 49 passed!

✅ Random Test 50 passed!

✅ Random Test 51 passed!

✅ Random Test 52 passed!

✅ Random Test 53 passed!

✅ Random Test 54 passed!

✅ Random Test 55 passed!

✅ Random Test 56 passed!

✅ Random Test 57 passed!

✅ Random Test 58 passed!

✅ Random Test 59 passed!

✅ Random Test 60 passed!

✅ Random Test 61 passed!

✅ Random Test 62 passed!

✅ Random Test 63 passed!

✅ Random Test 64 passed!

✅ Random Test 65 passed!

✅ Random Test 66 passed!

✅ Random Test 67 passed!

✅ Random Test 68 passed!

✅ Random Test 69 passed!

✅ Random Test 70 passed!

✅ Random Test 71 passed!

✅ Random Test 72 passed!

✅ Random Test 73 passed!

✅ Random Test 74 passed!

✅ Random Test 75 passed!

✅ Random Test 76 passed!

✅ Random Test 77 passed!

✅ Random Test 78 passed!

✅ Random Test 79 passed!

✅ Random Test 80 passed!

✅ Random Test 81 passed!

✅ Random Test 82 passed!

✅ Random Test 83 passed!

✅ Random Test 84 passed!

✅ Random Test 85 passed!

✅ Random Test 86 passed!

✅ Random Test 87 passed!

✅ Random Test 88 passed!

✅ Random Test 89 passed!

✅ Random Test 90 passed!

✅ Random Test 91 passed!

✅ Random Test 92 passed!

✅ Random Test 93 passed!

✅ Random Test 94 passed!

✅ Random Test 95 passed!

✅ Random Test 96 passed!

✅ Random Test 97 passed!

✅ Random Test 98 passed!

✅ Random Test 99 passed!
</details>

**Extra Credit:** Instead of summing individual numbers, see if you can edit your ```multiply``` function so that it is [broadcasting](https://docs.scipy.org/doc/numpy/user/basics.broadcasting.html) two arrays.

This version of your function should receive two inputs:
1. An array containing three numbers
2. An array containing three numbers

The output of the array should contain three numbers

```
[1,2,3] * [4,5,6] ---> [4,10,18]```


```python
import numpy as np

def multiply(arr1, arr2):
    np_array1 = np.asarray(arr1)
    np_array2 = np.asarray(arr2)
    return np_array1 * np_array2
```


```python
evaluate.run(multiply, random=True, broadcast=True)
```


## Passed!
 >*3 tests passed*

--------------- 
 
 <details><summary>Test Results</summary>

✅ Test 1 passed!

✅ Test 2 passed!

✅ Test 3 passed!</details>
### Randomly Generated Tests –– Passed
 >*100 tests passed.*

--------------- 

<details><summary>Random Tests Results</summary>

✅ Random Test 0 passed!

✅ Random Test 1 passed!

✅ Random Test 2 passed!

✅ Random Test 3 passed!

✅ Random Test 4 passed!

✅ Random Test 5 passed!

✅ Random Test 6 passed!

✅ Random Test 7 passed!

✅ Random Test 8 passed!

✅ Random Test 9 passed!

✅ Random Test 10 passed!

✅ Random Test 11 passed!

✅ Random Test 12 passed!

✅ Random Test 13 passed!

✅ Random Test 14 passed!

✅ Random Test 15 passed!

✅ Random Test 16 passed!

✅ Random Test 17 passed!

✅ Random Test 18 passed!

✅ Random Test 19 passed!

✅ Random Test 20 passed!

✅ Random Test 21 passed!

✅ Random Test 22 passed!

✅ Random Test 23 passed!

✅ Random Test 24 passed!

✅ Random Test 25 passed!

✅ Random Test 26 passed!

✅ Random Test 27 passed!

✅ Random Test 28 passed!

✅ Random Test 29 passed!

✅ Random Test 30 passed!

✅ Random Test 31 passed!

✅ Random Test 32 passed!

✅ Random Test 33 passed!

✅ Random Test 34 passed!

✅ Random Test 35 passed!

✅ Random Test 36 passed!

✅ Random Test 37 passed!

✅ Random Test 38 passed!

✅ Random Test 39 passed!

✅ Random Test 40 passed!

✅ Random Test 41 passed!

✅ Random Test 42 passed!

✅ Random Test 43 passed!

✅ Random Test 44 passed!

✅ Random Test 45 passed!

✅ Random Test 46 passed!

✅ Random Test 47 passed!

✅ Random Test 48 passed!

✅ Random Test 49 passed!

✅ Random Test 50 passed!

✅ Random Test 51 passed!

✅ Random Test 52 passed!

✅ Random Test 53 passed!

✅ Random Test 54 passed!

✅ Random Test 55 passed!

✅ Random Test 56 passed!

✅ Random Test 57 passed!

✅ Random Test 58 passed!

✅ Random Test 59 passed!

✅ Random Test 60 passed!

✅ Random Test 61 passed!

✅ Random Test 62 passed!

✅ Random Test 63 passed!

✅ Random Test 64 passed!

✅ Random Test 65 passed!

✅ Random Test 66 passed!

✅ Random Test 67 passed!

✅ Random Test 68 passed!

✅ Random Test 69 passed!

✅ Random Test 70 passed!

✅ Random Test 71 passed!

✅ Random Test 72 passed!

✅ Random Test 73 passed!

✅ Random Test 74 passed!

✅ Random Test 75 passed!

✅ Random Test 76 passed!

✅ Random Test 77 passed!

✅ Random Test 78 passed!

✅ Random Test 79 passed!

✅ Random Test 80 passed!

✅ Random Test 81 passed!

✅ Random Test 82 passed!

✅ Random Test 83 passed!

✅ Random Test 84 passed!

✅ Random Test 85 passed!

✅ Random Test 86 passed!

✅ Random Test 87 passed!

✅ Random Test 88 passed!

✅ Random Test 89 passed!

✅ Random Test 90 passed!

✅ Random Test 91 passed!

✅ Random Test 92 passed!

✅ Random Test 93 passed!

✅ Random Test 94 passed!

✅ Random Test 95 passed!

✅ Random Test 96 passed!

✅ Random Test 97 passed!

✅ Random Test 98 passed!

✅ Random Test 99 passed!
    </details>

# Exercise #2

Please fill in the code for the ```array_plus_array``` function below.

The function should have two inputs:
1. An array containing at least three numbers
2. An array containing at least three numbers

The function should return a single digit that sums all digits within both arrays


```python
def array_plus_array(arr1, arr2):
    return sum(arr1) + sum(arr2)
```

*Run the following cell to test your function!*


```python
evaluate = ArrayTest()
evaluate.run(array_plus_array)
```


## Passed!
 >*7 tests passed*

--------------- 
 
 <details><summary>Test Results</summary>

✅ Test 1 passed!

✅ Test 2 passed!

✅ Test 3 passed!

✅ Test 4 passed!

✅ Test 5 passed!

✅ Test 6 passed!

✅ Test 7 passed!

    </details>
Once you have managed to pass all of the tests, run the cell above to see if you function can pass 100 randomly generated tests!


```python
evaluate.run(array_plus_array, random=True)
```


## Passed!
 >*7 tests passed*

--------------- 
 
 <details><summary>Test Results</summary>

✅ Test 1 passed!

✅ Test 2 passed!

✅ Test 3 passed!

✅ Test 4 passed!

✅ Test 5 passed!

✅ Test 6 passed!

✅ Test 7 passed!</details>
### Randomly Generated Tests –– Passed
 >*100 tests passed.*

--------------- 

<details><summary>Random Tests Results</summary>

✅ Random Test 1 passed!

✅ Random Test 2 passed!

✅ Random Test 3 passed!

✅ Random Test 4 passed!

✅ Random Test 5 passed!

✅ Random Test 6 passed!

✅ Random Test 7 passed!

✅ Random Test 8 passed!

✅ Random Test 9 passed!

✅ Random Test 10 passed!

✅ Random Test 11 passed!

✅ Random Test 12 passed!

✅ Random Test 13 passed!

✅ Random Test 14 passed!

✅ Random Test 15 passed!

✅ Random Test 16 passed!

✅ Random Test 17 passed!

✅ Random Test 18 passed!

✅ Random Test 19 passed!

✅ Random Test 20 passed!

✅ Random Test 21 passed!

✅ Random Test 22 passed!

✅ Random Test 23 passed!

✅ Random Test 24 passed!

✅ Random Test 25 passed!

✅ Random Test 26 passed!

✅ Random Test 27 passed!

✅ Random Test 28 passed!

✅ Random Test 29 passed!

✅ Random Test 30 passed!

✅ Random Test 31 passed!

✅ Random Test 32 passed!

✅ Random Test 33 passed!

✅ Random Test 34 passed!

✅ Random Test 35 passed!

✅ Random Test 36 passed!

✅ Random Test 37 passed!

✅ Random Test 38 passed!

✅ Random Test 39 passed!

✅ Random Test 40 passed!

✅ Random Test 41 passed!

✅ Random Test 42 passed!

✅ Random Test 43 passed!

✅ Random Test 44 passed!

✅ Random Test 45 passed!

✅ Random Test 46 passed!

✅ Random Test 47 passed!

✅ Random Test 48 passed!

✅ Random Test 49 passed!

✅ Random Test 50 passed!

✅ Random Test 51 passed!

✅ Random Test 52 passed!

✅ Random Test 53 passed!

✅ Random Test 54 passed!

✅ Random Test 55 passed!

✅ Random Test 56 passed!

✅ Random Test 57 passed!

✅ Random Test 58 passed!

✅ Random Test 59 passed!

✅ Random Test 60 passed!

✅ Random Test 61 passed!

✅ Random Test 62 passed!

✅ Random Test 63 passed!

✅ Random Test 64 passed!

✅ Random Test 65 passed!

✅ Random Test 66 passed!

✅ Random Test 67 passed!

✅ Random Test 68 passed!

✅ Random Test 69 passed!

✅ Random Test 70 passed!

✅ Random Test 71 passed!

✅ Random Test 72 passed!

✅ Random Test 73 passed!

✅ Random Test 74 passed!

✅ Random Test 75 passed!

✅ Random Test 76 passed!

✅ Random Test 77 passed!

✅ Random Test 78 passed!

✅ Random Test 79 passed!

✅ Random Test 80 passed!

✅ Random Test 81 passed!

✅ Random Test 82 passed!

✅ Random Test 83 passed!

✅ Random Test 84 passed!

✅ Random Test 85 passed!

✅ Random Test 86 passed!

✅ Random Test 87 passed!

✅ Random Test 88 passed!

✅ Random Test 89 passed!

✅ Random Test 90 passed!

✅ Random Test 91 passed!

✅ Random Test 92 passed!

✅ Random Test 93 passed!

✅ Random Test 94 passed!

✅ Random Test 95 passed!

✅ Random Test 96 passed!

✅ Random Test 97 passed!

✅ Random Test 98 passed!

✅ Random Test 99 passed!

✅ Random Test 100 passed!

    </details>
**Extra Credit:** Instead of summing all numbers in your array, see if you can edit the ```array_plus_array``` function so that it is broadcasting two arrays.

```
[1,2,3] + [4,5,6] ----> [5,7,9]```


```python
import numpy as np

def array_plus_array(arr1, arr2):
    np_array1 = np.asarray(arr1)
    np_array2 = np.asarray(arr2)
    return np_array1 + np_array2
```

Test your code by running the cell below


```python
evaluate = ArrayTest()
evaluate.run(array_plus_array, random=True, broadcast=True)
```


## Passed!
 >*7 tests passed*

--------------- 
 
 <details><summary>Test Results</summary>

✅ Test 1 passed!

✅ Test 2 passed!

✅ Test 3 passed!

✅ Test 4 passed!

✅ Test 5 passed!

✅ Test 6 passed!

✅ Test 7 passed!</details>
### Randomly Generated Tests –– Passed
 >*100 tests passed.*

--------------- 

<details><summary>Random Tests Results</summary>

✅ Random Test 1 passed!

✅ Random Test 2 passed!

✅ Random Test 3 passed!

✅ Random Test 4 passed!

✅ Random Test 5 passed!

✅ Random Test 6 passed!

✅ Random Test 7 passed!

✅ Random Test 8 passed!

✅ Random Test 9 passed!

✅ Random Test 10 passed!

✅ Random Test 11 passed!

✅ Random Test 12 passed!

✅ Random Test 13 passed!

✅ Random Test 14 passed!

✅ Random Test 15 passed!

✅ Random Test 16 passed!

✅ Random Test 17 passed!

✅ Random Test 18 passed!

✅ Random Test 19 passed!

✅ Random Test 20 passed!

✅ Random Test 21 passed!

✅ Random Test 22 passed!

✅ Random Test 23 passed!

✅ Random Test 24 passed!

✅ Random Test 25 passed!

✅ Random Test 26 passed!

✅ Random Test 27 passed!

✅ Random Test 28 passed!

✅ Random Test 29 passed!

✅ Random Test 30 passed!

✅ Random Test 31 passed!

✅ Random Test 32 passed!

✅ Random Test 33 passed!

✅ Random Test 34 passed!

✅ Random Test 35 passed!

✅ Random Test 36 passed!

✅ Random Test 37 passed!

✅ Random Test 38 passed!

✅ Random Test 39 passed!

✅ Random Test 40 passed!

✅ Random Test 41 passed!

✅ Random Test 42 passed!

✅ Random Test 43 passed!

✅ Random Test 44 passed!

✅ Random Test 45 passed!

✅ Random Test 46 passed!

✅ Random Test 47 passed!

✅ Random Test 48 passed!

✅ Random Test 49 passed!

✅ Random Test 50 passed!

✅ Random Test 51 passed!

✅ Random Test 52 passed!

✅ Random Test 53 passed!

✅ Random Test 54 passed!

✅ Random Test 55 passed!

✅ Random Test 56 passed!

✅ Random Test 57 passed!

✅ Random Test 58 passed!

✅ Random Test 59 passed!

✅ Random Test 60 passed!

✅ Random Test 61 passed!

✅ Random Test 62 passed!

✅ Random Test 63 passed!

✅ Random Test 64 passed!

✅ Random Test 65 passed!

✅ Random Test 66 passed!

✅ Random Test 67 passed!

✅ Random Test 68 passed!

✅ Random Test 69 passed!

✅ Random Test 70 passed!

✅ Random Test 71 passed!

✅ Random Test 72 passed!

✅ Random Test 73 passed!

✅ Random Test 74 passed!

✅ Random Test 75 passed!

✅ Random Test 76 passed!

✅ Random Test 77 passed!

✅ Random Test 78 passed!

✅ Random Test 79 passed!

✅ Random Test 80 passed!

✅ Random Test 81 passed!

✅ Random Test 82 passed!

✅ Random Test 83 passed!

✅ Random Test 84 passed!

✅ Random Test 85 passed!

✅ Random Test 86 passed!

✅ Random Test 87 passed!

✅ Random Test 88 passed!

✅ Random Test 89 passed!

✅ Random Test 90 passed!

✅ Random Test 91 passed!

✅ Random Test 92 passed!

✅ Random Test 93 passed!

✅ Random Test 94 passed!

✅ Random Test 95 passed!

✅ Random Test 96 passed!

✅ Random Test 97 passed!

✅ Random Test 98 passed!

✅ Random Test 99 passed!

✅ Random Test 100 passed!
    </details>
