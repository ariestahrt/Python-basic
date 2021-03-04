# Python-basic


## Membuat Program Hello-World
Python adalah bahasa yang sangat sederhana, dan memiliki sintaks yang sangat mudah. Ini mendorong pemrogram untuk memprogram tanpa kode boilerplate (disiapkan). Direktif paling sederhana di Python adalah perintah "print" - ini hanya mencetak sebuah baris (dan juga menyertakan baris baru, tidak seperti di C).

- Kode Program
```python
print("Halo dunia!")
print("Halo dunia!")
```
- Output
```console
Halo dunia!
Halo dunia!
```

Fungsi print() akan memberikan output variabel yang diberikan ditambah dengan newline. Lalu bagaimana cara agar fungsi print() tidak memberikan newline?
- Kode Program
```python
print("Halo dunia!", end="")
print("Halo dunia!")
```
- Output
```console
Halo dunia!Halo dunia!
```

Fungsi print() juga dapat diberikan parameter lebih dari satu, setiap parameter akan dipisahkan dengan ' '
- Kode Program
```python
print("Total buku :", 2)
```
- Output
```console
Total buku : 2
```


## Variabel dan Tipe Data
Python sepenuhnya berorientasi objek, dan tidak "statically typed". Kita tidak perlu mendeklarasikan variabel sebelum menggunakannya, atau mendeklarasikan tipenya. Setiap variabel dalam Python adalah sebuah objek.

### Membuat variabel
Variabel dapat dibuat langsung dengan nilainya sebagai berikut:
- Kode Program
```python
a=7
b=10
c,d=11,12
print(a)
print(b)
print(c)
print(d)
```

- Output
```console
7
10
11
12
```


### Number
- Kode Program
```python
a=7 # Integer
b=7.0 # Float
c=a+b
print(a, b, c)
```

- Output
```console
7 7.0 14.0
```

### Strings
- Kode Program
```python
str1='Bayucaraka ITS'
str2="Bayucaraka ITS"
str3='''Magang
Bayucaraka
ITS'''
print(str1)
print(str2)
print(str3)
```

- Output
```console
Bayucaraka ITS
Bayucaraka ITS
Magang
Bayucaraka
ITS
```

### Array

Array dalam python sangat sederhana

- Kode Program
```python
# Deklarasi variabel yang menyatakan array dapat:
arr = []
arr2 = [1,2,3]

# Memasukan element kedalam array | .append()
arr.append(1)     # arr = [1]
arr.append(2)     # arr = [1,2]
arr.append("str") # arr = [1,"str"]

# Memasukan element kedalam array pada posisi tertentu | .insert()
arr = ['Ayam', 'Sapi', 'Kambing']
arr.insert(0, 'Babi')
print(arr) # ['Babi', 'Ayam', 'Sapi', 'Kambing']

# Menghapus nilai tertentu | .remove()
arr=[1,2,3,4,3]
arr.remove(3) # arr3=[1,2,4,3]

# Mengosongkan nilai array | .clear()
arr.clear() # arr3=[]

# Menghitung banyaknya nilai tertentu | .count()
arr = [1,3,4,5,2,6,3]
x=arr.count(3)
print(x) # 2

# Menggabungkan dua array | .extend()
fruits = ['apple', 'banana', 'cherry']
cars = ['Ford', 'BMW', 'Volvo']
fruits.extend(cars)
print(fruits) # ['apple', 'banana', 'cherry', 'Ford', 'BMW', 'Volvo']

# Mengurutkan array | .sort()
arr = [1,9,2,6]
arr.sort() # Sort secara ascending
print(arr)
arr.sort(reverse=True) # Sort secara descending
print(arr)

```

## Operasi
Operasi di python ada banyak :D

### Operasi aritmatika
#### Operasi +-/*
- Kode Program
```python
number = 1 + 2 * 3 / 4.0
print(number)
```
- Output
```console
2.5
```
#### Operasi modulo
- Kode Program
```python
remainder = 11 % 3
print(remainder)
```
- Output
```console
2
```

#### Operasi pangkat
- Kode Program
```python
squared = 7 ** 2
cubed = 2 ** 3
print(squared)
print(cubed)
```
- Output
```console
49
8
```

### Operasi pada strings
- Kode Program
```python
helloworld = "hello" + " " + "world"
print(helloworld)
```
- Output
```console
hello world
```
- Kode Program
```python
lotsofhellos = "hello" * 10
print(lotsofhellos)
```
- Output
```console
hellohellohellohellohellohellohellohellohellohello
```

### Operasi pada array
- Kode Program
```python
even_numbers = [2,4,6,8]
odd_numbers = [1,3,5,7]
all_numbers = odd_numbers + even_numbers
print(all_numbers)
```
- Output
```console
[1, 3, 5, 7, 2, 4, 6, 8]
```

## Kondisi
Dalam python penulisan kondisional if else sedikit berbeda dari bahasa C
### Kondisi Boolean
Operator "and" dan "or" mengizinkan pembuatan ekspresi boolean yang kompleks, misalnya:
- Kode Program
```python
nama = "Gon"
umur = 12
if nama == "Gon" and umur == 12:
    print("Namanya benar Gon dan umurnya 12.")

if name == "Gon" or name == "iKuuy":
    print("Namanya benar Gon atau iKuuy.")
```

### Kondisi "in"
Operator "in" dapat digunakan untuk memeriksa apakah objek tertentu ada dalam wadah objek
- Kode Program
```python
name = "Gon"
if name in ["Gon", "Anisa", "iKuuy"]:
    print("Nama berada dalam daftar.")
```

### Syntax Lainnya
- Kode Program
```python
x = 2
if x == 2:
    print("X == 2")
elif x == 3:
    print("X == 3")
else:
    print("Bukan 2 dan bukan 3")
```

## Perulangan (Loop)
Dalam python ada dua tipe perulangan yaitu for dan while

### For
Perulangan for dapat digunakan pada array
- Kode Program
```python
primes = [2, 3, 5, 7]
for prime in primes:
    print(prime)
```
- Output
```console
2
3
5
7
```

Perulangan for dapat juga digunakan seperti berikut:
- Kode Program
```python
# Prints out the numbers 0,1,2,3,4
for x in range(5):
    print(x)

# Prints out 3,4,5
for x in range(3, 6):
    print(x)

# Prints out 3,5,7
for x in range(3, 8, 2):
    print(x)
```

### While
Perulangan while digunakan seperti berikut
- Kode Program
```python
# Prints out 0,1,2,3,4

count = 0
while count < 5:
    print(count)
    count += 1  # This is the same as count = count + 1
```

## Fungsi
Fungsi adalah cara mudah untuk membagi kode Anda menjadi blok yang berguna, mudah dibaca, dan dapat digunakan kembali. Adapun cara membuat fungsi adalah sebagai berikut:
- Fungsi tanpa parameter
```python
def my_function():
    print("Hello From My Function!")

my_function()
```

- Fungsi dengan parameter

```python
def my_function(a,b):
    print("Nilai a", a)
    print("Nilai b", b)

my_function(1,"bayu")
```
