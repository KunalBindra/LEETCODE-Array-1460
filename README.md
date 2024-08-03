# LEETCODE-Array-1460
## Dry Run: `canBeEqual` method

### Understanding the Code
The provided code defines a class `Solution` with a method `canBeEqual` that takes two integer arrays, `target` and `arr`, as input and returns a boolean value. The method attempts to determine if the two arrays can be equal by following these steps:

1. **Sorting:** Both `target` and `arr` arrays are sorted in ascending order using `Arrays.sort`.
2. **Comparison:** The sorted arrays are compared using `Arrays.equals`. If they are equal, the method returns `true`; otherwise, it returns `false`.

### Dry Run Example
Let's consider two example inputs:

**Input 1:**
```
target = [1, 2, 3]
arr = [1, 1, 3]
```

**Dry Run:**
1. `Arrays.sort(target)`: `target` becomes [1, 2, 3]
2. `Arrays.sort(arr)`: `arr` becomes [1, 1, 3]
3. `Arrays.equals(target, arr)`: Returns `false` because the elements at index 1 are different.

**Output:** `false`

**Input 2:**
```
target = [1, 2, 3]
arr = [3, 2, 1]
```

**Dry Run:**
1. `Arrays.sort(target)`: `target` becomes [1, 2, 3]
2. `Arrays.sort(arr)`: `arr` becomes [1, 2, 3]
3. `Arrays.equals(target, arr)`: Returns `true` because all elements are equal.

**Output:** `true`
