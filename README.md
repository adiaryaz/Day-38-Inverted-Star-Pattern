# Day-38-Inverted-Star-Pattern
Day 38/100 - Python Program to Print Inverted Star Pattern

# Print Inverted Star Pattern
A program to generate and display a descending (inverted) right-angled triangle pattern using asterisk (`*`) characters.

## 📝 Description

This program prompts the user to input the desired number of rows for a geometric star pattern. It then dynamically generates an inverted triangle, where the first row contains the maximum number of stars, and each subsequent row contains one less star until it reaches a single star.

Instead of using complex nested loops (one loop for rows, one for columns), this script takes a highly efficient "Pythonic" approach. It uses a single `for` loop combined with the `range(start, stop, step)` function configured to count backwards (`range(rows, 0, -1)`). Inside the loop, it utilizes Python's string multiplication feature (`"*" * i`) to instantly generate the correct number of stars for that specific row.

---

## 🎯 Problem Statement

### Input:

* **Input 1:** A single integer representing the total number of `rows` for the pattern.

### Output:

* A multi-line visual pattern of asterisks (`*`), starting with `rows` number of asterisks on the first line and decreasing by one on each subsequent line.

### Rules:

1. The program must accept an integer input from the user.
2. The program must utilize a `for` loop that iterates in reverse. The `range()` function must start at `rows`, end before `0`, and decrement by `-1`.
3. Inside the loop, the program must print the asterisk character repeated `i` times, where `i` is the current loop variable.

---

## 💡 Examples

### Example 1 (Standard Pattern)

**Input:**

```
5


```

**Output:**

```
*****
****
***
**
*


```

**Explanation:** The loop starts at 5 and steps down to 1.

* Line 1: `"*" * 5` prints 5 stars.
* Line 2: `"*" * 4` prints 4 stars.
* This continues until `"*" * 1` prints 1 star.

### Example 2 (Smaller Pattern)

**Input:**

```
3


```

**Output:**

```
***
**
*


```

**Explanation:** The program correctly scales the inverted triangle to start with a maximum width of 3.

### Example 3 (Single Row)

**Input:**

```
1


```

**Output:**

```
*


```

**Explanation:** The loop `range(1, 0, -1)` executes exactly once, printing a single star before terminating.

### Example 4 (Zero or Negative Input)

**Input:**

```
0


```

**Output:**

```



```

**Explanation:** If the input is 0 or a negative number, the start condition of the `range` is already less than the stop condition (with a negative step). The loop evaluates as empty and executes zero times, leaving a blank output.

---

## 🚀 How to Use

1. **Clone this repository** (or save the script)

```bash
git clone https://github.com/adiaryaz/Day-38-Inverted-Star-Pattern.git
cd inverted-star-pattern


```

2. **Run the program**:

```bash
python main.py


```

Enter an integer when prompted to see the inverted star sequence printed to your console.
