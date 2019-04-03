---
Layout: post
Title:  "Split-and-Join"
Date:   2019-04-03 19:54:00
Category: Python_for_Machine_Learning
Chapter : 2. Pythonic Code
---

# 2019-04-03-Split-and-Join.md

## 1. Split 함수

  - .split()

  - String Type의 값을 나눠서 List 형태로 변환

```python
#빈 칸을 기준으로 문자열 나누기
items = "zero one two three".split()
print(items)
#","을 기준으로 문자열 나누기
example = "python, jquery, javascript"
example.split(",")
#리스트에 있는 각 값을 a, b, c 변수로 unpacking
a, b, c = example.split(",")
```
## 2. Join 함수

  - "".join()

  - String List를 합쳐 하나의 String으로 반환할 때 사용

```python
colors = ["red", "blue", "green", "yellow"]
result = "".join(colors)
result
#연결 시 빈칸 1칸으로 연결
result = " ".join(colors)
result
#연결 시 ","으로 연결
result = ",".join(colors)
result
#연결 시 "-"1칸으로 연결
result = "-".join(colors)
result
```
