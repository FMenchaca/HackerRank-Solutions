# Simple Array Sum (Python)

## Challenge Description
Given an array of integers, find the sum of its elements.

## 💡  Approach
The solution implements a optimal approach to aggregation.

* **Time Complexity:** The method achieves a **linear time complexity of O(N)**, where N is the number of elements in the array. This is the fastest possible time complexity, as every element must be visited once.
* **Method:** The core logic uses a standard `for` loop to iterate through the array elements, adding them to a running `sum` total. This is the most direct and efficient method for array summation.
* **Alternative (Pythonic):** Although the `for` loop is explicit, the built-in `sum(ar)` function in Python could achieve the same O(N) complexity in a single, cleaner line.