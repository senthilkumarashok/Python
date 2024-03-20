# Python

## 1. Enumeration over range 

Enumeration returns the value and index as tupule
```
data = [1,2,3,4]
for idx in range(len(data)):
    print(idx, data[idx])
```
```
for idx, num in enumerate(data):
    print(idx, num)
```

## 2. List comprehensions

## 3. Sort Complex Iterables with sorted()
```
data = [4,3,2,1]
print(sorted(data))
```
```
data = [{"age": 4},{"age": 3},{"age": 2},{"age": 1}]
print(sorted(data, key=lambda x: x["age"]))
```

## 4. Use Set method to avoid duplicates
```
data = [1,2,4,4]
print(set(data))
```
