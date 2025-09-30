When the ripple is big enough to change the polarity of the semiconductor devices, the converter transitions
into a new mode of operation. The boundary between continuous conduction mode (CCM) and discontinuous conduction
mode (DCM) can be identified by first assuming CCM and then evaluating the condition at critical conduction mode (CRM),
where this polarity change just begins. By rearranging the inequality—placing the terms involving the duty ratio $D$ 
on one side and the remaining terms on the other—we obtain the condition:
$$K<K_{crit} (D)$$

Once this new mode of operation occurs, the conversion ratio $M$ also changes. To calculate $M$ , we apply the inductor
volt–second balance and capacitor charge balance under steady-state conditions. However, in this case only a restricted
version of the linear-ripple approximation can be used. While designers typically aim for small output voltage ripple, 
inductor currents or capacitor voltages may still contain large switching ripples, preventing full use of the approximation.
After some algebra, the steady-state analysis yields the new expression for $M(D,K)$ .

Tips
1. When calculating $M(D,K)$ , start with the inductor volt–second balance and capacitor charge balance. Before diving into 
long algebra, simplify by forming $M$  and $K$  directly through dividing or multiplying both sides by $V_g$ and other parameters.
2. When working in CCM, always compare magnitudes carefully. Otherwise, $V_g$ may flip the inequality direction.
3. Memorize $M(D,K), K$ , $K_{crit}(D)$ for the basic converters.

| Converter  | Conversion Ratio $M(D)$ | $K$ | $K_{\text{crit}}(D)$ |
|------------|-------------------------|-----|----------------------|
| Buck       | $M = frac{2}{1+sqrt(1+frac{4K}{D^2})}$                 | $K = \tfrac{2L}{RT_s}$ | $K_{\text{crit}}(D) = \tfrac{1}{2(1-D)}$ |
| Boost      | $M = \tfrac{1}{1-D}$    | $K = \tfrac{2L}{RT_s}$ | $K_{\text{crit}}(D) = \tfrac{D}{2(1-D)}$ |
| Buck-Boost | $M = \tfrac{D}{1-D}$    | $K = \tfrac{2L}{RT_s}$ | $K_{\text{crit}}(D) = \tfrac{D}{2(1-D)}$ |
