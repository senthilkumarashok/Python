# Python

## Enumeration over range 

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

## List comprehensions

## Sort Complex Iterables with sorted()

```
data = [4,3,2,1]
print(sorted(data))
```
```
data = [{"age": 4},{"age": 3},{"age": 2},{"age": 1}]
print(sorted(data, key=lambda x: x["age"]))
```
