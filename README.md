# 🧮 GCD of Odd and Even Sums

🔗 [LeetCode Contest Problem Link](https://leetcode.com/contest/weekly-contest-464/problems/gcd-of-odd-and-even-sums/submissions/1749631995/)

---

## 🧠 Problem Statement

Given an integer `n`, compute the GCD of:
- `sumOdd`: the sum of the first `n` odd numbers
- `sumEven`: the sum of the first `n` even numbers

Return `gcd(sumOdd, sumEven)`

### Example:
```text
Input: n = 4
Output: 4

Explanation:
sumOdd = 1 + 3 + 5 + 7 = 16
sumEven = 2 + 4 + 6 + 8 = 20
gcd(16, 20) = 4
```
## ✅ Approach
We use mathematical formulas to avoid looping:

Sum of first n odd numbers: sumOdd = n²

Sum of first n even numbers: sumEven = n * (n + 1)

Then return gcd(sumOdd, sumEven) using fractions.gcd() for Python 2 compatibility.

## 📊 Complexity Analysis
Time Complexity: O(log n)

GCD computation is logarithmic.

Space Complexity: O(1)

Only uses a few integer variables.
