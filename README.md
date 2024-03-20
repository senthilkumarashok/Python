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

## 5. Remember the generator which will save memory in case of large datasets
```
import sys
my_list = [i for i in range(10000)]
print(type(my_list))
print(sys.getsizeof(my_list), "bytes")

my_gen = (i for i in range(10000))
print(type(my_gen))
print(sys.getsizeof(my_gen), "bytes")
```

## 6. Use Get and set the default for the dictionary

```
if you use attribute name and key does not exist . it will throw an error
data = [{"age": 4},{"age": 3},{"age": 2},{"age": 1}]
print(data[0].get("name","defaultName"))
```

## 7. count hashable objects with Collections.counter
```
from collections import Counter
data = [1,2,3,4,3,4,4]
counter = Counter(data)
print(counter)
print(counter[4])
```

## 8. use format strings using f
```
name = "xxxxx"
i = 10
template = f"{name} range is between {i} and {i*i}"
print(template)
```

## 9. concat strings with join (why ?)
```
my_list = ["my", "name", "is", "xxx"]
print(" ".join(my_list))
```

## 10. Merging dictionaries
```
dict1 = {"name": "zz", "age": 6}
dict2 = {"name": "yy", "city": "newyork"}
print({**dict1,**dict2})
```

## 11. simplify if statement with in
```
colors = ['green', 'red', 'yello']
color = 'green'
if color in colors:
    print(True)
```
