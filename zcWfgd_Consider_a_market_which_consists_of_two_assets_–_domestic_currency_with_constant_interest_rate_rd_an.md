

### Replication Prices of European Call and Put Options

A European call option gives the holder the right to buy one unit of the foreign currency at the exchange rate K at moment of time T. This can be replicated by a self-financing strategy πt= (Gt,Ht) with Gt=0 and Ht=H, where

<p align="center">
$H = \frac{KX_T - V_{\pi T}}{X_T - K}$
</p>

The value of the portfolio in the domestic currency is equal to Vπt = Gt+HtXt

<p align="center">
$V_{\pi t} = HX_t$
</p>

For the self-financing property of the strategy, we have:

<p align="center">
$dV_{\pi t}=rdGtdt+rfHtXtdt+HtdXt$
</p>

By setting Gt=0, we obtain

<p align="center">
$dV_{\pi t}=rfHtXtdt+HtdXt$
</p>

By solving the above equation, we obtain

<p align="center">
$H = \frac{X_T(r_f - \mu)}{K(r_f - r_d) - \mu}$
</p>

Therefore, the replication price of the European call option is given by

<p align="center">
$C_0 = V_{\pi 0} = HX_0 = \frac{X_0(KX_T - X_0(r_f - \mu))}{K(r_f - r_d) - \mu}$
</p>

Similarly, for a European put option, the replication price is given by

<p align="center">
$P_0 = V_{\pi 0} = HX_0 = \frac{X_0(X_T - K(r_f - \mu))}{K(r_f - r_d) - \mu}$
</p>