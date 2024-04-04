## Question:
  Given a custom order defined by a string `Order` (permutation of the 26 English alphabet), and a list of production code `productionCode` (strings), 
  output the lexicographical ordering of the codes in the `productionCode` based on the new alphabet order `Order`.
### input：
> In [1]: alphabet = "bafmxpzv"
>
> In [1]: a = ['af', 'ax', 'am', 'ab', 'zvpmf'] 
  
      
> Out [1]: ['ab', 'af', 'am', 'ax', 'zvpmf']

## Python:
```python
alphabet = "bafmxpzv"
a = ['af', 'ax', 'am', 'ab', 'zvpmf'] 
return sorted(a, key=lambda word: [alphabet.index(c) for c in word])

Out[34]: ['ab', 'af', 'am', 'ax', 'zvpmf']
```
