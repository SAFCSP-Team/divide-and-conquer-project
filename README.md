# Divide and Conquer Project


### Objective

In this project, our objective is to understand how to use divide and conquer algorithm

### Problem
Create `binarysearch` method that returns an integer representing the index of the target element in the array.

### Implementation

* initialize two integer variables `low` and `high`. Set low to 0, which represents the starting index of the array, and set high to `arr.length - 1`, which represents the ending index of the array.
* use a while loop to continue the search until low is less than or equal to high.
* within the loop, calculate the middle index `mid` by adding low to the difference between high and low, divided by 2.
* check if the element at the `mid` index of the array `arr[mid]` is equal to the target. If they are equal, return the `mid` index as the position of the target element in the array.
* if the target is greater than the element at the mid index, update low to mid + 1. This indicates that the target is located in the right half of the array.
* if the target is smaller than the element at the mid index, update high to mid - 1. This indicates that the target is located in the left half of the array.
* if the loop completes without finding the target element, return -1 to indicate that the element was not found in the array.

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
