2024-08-21

Important to remember: **dictionaries are inherently unordered**. We can iterate over them, but they don't have indeces per se or anything.

### Sort by keys
Example input:
```python
example_input = {2:3, 1:89, 4:5, 3:0}

output = dict(sorted(example_input.items()))
```
Output:
```python
{1: 89, 2: 3, 3: 0, 4: 5}
```

### sort by values
```python
input = {1: 2, 3: 4, 4: 3, 2: 1, 0: 0}
output = dict(sorted(input.items(), key=lambda item: item[1]))
```

In both cases, sorted() method itself gives us a list of tuples. Dict() turns them into a dictionary
### Hashtags:
#python #coding #codingfundamentals


### References (source material, similar notes):
