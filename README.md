# Density profile of Vector Fuzzy-Dark matter
( This work was done in collaboration with Ashish Narang, a post-doctoral student at PRL, Ahmedabad and under the mentorship of Prof. Subhendra Mohanty)


**Introduction**:  \
Aside from the usual matter(made up proton, neutron and electron) with which we interact everyday, physicists have long believed the existence of another type of invisible matter that surrounds most galaxies in the Universe, including our own Milky-way galaxy. Unlike the everyday matter around us, this unseen matter is not known to have any direct contact with the former, hence aptly named "dark matter"; although its amount is argued to be almost five times that of standard matter. Over the past several decades, following extensive and meticulous study of different cosmological phenomenon and observational data, majority of the scientific community today strongly argues the existence of dark matter, and is a topic of active research. One of the most fundamental question regarding dark matter that remains unanswered today is, what is it made up of?\
Several models and ideas have been proposed in this regard, and among them the most commonly accepted idea is that of Cold Dark Matter or CDM model. It elegantly explains several issues on the subject and enjoys great success, except at the region close to the center of galaxies, where a very massive Black Hole is known to exist. The key issue is that the theoretical prediction on the density profile in this region diverges to a huge value towards the galactic center, and is in conflict with observational data that the density actually flattens out or becomes 
constant at the center. This is widely known as the "Core-Cusp" problem in cosmology. One of the possible resolution to this tension comes through a relatively new idea of dark matter. They key difference in this idea is that the constituent particles of dark matter is considered to be extremely tiny(ultra-light) such that the fundamental description of suh a system can be given by the extremely powerful Schrodinger-Posisson(SP) equation.



![](https://latex.codecogs.com/png.image?\dpi{110}%20%20-\frac{\nabla^2}{2m}\psi(r)%20+%20m(\Phi%20+V)\psi(r)%20=%20E\psi(r)) 


  ![](https://latex.codecogs.com/png.image?\dpi{110}%20%20\nabla^2%20\Phi=%204\pi%20G%20|\psi|^2)

  The three main qunatities in above are :
  
  ![](https://latex.codecogs.com/png.image?\dpi{110}%20\psi(r)) denotes the dark matter which entails the fundamental description including the density
  
  ![](https://latex.codecogs.com/png.image?\dpi{110}%20\Phi(r)) efines the gravitational interaction with itself 
  
  ![](https://latex.codecogs.com/png.image?\dpi{110}%20V(r)) is the black hole potential.
  
The scalar type of such dark matter is already studied extensively, hence, in this project we aim to study a variant called vector fuzzy dark matter, which also obeys the SP eqn. 

**Goal** :\
Thus, the initial obejctive of this project was to numerically solve the Schrodinger-Poisson equation with relevant boundary condition and study the affect of varying Black Hole mass on the density profile of fuzzy VDM.

**Methodology**:\
1.The Schrodinger-Poisson equation is a set of two coupled, second order partial differential equation  which is best solved numerically using the "shooting-method".\
2. Considering the appropriate physical description, we would want to solve the equations with a specific set of four boundary conditions. The first three are\

![I)](https://latex.codecogs.com/png.image?\dpi{110}%20\psi(r=0)%20=%200), ![II)](https://latex.codecogs.com/png.image?\dpi{110}%20\psi(r=%20\infty)%20=%200), ![III](https://latex.codecogs.com/png.image?\dpi{110}%20\psi%27(r=%200)%20=%201)

For the potential function we would need the inital value, however, this cannot be randomly guessd apriori. So, we apply the following technique. \
3. First, we keep the value of   ![](https://latex.codecogs.com/png.image?\dpi{110}%20\Phi(r=0)%20=%20p)   as an unknown variable. Then we consider the solution of the SP eqn i.e $\psi(x)$ at the boundary, which ideally is supposed to be a very large number, say $\psi(x= some large distance)$. Thus, we now have an equation with undetermined parameter $p$ in terms of $\psi$ at the boundary value.\
4. A very simple e.g to exemplify the above is, say the eqn of interest is $x^2 + x +c+d$. At $x=2$, the eqn becomes $6+c+d$. So,we now call this as a function $f(p)$. \
5. The key idea now is that, we know that at a very large distance we want $\psi(s) = 0$, by virtue of physical limits. This essentially means that we want to find a value of $p$ such that the eqn evaluates to zero, in other words, we want to fnd the root of the equation. This is commonly called as root-finding technique. \
6. Thus, the final task is to plot the function $f(p)$ within a range and find the values of $p$ at which the funtion is zero. This value of p once determined can be directly used in solving the full Schrodinger-Poisson eqn exactly.
