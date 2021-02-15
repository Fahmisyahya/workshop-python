# Minggu-01
- [Minggu-01](#minggu-01)
- [Introduction Python](#introduction-python)
- [Interpreter dan Environtmennya](#interpreter-dan-environtmennya)
    - [Interactive Editing](#interactive-editing)
    - [Code Compilation](#code-compilation)
    - [History Substition](#history-substition)
  - [Using Interpreter](#using-interpreter)
  - [Environtment](#environtment)
- [An Informal Introduction to Python](#an-informal-introduction-to-python)
# Introduction Python
* Python adalah sebuah "High-Level" programming language (Bahasa Pemrograman tingkat tinggi) yang mudah digunakan dan memiliki banyak fungsi. 
* Python adalah sebuah bahasa pemrograman interpreter, jadi tidak ada proses kompilasi untuk menjalankan program python. 
* Python memperbolehkan untuk membagi program python ke beberapa module untuk dapat digunakan kembali di program python yang lain.
* Python adalah bahasa yang extensible.
* Python adalah bahasa yang read-able.
* Python tidak hanya dapat digunakan untuk membuat program CLI, Python juga dapat digunakan untuk membuat program berbasis GUI.

# Interpreter dan Environtmennya
Interpreter adalah sebuah alat yang dapat digunakan untuk menjalankan kode python langsung dari commmand prompt ataupun terminal. Fitur dari intrepeter python antara lain :

### Interactive Editing
Anda dapat langsung menuliskan kode python di dalam command prompt ataupun terminal dan sekaligus hasil dari kode akan ditampilkan.
### Code Compilation
Anda dapat menuliskan beberapa huruf dari syntax python dan lalu menekan tombol ```tab``` dan syntax anda akan terlengkapi sendiri.
### History Substition
Kode yang pernah anda tulis di intrepeter, dapat dilihat dan digunakan kembali.

## Using Interpreter
Untuk menjalankan interpreter, ketikkan ```python3``` di command prompt maupun terminal atau dengan cara menjalankan exec file dari python di directory ```/usr/bin/python3```.
![Interpeter](https://i.ibb.co/8bbK1Yc/Screenshot-from-2021-02-09-09-58-56.png)

Interactive code menggunakan intrepeter shell

Source Code :
```python
the_world_is_flat = True
if the_world_if_flat:
    print("Be careful not to fall off!")
```

On Intrepeter :
![Interpreter](https://i.ibb.co/WD8NvrG/Screenshot-from-2021-02-09-10-07-47.png)

## Environtment
Secara _default_ , Encode dari python interpreter adalah encode UTF-8. Namun, encode ini bisa di ubah dengan menggunakan sebuah komentar yaitu 
```
# -*- coding: _encoding_ -*_
```

On Interpreter
![Interpreter](https://i.ibb.co/yNFCqG9/Screenshot-from-2021-02-09-10-20-00.png)

# An Informal Introduction to Python
- How to add comments
```python
# This is first comment
spam = 1 # the second comment
         # the thir comment
text = "# This is not a comment because it's inside quotes."
```
- Python as Calculator
```python
print(2 + 2)
print(50 - 5 * 6)
print((50 - 5 * 6) / 4)
print(8 / 5) # division always returns a floating point number
print(17 / 3) # classic division returns a float
print(17 // 3) # floar division discards the fractional part
print(17 % 3) # the % operator returns the remainder of the division
print(5 * 3 + 2) # result * divisor + remainder
print(5 ** 2) # 5 squared
print(2 ** 7) # 2 to the power of 7

width = 20
height = 5 * 9
print(width * height)

print(4 * 3.75 - 1)

tax = 12.5 / 100
price = 100.50
_ = price * tax
print(_)
print(price + _)
print(round(_, 2))
```
- String
```python
print('spam eggs') # single quotes
print('doesn\'t') # use \' to escape single quotes
print("doesn't") # use double quotes instead
print('"Yes," they said.')
print("\"Yes,\" they said.")
print('"Isn\'t, " they said.')
print('C:\some\name')
print(r'C:\some\name')
print("""\
Usage: thingy [OPTIONS]
     -h                    Display this usage message
     -H hostname           Hostname to connect to
    """)
print(3 * 'un' + 'ium')
print('Py' 'thon')
text = ('Put several strings within parentheses '
        'to have them joined together.')
print(text)
prefix = 'Py'
print(prefix + "thon")
word = 'Python'
print(word[0])
print(word[5])
print(word[-1])
print(word[-2])
print(word[-6])
print(word[0:2])
print(word[2:5])
print(word[:2] + word[2:])
print(word[:4] + word[4:])
print(word[:2])
print(word[4:])
print(word[-2:])
```
- Lists
```python
squares = [1, 4, 9, 16, 25]
print(squares)
print(squares[0])
print(squares[-1])
print(squares[-3:])
print(squares[:])
print(squares + [36, 49, 64, 81, 100])
cubes = [1, 8, 27, 65, 125]
cubes[3] = 4 ** 3
print(cubes)
cubes.append(216)
cubes.append(7 ** 3)
print(cubes)
letters = ['a', 'b', 'c', 'd', 'e', 'f', 'g']
print(letters)
letters[2:5] = ['C', 'D', 'E']
print(letters)
letters[2:5] = []
print(letters)
letters[:] = []
print(letters)
a = ['a', 'b', 'c']
n = [1, 2, 3]
x = [a, n]
print(x)
print(x[0])
print(x[0][1])
a, b = 0, 1
while a < 10:
    print(a)
    a, b = b, a+b
i = 256 * 256
print('The value of i is ', i)
a, b = 0, 1
while a < 1000:
    print(a, end=', ')
    a, b = b, a+b
```