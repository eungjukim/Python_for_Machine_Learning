---
Layout: post
Title:  "List_Comprehension"
Date:   2019-04-03 20:09:00
Category: Python_for_Machine_Learning
Chapter : 2. Pythonic Code
---

# 2019-04-03-List_Comprehension.md

## 1. for loop + append 사용

```python
result = []
for i in range(10):
  result.append(i)

print(result)
```
## 2. List Comprehension 사용

```python
result = [i for i in range(10)]
print(result)

result = [i for i in range(10) if i % 2 == 0]
print(result)
```

## 3. Nested for loop

```python
word_1 = "Hello"
word_2 = "World"
result = [i + j i in word_1 for j in word_2]

print(result)
```
## 4. Nested for loop + if문

```python
case_1 = ["A", "B", "C"]
case_2 = ["D", "E", "F"]

result = [i + j for i in case_1 for j in case_2]
print(result)

result = [i + j for i in case_1 for j in case_2 if not(i==j)]
result.sort()

print(result)
```

## 5. Split + List Comprehension

```python
words = "The quick brown fox jumps over the lazy dog".split()
print(words)

stuff = [[w.upper(), w.lower(), len(w)] for w in words]

for i in stuff:
  print(i)
```
