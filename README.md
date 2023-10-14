# Diagonalisation_of_quadratic_forms
This is an (unfinished) algorithm of diagonalization of quadratic form matrices.
Intented as an exercice larening about bilinear and quadratic forms in an algebra course.

The program can diagonalize simple matrices in 2D, 3D and more.
It is written for wxMaxima, the file is .mac format.

Backdraw and improvements to do :

The principal diagonaliser function is still to be implemented.
Things to work : 
1 - Matrix of type (head nul) or of type m5a, m5b, m5c (see below) still generates error, zeros shound be dispalced properly in order to diagonalize.
2 - An algorythm that automatically make the reordering (push zeros backwards).
3 - Step 0 is to be implmented, by step 0 we mean the case where all diagonals are zero and we make a variable change y1=x1+x2 ; y2=x1-x2.

Further steps :
Once done, write the same functions in python and for sagemath.
Two versions, one for matrices one for polynomials.

Things yet to study : Jordanian matrices, Eigen values, diagonalization using duals.

Note :
Tested matrices that generates errors :

m5a:matrix(
        [0, 0,  -2, -2,11],
        [0, -2, -4, -5,-7],
        [-2,    -4, 0,  1,0],
        [-2,    -5, 1,  9,13],
        [11,-7, 0 , 13, 23  ]
    );

m5b:matrix(
        [0,    0, 0,  -5, -7],
        [0,    0,  0, 1,  0],
        [0, 0, 0,  -2, 11],
        [-5,    1,  -2, 9,  13],
        [-7,    0,  11, 13, 23]
    );

m5c:matrix(
        [0,    8, 0,  -5, -7],
        [8,    -7,  0, 1,  0],
        [0, 0, 0,  -2, 11],
        [-5,    1,  -2, 9,  13],
        [-7,    0,  11, 13, 23]
    );
