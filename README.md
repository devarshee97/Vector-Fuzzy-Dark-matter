# Density profile of Vector Fuzzy-Dark matter


**Introduction**:  \
Aside from the usual matter(made up proton, neutron and electron) with which we interact everyday, physicists have long believed the existence of another type of invisible matter that engulfs most galaxies in the Universe, including our own Milky-way galaxy. Unlike the everyday matter around us, this unseen matter is not known to have any direct contact with the former, hence aptly named "dark matter"; but its amount is argued to be almost five times the usual matter. Over the past several decades, following extensive and meticulous study of different cosmological phenomenon and observational data, majority of the scientific community strongly argues for the existence of dark matter, and thus is a topic of active research. One of the most fundamental question regarding dark matter that remains unanswered today is, what is it made up of? Several models and ideas have been proposed in this regard, and among them the most commonly accepted idea is that of Cold Dark Matter or CDM model. It elegantly explains several issues on the subject and enjoys great success, except at the region close to the center of galaxies, where a very massive Black Hole is known to exist. The key issue is that the theoretical prediction on the density profile in this region diverges to a huge value towards the galactic center, is in conflict with observational data that the density actually flattejs outor becomes 
constant at the center. This is widely known as the "Core-Cusp" problem in cosmology. One of the possible resolution to this tension comes through a relatively new idea o dar matter called scalar field dark matter. They key difference in th e latter is that the cinstituent particles of dark matter is considered to be extremely tiny(ultra-light) such that the fundamental description of suh a system can be given by the extremely powerful Schrodinger-Posisson(SP) equation. \

![](https://latex.codecogs.com/png.image?\dpi{110}%20%20-\frac{\nabla^2}{2m}\psi(r)%20+%20m(\Phi%20+V)\psi(r)%20=%20E\psi(r)) \
  ![](https://latex.codecogs.com/png.image?\dpi{110}%20%20\nabla^2%20\Phi=%204\pi%20G%20|\psi|^2)

The scalar type of such dark matter is already studied extensively, hence, in this project we aim to study a variant called vector fuzzy dark matter, which also obeys the SP eqn. \

**Goal** :\
Thus, the initial obejctive of this file is to numerically solve the SP eqn with relvant boundary condition and study the affect of varying Black Hole mass on the density profile of fuzzy VDM. This work was done in collaboration with Ashish Narang, post-doctoral student at PRL, Ahmedabad and under the mentorship of Prof. Subhendra Mohanty.

**Methodology**:\
1.The Schrodinger-Poisson equation(explicitly shown in respective files) is a set of two coupled, second order partial differential equation with two free parameters, which is best solved numerically. The approach we take is commonly known as shooting method method.\
2. The two dependent variables in the equation are $\phi(x)$ and $V(x)$, where the former denotes the wavefunction describing the dark matter behaviour and latte denoting its gravitational potential with itself.\
3. Considering the appropriate physical description, we would want to solve the equations with a specific set of boundary conditions(we need four). This includes 
$\psi(x=0) = 0, \psi(x=infinity)= 0, \psi'(x=0)=1$. For the potential function we would need the inital value, however, this cannot be randomly guessd apriori. So, we employ apply the following technique. \
4. First, we keep the value of $V(x=0) = p$ as an unknown variable. Then we consider the solution of the SP eqn i.e $\psi(x)$ at the boundary, which ideally is supposed to be a very large number, say $\psi(x= some large distance)$. Thus, we now have an equation with undetermined parameter $p$ in terms of $\psi$ at the boundary value.\
5. A very simple e.g to exemplify the above is, say the eqn of interest is $x^2 + x +c+d$. At $x=2$, the eqn becomes $6+c+d$. So,we now call this as a function $f(p)$. \
6. The key idea now is that, we know that at a very large distance we want $\psi(s) = 0$, by virtue of physical limits. This essentially means that we want to find a value of $p$ such that the eqn evaluates to zero, in other words, we want to fnd the root of the equation. This is commonly called as root-finding technique. \
7. Thus, the final task is to plot the function $f(p)$ within a range and find the values of $p$ at which the funtion is zero. This value of p once determined can be directly used in solving the full Schrodinger-Poisson eqn exactly.
