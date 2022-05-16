# Managing Risk in Option Portfolios: the Karhunen-Loeve Decomposition in Modelling Dynamics of Implied Volatilities

The project aims to model dynamics of implied volatilities of option prices in order for individuals to manage risk in option portfolios. The implied volatility σBS(K,T)  of a call option with strike level K and maturity date T actually depends on K  and T, which represents this dependencies the implied volatility surface at date t. Financial researchers are attracted to this surface because of the insufficiency of the Black–Scholes model and alteration the level of implied volatilities by time. In fact, the evolution in time of this surface captures the evolution of prices in the options market.
The previous models try to give an explanation the various empirical deviations by adding a local volatility function, a stochastic diffusion coefficient, jump intensities, jump amplitudes etc. However, it is not feasible to compute directly the shape of the implied volatility surface by introducing parameters, in the most of these models. For instance, a model may assess closely the strike profile and term structure of options on a given day, but the same model parameters might not do well at the next date. Risk management applications are resulted from this time instability of model parameters. The inability is due to increasing in autonomy of market and due to prices driven by internal supply and demand in the options market not to mention by the underlying assets.
It is essential to identify these extra sources of randomness, that is the salient dynamic properties of option prices, which are particular to the options market and their dynamics in the model. By doing so, instability of model parameters will be resolved.  

To this end, a stationary random field are applied to the analysis of the dynamics of all implied volatility surfaces with the Karhunen-Loeve decomposition. In this respect, the following homogenous Fredholm integral equation of the second kind should be solved:

![\Large \int(K(x,y)f_n(y)dy)=v_n^2*f_n(x) ](https://latex.codecogs.com/svg.latex?\Large&space;\int(K(x,y)f_n(y)dy)=v_n^2*f_n(x))

when (fn,vn) is an eigenpair of the associated integral operator and K(x,y) , Kernel function, is the covariance coefficient between two points on the implied volatility surface.

References:

[1] Cont, R., da Fonseca, J., Dynamics of implied volatility surfaces, Quantitative Finance, 2, 2002, 45-60.
[2] F. Guillaume, W. Schoutens, Calibration risk: Illustrating the impact of calibration risk under the Heston model, Rev. Deriv.
Res. (2012) 15:57 - 79.

Codes are provided to solve: 1) Fredholm integral equations second kind and 2) Homogenous Fredholm integral equation second kind by Quadrature method.
