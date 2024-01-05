
# Types of Build-In modules

Here are the major categories of built-in Python modules along with their purposes:

## Mathematical and Numerical Modules:


### Advanced functionalities:

 Are you curious about advanced functionalities like complex number operations, numerical precision control, or statistical distributions?

### 1. Math:
 
 Provides access to mathematical functions like trigonometric, logarithmic, exponential, and numerical operations.

```python
import math

 Trigonometric functions

print(math.sin(math.pi / 4)) 

# Output:0.7071067811865475

print(math.cos(math.pi))

 # Output: -1.0

print(math.tan(0)) 

# Output: 0.0

 Logarithmic and exponential functions

print(math.log10(100))

# Output: 2.0

print(math.exp(1))  

# Output: 2.718281828459045

 Rounding functions

print(math.ceil(3.14))

# Output: 4.0

print(math.floor(3.99))

# Output: 3.0

 Mathematical constants

print(math.pi)  

# Output: 3.141592653589793

print(math.e) 

# Output: 2.718281828459045

```

### 2. random:
 
 Generates random numbers and implements functions for random sampling and shuffling.

```python
from random import *
random_number = randint(1, 10)  

# Generate a random integer between 1 and 10

print(random_number)

#output:9
 

```

### 3. statistics:
 
 Calculates basic statistical measures like mean, median, mode, variance, standard deviation, and more.


## Data Handling Modules:


### 1. collections:

Offers specialized container data types like namedtuples, deques, counters, and OrderedDict.

```python
from collections import namedtuple
Person = namedtuple('Person', ['name', 'age', 'city'])
person = Person('Alice', 30, 'New York')
print(person.name)  

# Output: Alice

```

### 2. datetime: 

Handles dates and times, allowing operations like manipulation, formatting, and calculations.

```python
import datetime
now = datetime.datetime.now()
print(now.strftime("%Y-%m-%d %H:%M:%S"))  

# Output: e.g., 2024-01-05 15:35:00

```

### 3. json: 

Encodes and decodes JSON data, facilitating data exchange with web services.

### 4. re: 

Implements regular expression operations for pattern matching and text manipulation.

## System Interaction Modules:


### 1. os: 

Provides functions for interacting with the operating system, such as file system operations, environment variables, and process management.

```python
import os
print(os.getcwd())  # Get the current working directory
os.mkdir('new_folder')  

# Create a new folder

```

### 2. sys: 

Accesses system-specific parameters and functions, including command-line arguments and interpreter information.


```python
import sys
print(sys.argv)  # Access command-line arguments
#Output:['c:/Users/hp/Desktop/a/ab.py']
```

### 3. Platform: 

Provides information about the current platform and operating system.


## File I/O Modules:

### 1. io: 

Offers a core set of tools for working with various types of I/O, including files, streams, and buffers.

```python
import io
with io.open('my_file.txt', 'w', encoding='utf-8') as file:
    file.write('Hello, world!')
#Output:PS C:\Users\hp\Desktop\a> & C:/Users/hp/AppData/Local/Programs/Python/Python311/python.exe c:/Users/hp/Desktop/a/ab.py

```

### 2. OS.path: 

Manipulates file paths and names, handling path manipulations and directory operations.


## Concurrency Modules:


### 1. Threading: 

Enables multithreaded programming for concurrent execution of tasks.

```python
import threading
def worker():
    print("Hello from a thread!")
thread = threading.Thread(target=worker)
thread.start()
#output:Hello from a thread!
```

### 2. Multiprocessing: 

Utilizes multiple processes for parallel execution across multiple cores.


## Networking Modules:


### 1. Socket: 

Provides access to the underlying socket API for network communication.

```python
import urllib.request
response = urllib.request.urlopen('https://www.example.com')
print(response.read())  # Read the response content
# Output: PS C:\Users\hp\Desktop\a> & C:/Users/hp/AppData/Local/Programs/Python/Python311/python.exe c:/Users/hp/Desktop/a/ab.py

```

### 2. urllib: 

Offers functions for working with URLs and retrieving data from the web.

### 3. http.client: 

Implements a client-side HTTP protocol for connecting to web servers.

## Other Useful Modules:


### 1. Itertools: 

Provides functions for working with iterators and generating efficient sequences.

### 2. Functools: 

Offers high-order functions and tools for working with functions and callable objects.

### 3. operator: 

Contains a collection of built-in operators as functions for convenient manipulation.

