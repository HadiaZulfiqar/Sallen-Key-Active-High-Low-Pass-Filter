<h1>Sallen-Key 4th Order Active Low-Pass Filter</h1>

Proteus simulation, mathematical calculations, and PCB layout implementation of a 4th-order active low-pass Sallen-Key Butterworth filter designed for a 1 kHz cutoff frequency and 10 dB voltage gain.

<h2>Simulation</h2>
<img width="1002" height="446" alt="image" src="https://github.com/user-attachments/assets/8c8bcd72-9aab-4f2e-9113-43e0075cce27" />

<h2>explanation</h2>

<h3>Overview</h3>
<p>
This project covers the complete design and evaluation of an active 4th-order low-pass filter using the Sallen-Key topology. The system is split into two cascaded biquad stages to achieve sharp frequency attenuation past the 1 kHz cutoff threshold while providing a 10 dB voltage gain.
</p>

<h3>Ideal Op-Amp Simulation</h3>
<p>
Using an idealized operational amplifier model, the circuit maintains stable behavior with precise component values ($1.59\text{ k}\Omega$ resistors and $0.1\,\mu\text{F}$ capacitors). The time-domain response and Bode plots demonstrate clean passband amplification and a standard Butterworth roll-off characteristic.
</p>
<img width="1027" height="458" alt="image" src="https://github.com/user-attachments/assets/f9137bdb-f39e-4d98-b02f-429dd0c36305" />
<img width="923" height="490" alt="image" src="https://github.com/user-attachments/assets/ed0a6a95-fa09-4093-896e-dc6a3c3a044e" />

<h3>LM358 Practical Implementation</h3>
<p>
Transitioning to the real-world LM358 operational amplifier requires adjusting component values to standard E12 ranges ($1.6\text{ k}\Omega$ resistors and $1.2\text{ k}\Omega$ gain resistors). Due to practical limitations like finite bandwidth, common-mode voltage ranges, and slew rates, the circuit exhibits minor non-ideal behaviors such as high-frequency phase shifts and gain variations.
</p>
<img width="988" height="430" alt="image" src="https://github.com/user-attachments/assets/a229a83b-3161-4ccf-ac39-7349f3c53db2" />
<img width="691" height="472" alt="image" src="https://github.com/user-attachments/assets/9794ca69-a36d-4d8e-b6cd-81e48f1d5b71" />

<h3>PCB Layout Design</h3>
<p>
The printed circuit board (PCB) layout organizes the dual LM358 IC packages, axial resistors, and disc capacitors onto a compact green board. Input/output pin headers and power connectors are routed cleanly to minimize trace interference and ensure stable single-supply operation.
</p>
<img width="863" height="492" alt="image" src="https://github.com/user-attachments/assets/f1509db2-9a9a-456b-b020-fe17903565b8" />
