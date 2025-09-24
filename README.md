# DAA-LAB – Practical 5

 Aim  
Implement Longest Common Subsequence (LCS) algorithm to find the length and LCS for DNA sequences.  
Also implement Longest Repeating Subsequence (LRS) as a variation of the LCS problem.  

---

 Problem Statement  

DNA sequences can be viewed as strings of A, C, G, and T. Finding similarities between two DNA sequences is important in bioinformatics.

### Task 1: Longest Common Subsequence (LCS)  
- Input: Two DNA sequences `X` and `Y`  
- Output:  
  - Cost (DP) matrix with all costs and directions  
  - Final cost (length) of LCS  
  - The LCS sequence  

**Example (practical input)**  
X = AGCCCTAAGGGCTACCTAGCTT
Y = GACAGCCTACAAGCGTTAGCTTG
**One LCS found by program:** `AGCCCAAGGTTAGCTT` (length = 16)

---

### Task 2: Longest Repeating Subsequence (LRS)  
- Input: A string `S`  
- Output: The Longest Repeating Subsequence (LRS) within `S`  

**Example:**  
S = AABCBDC
LRS = ABC or ABD


Complexity

Time: O(m * n) where m = |X|, n = |Y|

Space: O(m * n) (needed to print the full cost & direction matrices)
