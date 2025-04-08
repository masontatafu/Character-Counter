# Lab 6 – Character Counter

This Python notebook lets the user enter a sentence, then builds a dictionary showing how many times each letter appears. It ignores spaces and treats letters case-insensitively.

## Technologies
- Python 3.x

## Example
```python
sentence = input("Enter a sentence: ")
counts = {}
for char in sentence.lower():
    if char.isalpha():
        counts[char] = counts.get(char, 0) + 1
