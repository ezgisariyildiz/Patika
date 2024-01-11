# Patika
Temel Python


1- Bir listeyi düzleştiren (flatten) fonksiyon yazın. Elemanları birden çok katmanlı listelerden ([[3],2] gibi) oluşabileceği gibi, non-scalar verilerden de oluşabilir. 


```python
def flatten(l):

    return [e for m in l for e in (m if type(m) is l else [m])]
```


2- Verilen listenin içindeki elemanları tersine döndüren bir fonksiyon yazın. Eğer listenin içindeki elemanlar da liste içeriyorsa onların elemanlarını da tersine döndürün.


```python
def reverse(l):

    l.reverse()
    
    for e in l:
    
        if type(e) == l:
        
            e.reverse()
            
    return l
```
