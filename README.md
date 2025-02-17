java c
EG501V Computational Fluid Dynamics 
SESSION 2017-18
00 December 2017
Problem 1 [40 marks] 
We use dimensionless quantities throughout this problem. 

Figure. Left: solution domain and boundary conditions; right: discretization and numbering of unknowns. 
We want to numerically solve a steady convection-diffusion equation in the   variable φ in   a two-   dimensional   square   domain   with   side   length L=1. The   equation   reads      ▽.(φu)   =   Γ▽2φ . The velocity   vector u is   constant   in   the   entire   domain   and   has   components ux =   1, uy =   1   ; the diffusion   coefficient   Γ   =1   . The   boundary   conditions   are φ = 0    on   the   west   boundary, φ = 1   on the   south   boundary,    ∂φ∂x = 0   on   the   east   boundary,   ∂φ ∂y =   0    on   the   north   boundary;   see   the left panel of   the figure. The square domain is   discretized   according to the   right panel   of   the figure. The dots are   equally   spaced.
a.       Give   the   discrete   equations   for   points   1,   3,   and   9 based   on   finite difference discretization with   a central scheme   for   the   convective   term. [16 marks] 
b.       Give   the   discrete   equations   for   points   1, 3,   and   9 based   on   finite volume discretization          with an upwind scheme for the convective term and the volume   centres   coinciding   with   the   numbered   dots. [16 marks] 
A   control   volume   based   Peclet   number   can   be   defined   as  the   spacing between points.c.       Determine      Pecv and   decide   if   you   want   to   apply   the central or upwind scheme. [8 marks]
Problem 2 [20 marks] 
We use dimensionless quantities throughout this problem. 


Figure: flow geometry, boundary conditions and discretization. 
Two-dimensional   fluid   flow   can   be   described   by   means   of   a   stream   function φ(x, y) that   obeys
the following elliptic PDE:  =   0 .    Consider the two-dimensional geometry as   shown in
the   figure. It   defines   the   flow   geometry   and   boundary   conditions:  = 0   at   the   inlet   (left)   and   at
the   outlet   (right); φ = 0    on   the   lower   wall; φ = 1   on   the   entire   upper   wall. The   figure   also   defines the discretization.
a.       From   the   discretization   (with      Δx = 1   and      Δy = 0.5   ) of   the   PDE, and   from   the   boundary
conditions   determine   the   10×10 matrix   [A] and   the   10-dimensional   vector b such   that   the
10-dimensional   vector φ containing φk , k =   1…10    satisfies      [A]φ = b . Number   the unknowns φk as   indicated   in   the   figure. [12 marks] 
b.       The   fluid   velocity   in x andy-direction   ( ux and uy ) is   related   to   the   stream   function ac代 写EG501V Computational Fluid Dynamics 2017-18C/C++
代做程序编程语言cording to ux =  and uy = −  .       The   solution to [A] φ = b is φ   =   [0.3284   , 0.3200   ,
0.2767   , 0.2641   , 0.6611   , 0.6487   , 0.5458 ,   0.5219   ,   0.7951   ,   0.7678].   Given   this   solution,   determine ux in   points   1, 5 and   8, and   determine uy in   points   6 and   9   based   on   central
differences approximations. Is the overall flow from   left   to   right   (in positive x-direction)
or   from   right   to   left   (in   negative x-direction)? [8 marks]
Problem 3 [20 marks] 
Water   (density ρ = 1000 kg/m3   ; dynamic   viscosity μ =   0.001   Pa.s) flows   steadily   through   a       horizontal, straight   pipe   with   circular   cross   section   of   diameter D=0.2 m.   The   volumetric   flow rate   is φv =   0.01 m3/s.
a.       Argue   that   this   is   turbulent   flow. [4 marks] 
Pressure drop in the pipe is due to friction.   The pressure   drop per unit   length   can be written   as  with U the   average   velocity   in   the   pipe   and f the   friction   factor.   Given   the   pipe wall   roughness f can   be   considered   a   constant: f =   0.015 .
b.       What   is   the   average   energy   dissipation   rate   (symbol ε ) in   the   pipe? [4 marks] 
c.       Argue   − based   on   a   dimensional   analysis      − that   the   expression   for   the   Kolmogorov   length scale   (the   micro   scale   of   turbulence) reads      l K =   (ν 3ε)14       with ν = μρ the   kinematic viscosity. Determine   lK based on the average dissipation rate in the pipe. [6 marks] 
The shear stress at the inner pipe surface   follows   from   a   force balance   in   the   streamwise   direction over   the   liquid   in   the pipe:  The   wall   shear   velocity u*    relates   to   the   wall   shear
stress:  We   want   to   simulate   the   flow   in   the   pipe   with   help   of   standard   wall
functions. For this the distance of   the first grid point next to the   inner pipe wall   needs   to   satisfy   the   condition   30 < y+    <100 .
d.       Given this condition, what is the allowed range of   distances   of   the   first   grid   point   from   the   inner   pipe   wall? [6 marks] 
Problem 4 (20 marks) 
Consider the linear system  a.       Solve   the   system      [A]   x(→) = b by   means   of   Gaussian   elimination;   show   all   the   steps   that   lead to   your   solution. [10 marks] b.       Perform. two (2) Gauss-Seidel   iterations   on the   system    [A]   x(→) =   b(→) . Take  as the    starting vector of the iteration process. For each of the two Gauss-Seidel iterations determine   the   normalized   residual  with   (n)   =   b(→) −[A](n)    and ||    ||   indicating the   length   (norm) of   the   vector. [10 marks] 



         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
