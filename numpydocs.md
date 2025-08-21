# np.diff
a=[x1,x2], np.diff(a) => x2-x1
a=[x1,x2,x3], np.diff(a) => [x2-x1, x3-x2]


# np.concatenate
a = np.array([[1, 2], [3, 4]])
b = np.array([[5, 6]])

_np.concatenate((a, b), axis=0)_
**Output**
array([[1, 2],
       [3, 4],
       [5, 6]])

_np.concatenate((a, b.T), axis=1)_
**Output**
array([[1, 2, 5],
       [3, 4, 6]])

_np.concatenate((a, b), axis=None)_
**Output**
array([1, 2, 3, 4, 5, 6])


# np.tile
_Clone an array n times_

->a = np.array([[1,2],[2,3]])
->np.tile(a,(3,1))	_clone 3 times, with same col size_
**Output**
array([[1, 2],
       [2, 3],
       [1, 2],
       [2, 3],
       [1, 2],
       [2, 3]])
       
->a = np.array([[1,2],[2,3]])
->np.tile(a,(3,2))
**Output**
array([[1, 2, 1, 2],	_clone 3 times, col is repeating 2 times_
       [2, 3, 2, 3],
       [1, 2, 1, 2],
       [2, 3, 2, 3],
       [1, 2, 1, 2],
       [2, 3, 2, 3]])
    
       
# np.repeat
n = 3
b = [1,2]

->np.repeat(n,3,axis=0)
**Output**
array([3,3,3])

->np.repeat(b,2,axis=0)
**Output**
array([1,1,2,2])
    
       
# np.hstack
a=[[1,2],[2,3]]
b=[[4,5],[7,8]]

->np.hstack((a,b))	_One tuple of arrays should be passed_
**Output**
array([[1, 2, 4, 5],
       [2, 3, 7, 8]])

       
# np.vstack
->np.vstack((a,b))
**Output**
array([[1, 2],
       [2, 3],
       [4, 5],
       [7, 8]])
 
       
# np.split
>>> a=np.array([[1,2,2,],[5,6,4]])
>>> a
array([[1, 2, 2],
       [5, 6, 4]])
>>> np.split(a, 3,axis=1)
[
array([[1],
	[5]]), 
array([[2],
	[6]]), 
array([[2],
	[4]])
]

       
       
       
       
       
