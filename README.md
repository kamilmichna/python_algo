# Python alghorithms 
repo with python alghoritms examples

## function to swap two elements in array
``` python
def swap(a,b,tab):
  temp = tab[a]
  tab[a] = tab[b]
  tab[b] = temp
```


## Bubble sort
``` python
def bubble_sort():
  while True:
    sorted = False
    for x in range(len(tab)-1):
      if tab[x] < tab[x+1]:
        sorted=True
        swap(x,x+1,tab)
    if not sorted:
      return tab
```
