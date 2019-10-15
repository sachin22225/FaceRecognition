"# Face_Recognition" 
"# Face_Recognition" 
"# Face_Recognition" 
"# Face_Recognition" 

Triplet Loss


For an image  x , we denote its encoding  f(x) , where  f(x)  is the function computed by the neural network.
Training will use triplets of images  (A,P,N) :

A is an "Anchor" image--a picture of a person.
P is a "Positive" image--a picture of the same person as the Anchor image.
N is a "Negative" image--a picture of a different person than the Anchor image.
These triplets are picked from our training dataset. We will write  (A(i),P(i),N(i))  to denote the  i -th training example.

we'd like to make sure that an image  A(i)  of an individual is closer to the Positive  P(i)P(i)  than to the Negative image  N(i) by at least a margin a :
||f(A(i))-f(P(i))||^2+a<||f(A(i))-f(N(i))||^2

we would thus like to minimize the following "triplet cost":
j=sum for all traning example(||f(A(i))-f(P(i))||^2-||f(A(i))-f(N(i))||^2+a)
The model accuracy is 95.6%
Installation
1.Clone this repository
2.install mention dependency
Tensorflow>=1.5.0
Keras>=2.2.4
Python=3.6
opencv>=4.0.0
Matplotlib>=3.0.2
Numpy>=1.15.4

Execution
The Face_Recognition.ipynb have a code.Use jupyter Notebook to run the code


