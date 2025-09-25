
# Sorting Algorithms in C++

**Aim:**
To study and implement different **Sorting Algorithms** in C++:
i) Selection Sort
ii) Insertion Sort
iii) Bubble Sort

**Tools Used:**

* VS Code or any online C++ Compiler

---

## Theory

A **Sorting Algorithm** is a method used to rearrange elements of an array or list into a particular order (ascending or descending). Sorting is one of the most important operations in computer science because it helps in efficient **searching**, **data organization**, and **optimization** of other algorithms.

Sorting algorithms are broadly classified as:

* **Comparison-based sorting** (e.g., Bubble Sort, Selection Sort, Insertion Sort, Merge Sort, Quick Sort).
* **Non-comparison sorting** (e.g., Counting Sort, Radix Sort, Bucket Sort).

In this experiment, we focus on **three simple, comparison-based sorting techniques**:

---

### 1. Selection Sort

* Selection sort works by **repeatedly finding the minimum element** from the unsorted part of the array and placing it in its correct position.
* The array is conceptually divided into **two subarrays**: a sorted part (on the left) and an unsorted part (on the right).
* In each iteration, the smallest element of the unsorted subarray is placed at the end of the sorted subarray.

**Time Complexity:**

* Best Case: O(n²)
* Average Case: O(n²)
* Worst Case: O(n²)

<img width="480" height="800" alt="image" src="https://github.com/user-attachments/assets/12288da4-86fb-4873-81fb-f1be02bc915f" />


---

### 2. Insertion Sort

* Insertion sort works like the way we arrange playing cards in our hands.
* Starting from the second element, it is compared with the elements before it and placed in its correct position in the sorted portion of the array.
* This process is repeated until the entire array is sorted.

**Time Complexity:**

* Best Case: O(n) (already sorted array)
* Average Case: O(n²)
* Worst Case: O(n²)

 <img width="392" height="503" alt="image" src="https://github.com/user-attachments/assets/38de6c3d-5573-4190-85c3-c6896c92c661" />
---

### 3. Bubble Sort

* Bubble sort works by **repeatedly swapping adjacent elements** if they are in the wrong order.
* With each pass, the largest element "bubbles up" to its correct position at the end of the array.
* This process continues until no more swaps are needed, meaning the array is sorted.

**Time Complexity:**

* Best Case: O(n) (when array is already sorted)
* Average Case: O(n²)
* Worst Case: O(n²)



  <img width="801" height="401" alt="image" src="https://github.com/user-attachments/assets/c0f5490b-e452-420b-a73d-621571bd5ecf" />


---

### General Syntax of Swap Function (used in sorting):

```cpp
void swap(int *a, int *b) {
    int temp = *a;
    *a = *b;
    *b = temp;
}
```

---

## Program 1 – Selection Sort

**Algorithm (Detailed):**

1. Start the program.
2. Read the number of elements `n` and input array elements.
3. For each index `i` from `0` to `n-2`:

   * Find the minimum element from the unsorted part (`i` to `n-1`).
   * Swap it with the element at index `i`.
4. Repeat until the array is sorted.
5. Display the sorted array.
6. End the program.

**Key Point:** Works by placing the smallest element at its correct position step by step.

---

## Program 2 – Insertion Sort

**Algorithm (Detailed):**

1. Start the program.
2. Read the number of elements `n` and input array elements.
3. For each element from index `1` to `n-1`:

   * Store the element in a temporary variable `key`.
   * Compare it with elements before it (`arr[j]`).
   * Shift elements greater than `key` one position to the right.
   * Insert `key` in its correct position.
4. Repeat until all elements are sorted.
5. Display the sorted array.
6. End the program.

**Key Point:** Elements are inserted one by one into their correct position, like sorting cards in hand.

---

## Program 3 – Bubble Sort

**Algorithm (Detailed):**

1. Start the program.
2. Read the number of elements `n` and input array elements.
3. For each pass `i` from `0` to `n-1`:

   * Compare adjacent elements `arr[j]` and `arr[j+1]`.
   * If `arr[j] > arr[j+1]`, swap them.
   * After each pass, the largest element moves to its correct position.
4. Repeat until no swaps are required or all passes are completed.
5. Display the sorted array.
6. End the program.

**Key Point:** Repeatedly compares and swaps adjacent elements until sorted.

---

## Key Learning Outcomes

* Understood three basic **sorting algorithms**: Selection, Insertion, and Bubble Sort.
* Learned how sorting reduces complexity of searching and improves efficiency.
* Observed how different algorithms have different time complexities.
* Learned to implement **swap operations** and looping structures for sorting.

---

## Applications

* **Databases:** Sorting records for quick access.
* **E-commerce:** Sorting products by price, popularity, or rating.
* **Operating Systems:** Sorting tasks for scheduling.
* **Gaming:** Sorting scores, leaderboards, or inventories.
* **Computer Graphics:** Sorting data for rendering objects in order.

---

## Conclusion

Thus, we have studied and implemented **Selection Sort, Insertion Sort, and Bubble Sort** in C++. These algorithms demonstrate how sorting works step by step, highlight their efficiency, and show the importance of choosing the right algorithm for a given application.


