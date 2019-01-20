## ALgorithm Analysis Cheat Sheet: 

http://bigocheatsheet.com/



## List of Algorithms (in no Particular order)


Euclidean algorithm for GCD
   "[The Euclidean algorithm] is the granddaddy of all algorithms, because it is the oldest nontrivial algorithm that has survived to the present day."

Donald Knuth, The Art of Computer Programming, Vol. 2: Seminumerical Algorithms, 2nd edition (1981), p. 318.


### Classic CS

1. Strassen’s algorithm for Matrix multiplication
2. String Matching
3. Binary search
4. Merge Sort 
5. Fast Fourier transform (FFT)
6. Dynamic Programming
      common subsequence
7. Random number generation
8. Testing for Random Numbers
9. RSA Encryption Algo and the Diffie Hellman Key exchange
10. Regular Expressions and Parsing (LISP)
11. LZ Compression algorithms 
      https://en.wikipedia.org/wiki/Burrows%E2%80%93Wheeler_transform

### Classic AI

- Search (A*) 
   -- Traveling Salesman Problem
   -- Dijkstra’s algorithm 

- Game Tree Search(MINIMAX AND MCTS)
- SAT SOLVER
- MAXSAT Solver

- BackPropogation

### Data 

-  SVD: http://www.uwlax.edu/faculty/will/svd/index.html
- Principal Component Analysis (PCA)


--------------

#### Modern hashing. 

we’ll discuss how hash functions can be used to perform “lossy compression” through
data structures like bloom filters and count-min sketches. The goal is to compress a
data set while approximately preserving properties such as set membership or frequency
counts.

#### The nearest neighbor problem and dimension reduction. 

Dimension reduction continues the theme of lossy compression: it’s about compressing data while approximately
preserving similarity information (represented using distances). In the nearest neighbor problem, you are given a point set (e.g., representing documents) and want to preprocess it so that, given a query (e.g., representing a keyword search query), you can quickly determine which point is closest to the query. This problem offers our first
method of understanding and exploring a data set.

#### Generalization, regularization, and all that. 

The next topic is motivated by issues in
machine learning. You’re probably at least vaguely familiar with the idea of using
labeled training data to learn a prediction function. (E.g., from a collection of past
emails labeled as spam or not, to learn a classifier that predicts whether or not a
previously unseen email is spam.) The goal is to learn a prediction function that
“generalizes,” meaning one that is accurate on examples that have not been previously
seen (as opposed to being accurate merely on the training samples). In particular, one wants to avoid learning a prediction function that effectively memorizes the training
sample — this would be “overfitting” to the particular data at hand.
Intuitively, the more training data you have, the better your chance of learning a
prediction function that generalizes well. We’ll introduce you to a clean and useful
conceptual framework, rooted in statistical learning theory, for reasoning about these
issues. We’ll also cover useful techniques for avoid overfitting in the practically common
case where the amount of training data is relatively small. One such technique is
“regularization,” whereby you penalize “more complex” prediction functions in favor
of “simpler” ones. This is a version of Occam’s Razor, which advocates accepting the
simplest theory that explains the known observations.


#### Linear algebra and spectral techniques. 

One could also call this topic “the unreasonable effectiveness of
sophomore-level linear algebra.” This is a major topic, and it will
occupy us for three weeks. Many data sets are usefully interpreted as points in space
(and hence matrices, with the vectors forming the rows or the columns of a matrix).
For example, a document can be mapped to a vector of word frequencies. Graphs
(social networks, etc.) can also usefully be viewed as matrices in various ways. We’ll
see that linear algebraic methods are incredibly useful for exposing the “geometry”
of a data set, and this allows one to see patterns in the data that would be otherwise undetectable. 
Exhibit A is principle component analysis (PCA), which identifies
the “most meaningful” dimensions of a data set. We’ll also cover the singular value
decomposition (SVD), which identifies low-rank structure and is useful for denoising
data and recovering missing data. Finally, we’ll see how eigenvalues and eigenvectors
have shockingly meaningful interpretations in network data. Linear algebra is a muchmaligned topic in computer science circles, but hopefully the geometric intuition and
real-world applications we provide will bring the subject to life


#### Sampling and estimation. 

It’s often useful to view a data set as a sample from some
distribution or population. How many samples are necessary and sufficient before you
can make accurate inferences about the population? How can you estimate what you
don’t know? We’ll also study the Markov Chain Monte Carlo method, by which you
can estimate what you cannot compute.

Alternative bases and the Fourier perspective. This topic continues the theme of how
a shift in perspective can illuminate otherwise undetectable patterns in data. For
example, some data has a temporal component (like audio or time-series data). Other
data has locality (nearby pixels of an image are often similar, same for measurements
by sensors). A naive representation of such data might have one point per moment
in time or per point in space. It can be far more informative to transform the data
into a “dual” representation, which rephrases the data in terms of patterns that occur
across time or across space. This is the point of the Fourier transform and other
similar-in-spirit transforms.

#### Mathematical programming. 
Many optimization and data analysis problems can be solved using linear, 
integer, or convex programming. These days, there are powerful
solvers at your disposal that can be used to attack such problems. We’ll study the
representative application of compressive sensing, which allows you to recover a sparse
signal from amazingly few “linear measurements.”



### Data Structures that power Modern DB systems

1. Hash Table
2. Sorted String Table
3. B-Trees
4. Log-Structured Merge-Tree (LSM-Tree)

reference: http://shop.oreilly.com/product/0636920032175.do


### Interesting Links: 

https://www.quora.com/Can-you-describe-the-beauty-of-algorithms

https://www.coursera.org/specializations/algorithms

http://aima.cs.berkeley.edu/

https://github.com/norvig/pytudes

http://web.stanford.edu/class/cs168/index.html

https://medium.com/@codingfreak/top-algorithms-data-structures-concepts-every-computer-science-student-should-know-e0549c67b4ac

https://blog.codinghorror.com/classic-computer-science-puzzles/

https://www.quora.com/What-are-some-amazing-computer-science-algorithms

https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-0002-introduction-to-computational-thinking-and-data-science-fall-2016/index.htm



### Books: 
   - Artificial Intelligence: A Modern Approach
   - Introduction to information Retreival 
   - Designing data Intensive Applications
   - https://nlp.stanford.edu/manning/
   - Introduction to Computation and Programming Using Python: With Application to Understanding Data
   - https://composingprograms.com/
   - Decision Making Under Uncertainty (MIT Press)
   - Reinforcement Learning by Sutton And Barto
   - Intro to Statistical Learning
   - Algorithms for Optimization
   - Computer Age Statistical Inference: Algorithms, Evidence, and Data Science 
   - Data Science from Scratch
   - Linear Algebra and Learning from Data
   - Foundations of Data Science
   
   - Python Data Science Handbook
   - Data Science from scratch
   - Statistics for data scienstists


-----------

### Interesting Areas

- Computational Geometry
- Multi-threaded algorithms - Operating Systems
- Distributed Computing
- Distributed Process Mining
- Distributed ML
- Image Processing
- Graphics 
- Compilers 

