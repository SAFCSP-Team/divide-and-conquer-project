# Divide and Conquer Project


### Objective

In this project, our objective is to understand how to use the divide and conquer approach.

### Problem
Create a `binarysearch` method that returns an integer representing the index of the target element in the array.

### Implementation
* Initialize variables `low` to the starting index and `high` to the last index of the array.
* Write the code that performs the *binary search algorithm* on the given array.
* Return the *index* of the target.
```java
public class BinarySearch {

      /* write your code here */

    public static void main(String[] args) {
        int[] arr = {2, 5, 8, 12, 16, 23, 38, 56, 72, 91};
        int target = 16;
        
        int index = binarysearch(arr, target);
        
        if (index != -1) {
            System.out.println("Element found at index " + index);
        } else {
            System.out.println("Element not found in the array");
        }
    }
}

  ```
