# Vectorization Using Numpy

Deep learning and machine learning algorithms work on very large data sets, it is thus required to be able to get results fast. Iterating over large data sets using constructs like loops can get slower, vectorization on the other hand leverage parallel processing of GPU and CPU to do operations much faster. Thus vectorization is very important for deep learning.

NumPy, or Numerical Python is Python library that can be used to implement vectorization.

Take the example of computing liner regression equation using NumPy:


```
z = (wT * x) + b

w = |---|        x = |---|
    | w1|            | x1|
    | w2|            | x2|
    | w3|            | x3|
    | . |            | . |
    | . |            | . |
    | . |            | . |

# Non-vectorized version
z = 0
for i in range(n):
    z += w[i] * x[j]
z += b

# Vectorized version
z = np.dot(w.T, x) + b
```

Vectorization helps get rid of for loops.

## Creating NumPy Arrays

NumPy library provides method to create multi-dimensional array from python lists or sequences like:

```
one_dim_array = np.array([1, 2, 3, 4])
two_dim_array = np.array([[1, 2], [3, 4]])
```

Other useful methods provided by the library include: `zeros`, `ones`, `random`, `arange`:

```
np.zeros((2, 3))
array([[0., 0., 0.],
       [0., 0., 0.]])

np.ones((2, 3))
array([[1., 1., 1.],
       [1., 1., 1.]])

from numpy.random import default_rng
np.random.rand(2,3)
array([[0.77395605, 0.43887844, 0.85859792],
       [0.69736803, 0.09417735, 0.97562235]])

np.arange(10)
array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])
```

## Other useful NumPy methods
Whenever possible for loops should be avoided in neural network programming. NumPy library provides methods that can be executed on each element in vector, for example: 
- `np.exp`: to find exponent of each value in vector
- `np.log`: to find log of each value in vector
- `np.abs`: to find absolute value of each value in vector
- `np.maximum(v, 0)`: to find maximum when xcompared to `0` for each element in vector

Additionally an operation done on the vector is executed on each element of the vector, for instance
- `v**2`: gives new vector of square of each element in the vector
- `1/v`: gives new vector of inverse of each lement in the vector
- `v + 5`: gives new vector of values with 5 added to each element of the vector

This second technoque is also called as broadcasting and used widely and deep learning. In theory Python broadcasts the value to make an equal size matrix and then performs the operation as shown below:

```
---                         ---      -----              -----
|1|                         |1|      |100|              |101|
|2|   + 100         =       |2|   +  |100|       =      |102|
|3|                         |3|      |100|              |103|
|4|                         |4|      |100|              |104|
---                         ---      -----              -----
```

```
-------                            -------       -------------               -------------
|1 2 3|      -------------         |1 2 3|       |100 200 300|               |101 202 303|
|4 5 6|   +  |100 200 300|    =    |4 5 6|   +   |100 200 300|        =      |104 205 306|
-------      -------------         -------       -------------               -------------
```
