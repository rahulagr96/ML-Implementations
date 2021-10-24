# Python Tips and Tricks

 ## 1. Take multiple inputs and store in a list

```python
x = list(map(str, input().split()))
```

## 2. Take multiple input in ‘n’ var

``` python
x,y,z = input().split()
```

``` python
x, y, z, n = (int(input()) for _ in range(4))
```

## 3. Swap Character Case in a line

``` python
print("".join(map(str.swapcase, input())))
```

## 4. Split line by space char and join by '-'

```python
def split_and_join(line):
    return "-".join(line.split(" "))
```

## 5. String Tips

```python
print "Hello {0} {1}! You just delved into python.".format(raw_input(), raw_input())
```

##### Print up-to two decimal places

``` python
print("{:.2f}".format(myFloatNum))
```

##### Print in same line ==> use endl = '' or ' ' or '\n' or '@' or '-'

``` python
print("Welcome to" , end = ' ') 
print("GeeksforGeeks", end = ' ')
```

## 6. Change specific char in string

``` python
print(string[:position] + "k" + string[(position+1):])
Eg: string[:5] + "k" + string[6:]
```

## 7. Pass keyword

The `pass` statement is used as a placeholder for future code.

When the `pass` statement is executed, nothing happens, but you avoid getting an error when empty code is not allowed.

Empty code is not allowed in loops, function definitions, class definitions, or in if statements.

## 8. Max of a dictionary

``` python
self.most_freq = max(c_dict, key=c_dict.get)
```

## 9. Capitalize every first char of string 

```python
a_string = input().split(' ')
print(' '.join((word.capitalize() for word in a_string)))
```

