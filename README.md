## Experiment 2

## NUMERICAL PYTHON (NUMPY)

##### Amiel Elestin M. Cruz
##### 2ECE-D

### 1. Normalization Problem
Normalization is one of the
most basic preprocessing techniques in data analytics. 
This involves centering and scaling process. Centering 
means subtracting the data from the mean and scaling means 
dividing with its standard deviation. Mathematically, normalization
can be expressed as: 𝑍 = 𝑋 − 𝑥̅  / 𝜎

import numpy as np 

x = np.random.random((5,5))

print (x)

a = x.mean()

b = x.std()

normal = (x-a)/b

print (normal)

np.save ('X_normalized.npy', normal)


### 2. Divisible by 3 Problem 
Create the following 10 x 10 ndarray.
which are the squares of the first 100 positive integers.
From this ndarray, determine all the elements that are divisible by 3. 

a = np.arange(1,101)
e = np.square (a)
m = e.reshape (10,10)

print(m)

c = m [m%3==0]

print (c)

## Explanation:

To solve the normalization problem, we should first declare to import numpy as np
and we declare the x = np.random.random((5,5)) which will give us 5x5 random numbers.
Next, we declared that a = to the mean of x and b = to the standard deviation. We subtracted
every random number from X to the overall mean and divided it by its standard deviation. I declared
print (normal) to perform the operation and show the result. Lastly, I saved it as npy to access the NUMPY.

To solve the Divisible by 3 problem, we need 1 to 100, square every number and reshape it to 10x10. 
Since np.arange uses the  code to create an array of evenly spaced values from a to be excluding b so we input 
(1,101) 1 as a and 101 as b we declared that a = np.arange(1,101). We declared e as np.square(a) to square all 
the values from a. The last is we declared m = e.reshape(10,10) to arrange the value with 10x10 dimensions. I 
encoded print(m) to show all the squared values of 1 to 100 in a 10x10 dimension. Next, we declared c=m and [m%3==0]
to sort out the numbers that are divisible by 3. I encoded print (c) to show all the numbers that are divisible by 3.
Lastly, I saved it as npy to access the NUMPY









