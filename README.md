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



# PRACTICAL 8 : Graph Coloring using Backtracking 

##  Overview
This project implements the **Graph Coloring Problem** using the **Backtracking algorithm** in Java.  
The goal is to assign different colors (or frequencies) to each vertex (or cell tower) such that no two adjacent vertices share the same color.  

It is a real-life model of the **GSM network frequency assignment problem**, where each tower must use a different frequency from its neighbors to avoid interference.

---

##  Problem Statement
Given:
- A graph represented by an adjacency matrix.
- A number of available colors (frequencies).

Find a way to color all vertices such that no two adjacent vertices have the same color.

If no such assignment is possible, display a suitable message.

---

##  Algorithm Used
**Backtracking Algorithm**

Steps:
1. Assign a color to a vertex.
2. Check if the assignment is valid (no adjacent vertex has the same color).
3. Recursively assign colors to the next vertex.
4. If a conflict occurs, backtrack and try the next color.
5. Continue until all vertices are successfully colored or no valid configuration exists.

---

##  Example Input / Output

### Input
Enter number of vertices: 4
Enter adjacency matrix:
0 1 1 1
1 0 1 0
1 1 0 1
1 0 1 0
Enter number of colors (frequencies): 3

### Output
Color assignment to vertices:
Vertex 1 ---> Color 1
Vertex 2 ---> Color 2
Vertex 3 ---> Color 3
Vertex 4 ---> Color 2
---

## 🧾 Features
- Uses **Backtracking** for graph coloring.
- Works for any adjacency matrix.
- Prints a valid color assignment or a message if no solution exists.
- Demonstrates a practical application in **cellular network frequency planning**.


