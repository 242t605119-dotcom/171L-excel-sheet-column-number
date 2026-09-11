# LeetCode 171 - Excel Sheet Column Number

## Problem

Given a string `columnTitle` representing an Excel column title, return its corresponding column number.

### Examples

```text
A → 1
B → 2
Z → 26
AA → 27
AB → 28
ZY → 701
```

## Approach

This problem is the reverse of LeetCode 168.

Each letter has a value:

```text
A = 1
B = 2
...
Z = 26
```

For every character, multiply the current result by `26` and add the value of the current character.

The formula is:

```text
result = result * 26 + character_value
```

## Example

For `AB`:

```text
A = 1
B = 2

result = 0
result = 0 * 26 + 1 = 1
result = 1 * 26 + 2 = 28
```

So:

```text
AB → 28
```

## Complexity

* **Time Complexity:** `O(n)`
* **Space Complexity:** `O(1)`

where `n` is the length of the column title.

## Key Concepts

* String traversal
* Character conversion
* Base-26 conversion
* ASCII values
* Mathematical representation

## What I Learned

This problem helped me understand how Excel column names can be converted into numbers using a base-26 style calculation.

It is also the reverse idea of LeetCode 168, where a number is converted into an Excel column title.

## LeetCode Details

* **Problem:** 171
* **Title:** Excel Sheet Column Number
* **Language:** Python
* **Difficulty:** Easy

## Author

T.Nandhini
