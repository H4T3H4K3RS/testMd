

## Solution
The PDE for the replication price of a contingent claim of the form $X=g(ST)$ is the Black-Scholes equation:

$$\frac{\partial V}{\partial t}+\frac{\sigma^2S^2}{2}\frac{\partial^2V}{\partial S^2}+\mu S\frac{\partial V}{\partial S}-rV=0$$

where $V(t,S)$ is the value of the claim at time $t$ and $S$ is the price of the risky asset at time $t$.

The boundary condition is given by

$$V(T,S)=g(S)$$

where $T$ is the expiration date of the option and $g(S)$ is the payoff of the option. 

The solution to the Black-Scholes equation can be found by solving the following initial value problem:

$$\frac{\partial V}{\partial t}+\frac{\sigma^2S^2}{2}\frac{\partial^2V}{\partial S^2}+\mu S\frac{\partial V}{\partial S}-rV=0$$

with boundary condition

$$V(T,S)=g(S)$$

The solution to this initial value problem is given by

$$V(t,S)=\mathbb{E}[e^{-r(T-t)}g(S_{T})|S_t=S]$$

where $S_{T}$ is the price of the risky asset at time $T$ and $S_t$ is the price of the risky asset at time $t$.