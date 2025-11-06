# Strings Parsing (C++)

## Challenge Description
The goal is to implement a function that takes a string of comma-separated integers (e.g., "23,4,96") and returns a vector of integers.

## 💡 Approach
The solution uses the C++ Standard Template Library's **`stringstream`** class for robust formatted parsing. **This approach achieves a linear time complexity of O(N), where N is the length of the string, as each character is processed once.**

* **Process:** A `while` loop extracts the integer (`ss >> temp`) followed by the comma delimiter (`ss >> ch`) sequentially.
* **Robustness:** This method handles the end-of-string gracefully. When the last integer is read, the subsequent failed attempt to read the comma automatically sets the stream's failbit, causing the next loop condition check to terminate the process cleanly.