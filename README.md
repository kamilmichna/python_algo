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
## Selection sort
``` python
def selectionSort():
  minim = -99999
  for x in range(len(tab)):
    for j in range(x,len(tab)):
      if tab[x] > tab[j]:
        swap(x,j,tab)
  return tab
```
## Insertion sort
``` python
def insertion_sort(tab):
  for i in range(1,len(tab)):
    # sprawdzanie podzbioru ulozonego
    for j in range(len(tab[0:i])):
      if tab[j] > tab[i]:
        temp = tab[i]
        tab.pop(i)
        tab.insert(j,temp)
  return tab
```
