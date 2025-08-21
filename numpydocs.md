# np.diff
a=[x1,x2], np.diff(a) => x2-x1 <br/>
a=[x1,x2,x3], np.diff(a) => [x2-x1, x3-x2]


# np.concatenate
a = np.array([[1, 2], [3, 4]]) <br/>
b = np.array([[5, 6]]) <br/>

_np.concatenate((a, b), axis=0)_ <br/>
**Output** <br/>
array([[1, 2], <br/>
       [3, 4], <br/>
       [5, 6]]) <br/>

_np.concatenate((a, b.T), axis=1)_ <br/>
**Output**
array([[1, 2, 5], <br/>
       [3, 4, 6]])

_np.concatenate((a, b), axis=None)_ <br/>
**Output** <br/>
array([1, 2, 3, 4, 5, 6]) <br/>


# np.tile
_Clone an array n times_

->a = np.array([[1,2],[2,3]])  <br/>
->np.tile(a,(3,1))	_clone 3 times, with same col size_  <br/>
**Output**  <br/>
array([[1, 2],  <br/>
       [2, 3],  <br/>
       [1, 2],  <br/>
       [2, 3],  <br/>
       [1, 2],  <br/>
       [2, 3]])  <br/>
       
->a = np.array([[1,2],[2,3]])  <br/>
->np.tile(a,(3,2))  <br/>
**Output**  <br/>
array([[1, 2, 1, 2],	_clone 3 times, col is repeating 2 times_  <br/>
       [2, 3, 2, 3],  <br/>
       [1, 2, 1, 2],  <br/>
       [2, 3, 2, 3],  <br/>
       [1, 2, 1, 2],  <br/>
       [2, 3, 2, 3]])  <br/>
    
       
# np.repeat
n = 3  <br/>
b = [1,2]  <br/>

->np.repeat(n,3,axis=0)  <br/>
**Output**  <br/>
array([3,3,3])  <br/>

->np.repeat(b,2,axis=0)  <br/>
**Output**  <br/>
array([1,1,2,2])  <br/>
    
       
# np.hstack
a=[[1,2],[2,3]]  <br/>
b=[[4,5],[7,8]]  <br/>

->np.hstack((a,b))	_One tuple of arrays should be passed_  <br/>
**Output**  <br/>
array([[1, 2, 4, 5],  <br/>
       [2, 3, 7, 8]])  <br/>

       
# np.vstack
->np.vstack((a,b))  <br/>
**Output**  <br/>
array([[1, 2],  <br/>
       [2, 3],  <br/>
       [4, 5],  <br/>
       [7, 8]])  <br/>
 
       
# np.split
>>> a=np.array([[1,2,2,],[5,6,4]])  <br/>
>>> a  <br/>
array([[1, 2, 2],  <br/>
       [5, 6, 4]])  <br/>
>>> np.split(a, 3,axis=1)  <br/>
[  <br/>
array([[1],  <br/>
	[5]]),   <br/>
array([[2],  <br/>
	[6]]),   <br/>
array([[2],  <br/>
	[4]])  <br/>
]

       
       
       
       
       
