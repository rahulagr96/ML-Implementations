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

## 10. Use of sort() and sorted()

https://realpython.com/python-sort/

```python
# Sorting the original list and not assigning to other variable
# Use sort()
arr.sort()

# Sorting the original list and assigning to a new variable
# Use sorted()
new_arr = sorted(arr)
```

Both have very different characteristics when it comes to output and in-place modifications, so make sure you think through any application functionality or program that will be using `.sort()` as it can irrevocably overwrite data.

## 11. Important conclusion on division

When we divide any `int` number using `/` operator, we obtain a result as `float`  not as `int`

```python
#Example
n = len(arr)
print(arr[n/2])			# Throws Error
print(arr[int(n/2)])	# Correct way
```

## 12. Understanding For loop in python

Python does not give standard for loop conversion like that of C++ or C#. 

`Remember this:`  Python FOR loops are same as FOREACH of C++/C#

```python
lis = [1, 2, 3, 4, 5]
for i in range(len(lis)):
    print(lis[i])
    i += 2
# O/P ==> 1 2 3 4 5
```

`Alternate way:` Use while loop like this when needed controlled FOR kind of loop

```python
lis = [1, 2, 3, 4, 5]
i = 0
while(i < len(lis)):
    print(lis[i], end = " ")
    i += 2
# O/P ==> 1 3 5
```

## 13. Positive Differance between 2 number (Mod Diff)

```python
abs(a-b)
```

## 14. List to String

```python
s = ['Geeks', 'for', 'Geeks']
print(' '.join(s))
```

