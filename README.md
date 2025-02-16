java c
Tutorial EG501V Computational Fluid Dynamics (AY   2023/24) 
Tutorial 3. Discretization: start-up flow in a thin fluid layer
In Lecture Notes 2  Tutorial 2 we derived   a parabolic PDE for the flow between two parallel plates. Initially both   plates and the fluid between them are at rest.    At   time   equal   zero the upper plate starts moving with a constant velocity u0   , see the figure. The PDE reads  (Eq. 2.2 in Lecture Notes 2) with ux the   flow velocity   in x-direction   that   depends   on   they-location   and   time t; ν = μρ is   the   kinematic viscosity of   the fluid and is   a   constant.
In Lecture Notes 3 it was   shown how to discretize a parabolic PDE   (there in   temperature T)   and to eventually come up with an update rule (Eq. 3.5) that   descr代 写EG501V Computational Fluid Dynamics (AY 2023/24) Tutorial 3R
代做程序编程语言ibes how to   determine   the   situation at a new time instant (j+1) if   the situation   at   the   old   time   instant   (j)   is   known. 

Your assignment 
(1) Follow the same procedure as in Lecture Notes 3 to   derive   an   update rule   for the velocity ux at   time   instant j+1 ( ux ,i ,j+1       where   the   index i stands   for   they-location   in   the   fluid   film).
(2) Consider the specific situation where L=5 mm, u0   =1 m/s, and ν =10-6   m2/s. Discretize y such   that   △y =1 mm   (i.e. divide   the   distance L in   five   equal   portions) and   take   time   steps   of    △t =0.1 s. Determine the velocity in the fluid layer after one   and two time   steps   (i.e.   at t=0.1   s and t=0.2   s).



         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
