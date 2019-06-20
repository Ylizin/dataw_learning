# AX=b

if we want to represent a line, we need a formular:  
$l= \vec{b}+t*\overrightarrow{dir}$  
here $\overrightarrow{dir}$ is the direction of the line, like $[2,2]^T$

so the $\vec{b}$ determines where the line intersect with the axies.  

the next point is, to represent a plane, we need:  
$P=\vec{b}+\alpha*\overrightarrow{x_1}+\beta*\overrightarrow{x_2}$ where $\vec{x_1}$ and $\vec{x_2}$ is the basis of the plane and the $\vec{b}$ can repersent a point on the plane, it will tell us how far the plane is from the base point.

here we can go further to understand what is happening when solving a equation of $AX=b$, so after the elimination, if the equation has two plane intersect, the result is a line which may biased from the base point. if the $b$ is $0$ the line go through the base point. if not, the bias between the line and the base point depends on the $b$ after elimination.

as well as a plane if we have to solve it.

what we need to do is:  
1. find out the result of $Ax=0$
2. find out a point on the plane/line of the result $Ax=b$
3. get the line/plane by the formula we discussed above
   
also we can find out why the normal vector of $Ax+By+Cz=D$ is $[A,B,C]$:  
for a plane, the normal vector has nothing to do with the bias $\vec{b}$ since it's just a description of have far this plane is biased from the raw one which go through the base point.
so for a plane $p=\alpha*\overrightarrow{x_1}+\beta*\overrightarrow{x_2}$  ***remember $\vec{x_1}$ and $\vec{x_2}$ is the basis of the plane***  
we have the equations below:  
for each point in the plane:$[\alpha*x_1+\beta*x_2,\cdots]$
and the normal vector:$[v_1,v_2,v_3]$ must be orthogonal with any vector $\overrightarrow{0,p}$, so we have:  
$v_1*(\alpha*x_1+\beta*x_2)+\cdots=0\Rightarrow$  here the $(\alpha*x_1+\beta*x_2)$ is equals to the $x$ in the euqation $A*x+B*y+C*z=0$, for any $(x,y,z)$ in the plane it holds, so the $v_1$ must be equal to $A$ as well as $v_2,v_3$
