java c
Tutorial EG501V Computational Fluid Dynamics (AY   2023/24) 
Tutorial 5. Building a system matrix 
Two-dimensional fluid flow   can be   described   by   means   of   a stream   function φ(x, y) that obeys the following   elliptic
PDE:  Consider the two-dimensional contraction as shown in the figure. The left panel   of   the   figure   is   a   cartoon   of   the   streamlines.
The right panel defines the flow geometry and boundary conditions:  at the inlet (left) and   at   the   outlet   (right); φ = 0    on   the   entire   lower   wall; φ = 1   on   the   upper   wall. The   figure   also defines the discretization. We use dimensionless quantities throughout this   problem.

Q1 
From   the   discretization   (with      Δx = 1   and   Δy = 0代 写EG501V Computational Fluid Dynamics (AY 2023/24) Tutorial 5R
代做程序编程语言.5   ) of   the   PDE, and   from   the   boundary conditions   determine   the   10×10 matrix   [A] and   the   10-dimensional   vector b such   that   the   10-dimensional   vector φ containing φk , k =   1…10    satisfies      [A]φ = b . Number   the   unknowns φk as indicated in   the   figure.
Q2 
The fluid velocity in x andy-direction ( ux and uy ) is related to the stream function   according to  and  The solution to  =   [0.2322   , 0.2049   ,   0.4781   ,   0.4542   ,
0.3513 , 0.3389 , 0.7359   ,   0.7233   ,   0.6800   ,   0.6716].   Given   this   solution,   determine ux in   points 3 and   6, and   determine uy in   points   2 and   5   based   on   central   differences   approximations.





         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
