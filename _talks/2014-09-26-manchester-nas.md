---
title: Computational Tools for PDEs with Random Coefficients
speaker: Elisabeth Ullmann
speaker-url: http://people.bath.ac.uk/eu204/
affil: University of Hamburg
date: 2014-09-26 15:00:00
talk-url: http://www.maths.manchester.ac.uk/our-research/events/seminars/numerical-analysis-and-scientific-computing/computational-tools-for-pdes-with-random-coefficients.htm
series: manchester-nas
---

The simulation and forecast of complex physical processes in science,
engineering and industry requires input data which are often subject to
considerable uncertainties. This is due to incomplete models, measurement
errors or lack of knowledge. Partial differential equations (PDEs) with random
coefficients offer the opportunity to incorporate data uncertainties in
mathematical models and subsequent computer simulations. However, these PDEs
are formulated in a physical domain coupled with a possibly high-dimensional
sample space generated by random parameters and can be very
computing-intensive.

We outline the key computational challenges by discussing a model elliptic PDE
of single phase subsurface flow in a random porous medium. Suggested by
real-world data the diffusion coefficient is modeled as a lognormal random
field with rough realisations. Hence a large number of random parameters is
required. To date, only Monte Carlo based methods are computationally feasible
in this case, however the cost of Monte Carlo is often prohibitively large. We
employ multilevel Monte Carlo (MLMC), a novel variance reduction technique
which can reduce the cost significantly. We explain the basic MLMC idea and
combine this technique with mixed finite element discretisations to calculate
travel times of particles in groundwater flows (Graham et al., preprint).

For coefficients which can be parameterised by a small number of random
variables we employ spectral stochastic Galerkin (SG). A standard SG
discretisation of lognormal diffusion problems gives a block-dense Galerkin
matrix with sparse blocks. This precludes the development of iterative solvers
with optimal complexity from the outset. An alternative problem formulation as
convection-diffusion-type problem with random convective velocity has been
studied in (Ullmann et al., 2012). We discuss possible mixed formulations of
this problem. The saddle point Galerkin matrices are sparse, but have
nonsymmetric off-diagonal blocks. We suggest block-diagonal and
block-triangular preconditioners for use with GMRES and report on the
efficiency of the preconditioners.


## References

1. I.G. Graham, R. Scheichl, and E. Ullmann. Mixed Finite Element Analysis of Lognormal Diffusion and Multilevel Monte Carlo Methods. Available from arXiv:1312.6047
2. E. Ullmann, H.C. Elman, and O. G. Ernst. Efficient iterative solvers for stochastic Galerkin discretizations of log-transformed random diffusion problems. SIAM J. Sci. Comput., 34:A659-A682, 2012.
 
