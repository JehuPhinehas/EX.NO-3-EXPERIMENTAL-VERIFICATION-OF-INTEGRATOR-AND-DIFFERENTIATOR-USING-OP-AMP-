3. #**EX.NO:
** 3  EXPERIMENTAL VERIFICATION OF INTEGRATOR AND DIFFERENTIATOR USING OP-AMP 
            
**DATE:**  
             3A INTEGRATOR
---

## AIM
To design and test the performance of integrator and differentiator circuits using Op-amp

---

## APPARATUS REQUIRED

| S.No | Name of the Apparatus | Range | Quantity |
|------|------------------------|--------|-----------|
| 1 | Function Generator | 3 MHz | 1 |
| 2 | DSO | 30 MHz | 1 |
| 3 | Dual RPS | (0 – 30) V | 1 |
| 4 | Op-Amp | µA741 | 1 |
| 5 | Bread Board | — | 1 |
| 6 | Resistors | 1K,10K,100K  | 2 |
| 7 | capacitors | 0.1µF,0.01µF | 1 |
| 8 | Connecting wires and probes | As required | — |

---

## THEORY
INTEGRATOR
A circuit in which the output voltage waveform is the integral of the input voltage waveform is the integrator. Such a circuit is obtained by using a basic inverting amplifier configuration if the feedback resistor Rf is replaced by a capacitor Cf . The expression for the output voltage is given as,
Vo = - (1/Rf C1 ) ∫ Vi dt

Here the negative sign indicates that the output voltage is 180 0 out of phase with the input signal. Normally between fa and fb the circuit acts as an integrator. Generally, the value of fa < fb . The input signal will be integrated properly if the Time period T of the signal is larger than or equal to Rf Cf . That is,
T ≥ Rf Cf

The integrator is most commonly used in analog computers and ADC and signal-wave shaping circuits.
CIRCUIT DIAGRAM
## CIRCUIT DIAGRAM
<img width="1600" height="1141" alt="image" src="https://github.com/user-attachments/assets/f7087efc-f933-4663-99c9-e73a50e543d9" />



## MODEL GRAPH
<img width="807" height="1279" alt="image" src="https://github.com/user-attachments/assets/ab65b181-f288-475e-ab12-a68420c5575b" />

---

## DESIGN
<img width="1125" height="540" alt="image" src="https://github.com/user-attachments/assets/f1ae3e5e-9195-4cfb-9f46-85b71179ba47" />


To obtain the output of an Integrator circuit with component values R1Cf = 0.1ms , Rf = 10 R1 and Cf = 0.01 µF and also if 1 V peak square wave at 1000Hz is applied as input.
We know the frequency at which the gain is 0 dB, fb = 1 / (2π R1 Cf) Therefore fb = 	 Since fb = 10 fa , and also the gain limiting frequency fa = 1 / (2π Rf Cf)
We get , R1 =	and hence Rf = 	

## PROCEDURE

1.	Connections are given as per the circuit diagram
2. + Vcc and - Vcc supply is given to the power supply terminal of the Op-Amp IC.
3.	By adjusting the amplitude and frequency knobs of the function generator, appropriate input voltage is applied to the inverting input terminal of the Op- Amp.
4.	The output voltage is obtained in the CRO and the input and output voltage waveforms are plotted in a graph sheet.


## TABULATION

<img width="1600" height="1228" alt="image" src="https://github.com/user-attachments/assets/0a490287-c2e2-446d-8469-e11ce9693bb0" />



---

## OUT PUT WAVEFORM AND DISCUSSION 

<img width="1065" height="1280" alt="image" src="https://github.com/user-attachments/assets/6a1dcfaa-1472-4cdf-90d2-5498670e6e59" />


---
**DATE:**  
             3 B DIFFERENTIATOR
---

## AIM
To design and test the performance of integrator and differentiator circuits using Op-amp

---

## APPARATUS REQUIRED

| S.No | Name of the Apparatus | Range | Quantity |
|------|------------------------|--------|-----------|
| 1 | Function Generator | 3 MHz | 1 |
| 2 | DSO | 30 MHz | 1 |
| 3 | Dual RPS | (0 – 30) V | 1 |
| 4 | Op-Amp | µA741 | 1 |
| 5 | Bread Board | — | 1 |
| 6 | Resistors | 1K,10K,100K  | 2 |
| 7 | capacitors | 0.1µF,0.01µF | 1 |
| 8 | Connecting wires and probes | As required | — |

---

## THEORY
DIFFEERENTIATOR:
The differentiator circuit performs the mathematical operation of differentiation; that is, the output waveform is the derivative of the input waveform. The differentiator may be constructed from a basic inverting amplifier if an input resistor R1 is replaced by a capacitor C1 . The expression for the output voltage is given as,
Vo = - Rf C1 ( dVi /dt )

Here the negative sign indicates that the output voltage is 180 0 out of phase with the input signal. A resistor Rcomp = Rf is normally connected to the non-inverting input terminal of the op-amp to compensate for the input bias current. A workable differentiator can be designed by implementing the following steps:
1.	Select fa equal to the highest frequency of the input signal to be differentiated. Then, assuming a value of C1 < 1 µF, calculate the value of Rf.
2.	Choose fb = 20 fa and calculate the values of R1 and Cf so that R1C1 = Rf Cf.

The differentiator is most commonly used in wave shaping circuits to detect high frequency components in an input signal and also as a rate–of–change detector in FM modulators.

## CIRCUIT DIAGRAM

<img width="1600" height="809" alt="image" src="https://github.com/user-attachments/assets/fd82ad15-df0a-45a2-a919-5ac2fb384205" />

## MODEL GRAPH

(i)	 SINE WAVE INPUT

<img width="1600" height="1103" alt="image" src="https://github.com/user-attachments/assets/c1d7c8be-e12e-4016-afca-9b223aea1054" />


AND

(ii) SQUARE WAVE INPUT

<img width="1600" height="1081" alt="image" src="https://github.com/user-attachments/assets/38dba052-46a0-4a7c-b1ac-7b622d0fa997" />



---

## DESIGN
<img width="1600" height="733" alt="image" src="https://github.com/user-attachments/assets/06fec87e-1f59-45d3-89f8-b02d432650f3" />

Design an op-amp differentiator that will differentiate an input signal with fmax = 100HZ Select fa = fmax = 100 HZ = 1 / 2πRFC1
Let C1 = 0.1μF
Then RF = 1 / 2π(102)(10-7)
= 15.9KΩ
Now choose fb = 10fa = 1 / 2πR1C1 Therefore, R1 = 1 / 2π(103)(10-7)
= 1.59KΩ Since RFCF = R1C1
We get, CF = (1.59*103*10-7) / 15.9*103
= 0.01μF


## PROCEDURE

1.	Connections are given as per the circuit diagram
2. + Vcc and - Vcc supply is given to the power supply terminal of the Op-Amp IC.
3.	By adjusting the amplitude and frequency knobs of the function generator, appropriate input voltage is applied to the inverting input terminal of the Op- Amp.
4.	The output voltage is obtained in the CRO and the input and output voltage waveforms are plotted in a graph sheet.

 ## TABULATION

<img width="1600" height="953" alt="image" src="https://github.com/user-attachments/assets/81b815a2-6c49-47e0-bf0a-17d4a18ed2c6" />
<img width="1600" height="679" alt="image" src="https://github.com/user-attachments/assets/4345f228-bf60-4505-9c1b-8d2bb88c9a33" />



## OUT PUT WAVEFORM AND DISCUSSION 

<img width="984" height="1279" alt="image" src="https://github.com/user-attachments/assets/8c1e2ddf-7162-4fdc-91c4-443947714843" />

---

RESULT:
<img width="1600" height="696" alt="image" src="https://github.com/user-attachments/assets/348babbb-e46a-4c68-ba93-73a9d2ab2000" />

Thus an Integrator and Differentiator using op-amp are designed and their performance was successfully tested using op-amp IC 741.
---



