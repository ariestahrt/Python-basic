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
