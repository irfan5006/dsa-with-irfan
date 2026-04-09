# Time Complexity - Complete Notes

## 1. Introduction
Time complexity tells us how the running time of an algorithm grows as the input size increases.  
It does not measure exact time in seconds.

---

## 2. Why Time Complexity is Important
- Helps compare algorithms  
- Helps choose efficient solutions  
- Important for large datasets  

---

## 3. Big-O Notation
Big-O notation is used to describe the upper bound (worst case) of time complexity.

Example:
O(1), O(n), O(n²)

---

## 4. Types of Time Complexity

### **O(1) – Constant Time**
Time does not change with input size.

Example:
```python
arr = [10, 20, 30]
print(arr[0])
```

---

### **O(log n) – Logarithmic Time**
Input size reduces by half each step.

Example:
```python
n = 16
while n > 1:
    n = n // 2
```

---

### **O(n) – Linear Time**
Time increases with input size.

Example:
```python
for i in range(n):
    print(i)
```

---

### **O(n log n) – Linearithmic Time**
Combination of linear and logarithmic.

Example:
Used in merge sort.

---

### **O(n²) – Quadratic Time**
Time grows as square of input.

Example:
```python
for i in range(n):
    for j in range(n):
        print(i, j)
```

---

### **O(2ⁿ) – Exponential Time**
Time doubles with each input.

Example:
```python
def func(n):
    if n == 0:
        return 1
    return func(n-1) + func(n-1)
```

---

## 5. Time Complexity Comparison

| Complexity | Speed |
|-----------|------|
| O(1) | Very Fast |
| O(log n) | Fast |
| O(n) | Medium |
| O(n log n) | Good |
| O(n²) | Slow |
| O(2ⁿ) | Very Slow |

---

## 6. Key Points
- Ignore constants (e.g., O(2n) = O(n))  
- Focus on highest power  
- Nested loops multiply complexity  
- Sequential loops add complexity  

---

## 7. Conclusion
Time complexity helps in writing efficient and scalable code.  
Understanding it is important for coding interviews and real-world problems.
