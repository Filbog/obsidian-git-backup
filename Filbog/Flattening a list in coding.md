#coding #python
Flattening a list is essentially making a 1D list from a 2D+ list, for example we have a 2D list:

```
list = [
[1, 2, 3], [4, 5, 6], [7, 8, 9]
]
```
And the flattened list would be:
```
flattened_list = [1, 2, 3, 4, 5, 6, 7, 8, 9]
```
We could achieve the flattened list with this (convoluted) list comprehension:
```
flattened_list = [e for p in list for e in p]
```
