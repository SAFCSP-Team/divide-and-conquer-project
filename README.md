# Divide and Conquer Project


### Objective

In this project, our objective is to understand how to use divide and conquer approach.

### Problem
Create `binarysearch` method that returns an integer representing the index of the target element in the array.

### Implementation
* initialize variables `low` to starting index and `high` to the last index of the array.
* continue searching while low is less than or equal to high.
* determine the middle index mid of the current search range.
* if the middle element matches the target, return its index.
* if the target is larger than the middle element, focus on the right half of the array.
* if the target is smaller than the middle element, focus on the left half of the array.
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
