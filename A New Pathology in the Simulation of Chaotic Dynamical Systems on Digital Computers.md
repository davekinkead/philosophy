---
bibtex: @article{boghosian2019new,
  title={A new pathology in the simulation of chaotic dynamical systems on digital computers},
  author={Boghosian, Bruce M and Coveney, Peter V and Wang, Hongyan},
  journal={Advanced Theory and Simulations},
  volume={2},
  number={12},
  pages={1900125},
  year={2019},
  publisher={Wiley Online Library}
}
---

# A New Pathology in the Simulation of Chaotic Dynamical Systems on Digital Computers

> Systematic distortions are uncovered in the statistical properties of chaotic dynamical systems when represented and simulated on digital computers using standard IEEE floating-point numbers. This is done by studying a model chaotic dynamical system with a single free parameter β, known as the generalized Bernoulli map, many of whose exact properties are known. Much of the structure of the dynamical system is lost in the floating-point representation. For even integer values of the parameter, the long time behaviour is completely wrong, subsuming the known anomalous behaviour for β = 2. For non-integer β, relative errors in observables can reach 14%. For odd integer values of β, floating-point results are more accurate, but still produce relative errors two orders of magnitude larger than those attributable to roundoff. The analysis indicates that the pathology described, which cannot be mitigated by increasing the precision of the floating point numbers, is a representative example of a deeper problem in the computation of expectation values for chaotic systems. The findings sound a warning about the uncritical application of numerical methods in studies of the statistical properties of chaotic dynamical systems, such as are routinely performed throughout computational science, including turbulence and molecular dynamics.

By comparing a simulation of a simple chaotic system with known outcomes, systematic distortions with the use of floating point numbers where found indicating a new pathology in discrete computation.

> Extreme sensitivity to initial conditions is a defining feature of chaotic dynamical systems. Since the first usage of digital computers for computational science, it has been known that loss of precision due to the discrete approximation of real numbers can dramatically alter the dy- namics of chaotic systems after a short amount of simulation time. (p1)

Depsite this, researchers believe that averages of multiple numberic simulations still provide robust approximations of analytic solutions.

> Here, we demonstrate that, for at least one simple-but-prototypical driven, dissipative dynamical system, namely the generalized Bernoulli Map, the abovementioned hopes are dashed. While it has long been known that individual orbits of this map are chaotic in nature, and that even statistical averages are problematic. (p2)

These errors are not typical FPN errors.

> Unlike other sources of error associated with floating-point numbers, such as loss-of-significance errors, noise in function evaluation, and underflow and overflow,10 the problem we describe in this work is due to the discrete and finite nature of the floating-point numbers and the extremely delicate structure of the attracting set of chaotic dynamical systems. (p2)

> it is entirely possible that many published results of numerical simulation are substantially inaccurate for this reason (p2)

3 distinct effects are observed :

1. observable expectation values that are nearly correct  
2. observable expectation values that are obviously wrong  
3. observable expectation values that are wrong, but not obviously so

> we have demonstrated a serious systematic error in the numerical calculation of the statistical properties of a very representative chaotic nonlinear dynamical system. 

> It arises from the discreteness of floating-point numbers, their non-uniform distribution along the real axis, and their inability to represent points on periodic orbits of the dynamics in a precise way, giving rise to a dramatically truncated periodic orbit spectrum. It cannot be mitigated by the use of fixed-point arithmetic or other recently proposed adjustments to the floating-point system of representation22, 23 owing to the discrete nature of any finite-state digital computer. 

