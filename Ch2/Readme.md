# Principles of Steady-State Converter Analysis
 The small-ripple approximation assumes that the ripple of a continuous variable, such as capacitor voltage, is much smaller than its DC value. This 
is justified because engineers generally design circuits with small ripples. Under this assumption, the ripple can be treated as approximately linear,
which is why the method is also called the linear-ripple approximation.
 When we apply the small-ripple approximation and the calculated value is not zero, the result is expressed mainly in terms of dominant DC terms. 
In this case, small changes in the variables do not significantly affect the result, so the approximation is valid. However, if the result turns 
out to be zero, the dominant terms disappear from the expression, and even small variations cannot be ignored. In such cases, the approximation
is not valid.
 We analyze converters using three tools: inductor volt-second balance, capacitor amp-second balance, and the small-ripple approximation. However,
when the result of the last one is zero, we must be ready to abandon it. In steady state, a converter cannot operate correctly unless the first two balances hold true:

$$\langle v_L \rangle = \frac{1}{T_s}\int_0^{T_s} v_L \, dt = 0$$
$$\langle i_C \rangle = \frac{1}{T_s}\int_0^{T_s} i_C \, dt = 0$$

It would be useful to memorize the DC capacitor voltages and inductor current of basic converters, such as buck, boost, buck-boost converters.

### Buck Converter
$$V = D V_g$$
$$I_L = \frac{D V_g}{R}$$
### Boost Converter
$$V = \frac{V_g}{D'}, \quad D' = 1 - D$$
$$I_L = \frac{I_o}{D'} = \frac{V_g}{D'^2 R}$$
### Buck-Boost Converter
$$V = -\frac{D}{D'} V_g, \quad D' = 1 - D$$
$$I_L = \frac{I_o}{D} = -\frac{V_g}{D'R}$$
