# Matrix-Multiplication-using-Message-Passing-Interface-MPI


# In this project, I had implemented Matrix Multiplication parallel algorithm using the Message-Passing Interface (MPI)

# Assumptions: 

• The matrices are square matrices.
• The number of rows of the matrix A should be equal to number of columns of matrix B.
• The size of matrix should be divisible by number of processors.
• The size of matrix should be divisible by the grid of bocks.
• Number of executable processors should be either 1 , 2 , 4, or 8.

# Procedure: 

In order to carry execution process for matrix multiplication, We have used a block-wise distribution of data with master and slave pattern.
Work is divided by the checkerboard implementation, where the matrix C which is the resultant matrix is divided into n submatrices. Here n is equal to the number of processors participating in executing the program. Each sub matrix is assigned to each node for calculation. Each nodes get their own computation values from the master. After calculation the slave nodes send their results to master node and the final resultant matrix is printed.
