java c
EG501V Computational Fluid Dynamics 
SESSION 2016-17 
00 December 2016
Problem 1 (a: 2 marks; b: 15 marks; c: 8 marks; total 25 marks) 
We use dimensionless quantities throughout this problem. 

Figure. Left: flow geometry and streamlines; right: discretization and numbering of unknowns. 
Consider the two-dimensional flow in a sharp 90o   bend   as   sketched   in the   left panel   of   the   figure.   This   flow   can   be   described   by   means   of   a   stream   function φ(x, y) that   obeys   the   following   PDE:  The   right   panel   of   the   figure   defines   the   flow   geometry   and   boundary   conditions:  = 0   at the inlet (bottom);  = 0    at the outlet (right) ; φ = 0    on the right and   lower wall; φ = 1 on   the   left   and   upper   wall. The   figure   also   defines   the   discretization, with   spacing   Δ =   1   . We realize that the problem is symmetric with respect to the dashed line   in the   left panel.   This   implies   that we only need to solve φ in the numbered points in the right panel of   the figure.
a.       What   type   of   PDE   (parabolic, elliptic, hyperbolic)   are   we   dealing   with?
b.       From   a   discretization   of   the   PDE, and   from   the   boundary   conditions   determine   the   9×9
matrix   [A] and   the   9-dimensional   vector b such   that   the   9-dimensional   vector φ 
containing φk , k = 1…9   satisfies   [A]φ = b . Number   the   unknowns φk as   indicated   in   the figure.
c.       The   fluid   velocity   in x andy-direction   ( ux and uy ) is   related   to   the   stream   function φ 
according to ux =  and uy = −  .       The   solution to [ A b ]φ = b is φ
=   [0.6266, 0.4347, 0.3737, 0.3594, 0.9093, 0.8186, 0.7385, 0.7006, 0.6901].   Given   this   solution,   determine ux and uy in   points   1, 3, 4, and   5 based   on central differences   approximations.
Problem 2 (a: 7 marks; b: 9 marks; c: 9 marks; total: 25 marks) 


Figure. Catalytic layer  discretization 
In steady state, the concentration c of   a chemical species that is being   consumed   in   a   layer (thickness d) of   solid catalytic material can be described by the following reaction-diffusion
equation:  with   Γ   the   diffusion   coefficient, and k the   reaction   rate   constant. At   the
left   side   of   the   layer   (at x=0) the   concentration c is   maintained   at c0, at   the   right   side   (at x=d) at c=0. In   dimensionless   form   the   parameters   of   this   problem   are: d=4,    Γ =   1   , k=1, and c0      = 1   .
In   order   to   solve   for c as   a   function   of x, c is   discretized   to ci , i =   1…3   , with   a   constant   spacing Δx = 1   between   the   points, see   the   figure.
a.       First discretize the differential   equation: write   it   as   a   linear   algebraic   equation   in代 写EG501V Computational Fluid Dynamics 2016-17SQL
代做程序编程语言 terms   of
ci . Then   set   up   a   linear   system   of   equations   in   matrix-vector   form      [A]   c(→) =   b(→) with      c(→) the
vector   containing   the   three   unknown   concentrations ci ,   [A]a 3x3 matrix, and b a   three-
dimensional   vector. Determine   [A] and b .
The   rest   of   this   question   is   about   solving      [A]   c(→) = b . If   you   do   not   have   an   answer   under   Question a.,   assume  and  (these [A] and b are not the correct answer for a.).b.       Solve   the   system      [A]   c(→) = b by   means   of   Gaussian   elimination;   show   all   the   steps   that   lead to your   solution.c.       Perform. two (2)   Gauss-Seidel iterations on   the   system [A] c = b. Take  as the
starting vector of   the iteration process.
Problem 3 (a: 5 marks; b: 5 marks; c: 15 marks; total: 25 marks) 
We   are   dealing   with   a   turbulent   flow   in   which   the   chemical   reaction A + B → P takes   place. The reaction is of   second order which means that the number of   moles of   product P being produced            per   unit   volume   and   per   unit   time   (symbol rP, unit   [mol/(m3.s)]) is rP = kPcAcB with cA and cB the   concentration   [mol/m3] of   species A and B respectively, and kP the   reaction   rate   constant
[m3/(mol.s)]. We   assume   all   species   have   the   same   diffusion   coefficient      Γ    [m2/s].
a.       For a non-reacting system, the transport equations   for   chemical   species A and B read
respectively. Argue   that   for   the reacting system   these   equations   become  and

b.       What   is   the   transport   equation   for   the   concentration cP [mol/m3] of   chemical   species P?
c.       Derive through a Reynolds decomposition   of   the   equation
an   equation   for   the   time-average   concentration c .
Assume a two dimensional situation. Identify the terms in the   equation that   need   closure.
Problem 4 (25 marks) 
We use dimensionless quantities throughout this problem. 
The discrete version of   the pressure-correction equation reads:

Given the 3x3 mesh of   control volumes as in the figure,   given   the boundary   conditions   for
pressure   correction π which   is      ∂π∂n =   0   on   all   four   boundaries, and   the   preliminary   velocity
values ux(*)    and uy(*)    as   given   in   the   figure,   determine   the   matrix-vector   system      [A =   b(→) that
needs to be solved   in   order to      in the same order as the pressure points numbered in the   figure).
Further given: hx =   1, hy =   0.5, ρ △t =   1   .

Figure. Staggered mesh. Pressure defined in the centre of each control volume (dots); velocity at the vertices of each control volume (arrows). All values given are velocity values. 





         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
