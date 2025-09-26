 **When the ripple in a DC converter circuit is small**, the converter can be approximated as an ideal DC transformer. The DC transformer model is time-invariant and therefore
contains only the DC component. Although it is not perfectly accurate, it provides useful intuition about the circuit.
 <br><br> Practical DC converters are not ideal because they include many sources of power loss, such as inductor copper and core loss, and voltage drops across semiconductor devices.
- Inductor copper loss can be modeled by adding a series resistance to the inductor.
- MOSFETs and BJTs can be modeled with an on-resistance.
- Diodes, IGBTs, and thyristors can be modeled with an on-resistance and a voltage source.
 Although $I_rms^2*R$is not exactly equal to $I_avg^2*R$, the difference is very small when ripples are small (for example, a 10% ripple produces only about a 0.33% difference).
Therefore, the DC transformer model can be used to calculate the DC component of the real circuit and the power absorbed or supplied by elements, even though the currents are represented
by their average values.
How to Approximate a DC Converter as a DC Transformer Circuit
1.	Derive the corresponding mesh and node equations from the volt-second balance and the charge balance, respectively.
2.	Use the small-ripple approximation to calculate $\langle i_g \rangle$, and represent the source as a voltage source $V_g$ with current $I_g$.
3.	Combine the circuits obtained from steps 1 and 2.
4.	Replace the dependent sources with an equivalent DC transformer.

