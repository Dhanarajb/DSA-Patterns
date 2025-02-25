## 🟢 Maximum Sum of Subarray of Size `k`

### ✅ Problem Statement
Given an array of integers and a number `k`, find the maximum sum of any contiguous subarray of size `k`.

---

## 🟡 Brute Force Approach

### 🔸 **Idea:**
- Check **all possible subarrays** of size `k`.
- Calculate their sums and keep track of the **maximum sum**.

### 📋 **Algorithm:**
1. Loop through the array from index `0` to `n - k`.
2. For each starting index, calculate the sum of the next `k` elements.
3. Update the maximum sum if the current sum is greater.

### 💻 **Code:**
```java
public class Main {
    public static int maxSumBruteForce(int[] arr, int k) {
        int maxSum = Integer.MIN_VALUE;

        for (int i = 0; i <= arr.length - k; i++) {
            int currentSum = 0;
            for (int j = i; j < i + k; j++) {
                currentSum += arr[j];
            }
            maxSum = Math.max(maxSum, currentSum);
        }

        return maxSum;
    }

    public static void main(String[] args) {
        int[] arr = {2, 1, 5, 1, 3, 2};
        int k = 3;
        System.out.println("Brute Force Max Sum: " + maxSumBruteForce(arr, k));
    }
}
```

### ⏰ **Time Complexity:** `O(n * k)`  
### 📦 **Space Complexity:** `O(1)`

---

## 🟢 Optimized Approach (Sliding Window)

### 🔸 **Idea:**
- Use a **sliding window** of size `k`.
- Start by calculating the sum of the first `k` elements.
- Slide the window by adding the next element and removing the first element of the previous window.
- Keep track of the maximum sum.

### 📋 **Algorithm:**
1. Calculate the sum of the first `k` elements.
2. Slide the window by one element at a time:
   - **Add** the next element (`arr[i]`).
   - **Subtract** the element that falls out of the window (`arr[i - k]`).
3. Update the maximum sum if the new window sum is greater.

### 💻 **Code:**
```java
public class Main {
    public static int maxSum(int[] arr, int k) {
        int maxSum = 0;
        int windowSum = 0;

        // Step 1: Calculate sum of first k elements
        for (int i = 0; i < k; i++) {
            windowSum += arr[i];
        }
        maxSum = windowSum;

        // Step 2: Slide the window
        for (int i = k; i < arr.length; i++) {
            windowSum += arr[i] - arr[i - k];
            maxSum = Math.max(maxSum, windowSum);
        }

        return maxSum;
    }

    public static void main(String[] args) {
        int[] arr = {2, 1, 5, 1, 3, 2};
        int k = 3;
        System.out.println("Sliding Window Max Sum: " + maxSum(arr, k));
    }
}
```

### ⏰ **Time Complexity:** `O(n)`  
### 📦 **Space Complexity:** `O(1)`

---

## 🟣 Dry Run Example

**Array:** `[2, 1, 5, 1, 3, 2]`  
**k:** `3`

### 🔄 Sliding Window Steps:
1. **Initial Window (first 3 elements):** `2 + 1 + 5 = 8` → `maxSum = 8`
2. **Slide 1:** Add `1`, Remove `2`: `8 + 1 - 2 = 7`
3. **Slide 2:** Add `3`, Remove `1`: `7 + 3 - 1 = 9` → `maxSum = 9`
4. **Slide 3:** Add `2`, Remove `5`: `9 + 2 - 5 = 6`

**🎉 Final Max Sum = 9**

---

## ⚖️ Comparison

| Approach        | Time Complexity | Space Complexity | Use Case                  |
|-----------------|-----------------|------------------|---------------------------|
| Brute Force     | O(n × k)        | O(1)             | Small-sized arrays        |
| Sliding Window  | O(n)            | O(1)             | Large-sized arrays, Efficient |

---

💡 **Tip:** Always look for patterns like **sliding windows** when dealing with subarrays of fixed size.

🚀 *Happy Coding!*

