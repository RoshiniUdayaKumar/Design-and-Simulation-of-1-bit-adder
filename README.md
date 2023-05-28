# Design-and-Simulation-of-1-bit-adder

In this project, we will design a 1-bit adder which is used to further design a 4-bit adder. 

The objective of this project is to perform post-layout simulations. After verifying that the DRC and LVS have passed without any errors, we shall extract the parasitics to perform post-layout simulations. This will provide a clear understanding of the circuit speed, the effect of parasitics on the circuit, and any glitches introduced due to signal delay mismatches. 

Unlike only designing the layouts only with VDD and GND, this will not assure that the circuit will perform as desired. Hence, we will apply the required voltage and load to the pins and measure the performance of the circuit. 

Steps followed to accomplish this:

1. Creating a symbol of the standard cell.

2. Creating a test bench using the symbol we created.

3. Creating the layout of the standard cell.

4. Observing the waveforms for transient simulation.

5. Plotting waveforms for the extracted parasitics.
 
6. Measuring the rising and falling delays from the waveform.

Important Notes to remember:

1. To accomplish the optimal trade-off between area and frequency and to ensure that the worst-case and best-case delays of the circuit do not significantly differ from one another, we would prefer to match the rising and falling delays of the standard cells. 

2. Make sure the heights of all the common cell arrangements are equal. Because we will eventually use each of these gates to construct an adder circuit, we must arrange them close together. The Nwell areas of all the cells can be combined as well as the power lines VDD and GND when they are of the same height.

Next, we will use the standard cells to build a single-bit adder

Symbol of an Inverter:

![InverterSymbol](https://github.com/RoshiniUdayaKumar/Design-and-Simulation-of-1-bit-adder/assets/133715179/0c032b09-2ccd-4674-a38d-0c12d3371874)

Layout of an Inverter:

![Inverterlyt](https://github.com/RoshiniUdayaKumar/Design-and-Simulation-of-1-bit-adder/assets/133715179/ea6bad8a-bc0e-41df-a0ce-02c652d14648)

Circuit Under Test(CUT):

![Inverterschm](https://github.com/RoshiniUdayaKumar/Design-and-Simulation-of-1-bit-adder/assets/133715179/c9b1c626-e2ca-4daa-bff8-fbbe5b25bc60)

![in_out plot](https://github.com/RoshiniUdayaKumar/Design-and-Simulation-of-1-bit-adder/assets/133715179/1fd5fd47-285f-4432-bff1-2ee7a08f2634)

![image](https://github.com/RoshiniUdayaKumar/Design-and-Simulation-of-1-bit-adder/assets/133715179/ce361662-e3f8-4163-bbff-d96a3c11b670)


![split in_out](https://github.com/RoshiniUdayaKumar/Design-and-Simulation-of-1-bit-adder/assets/133715179/59013925-c6d9-4ca9-9d32-65e119a47e8b)

Delay Plots:

![power, delay plot](https://github.com/RoshiniUdayaKumar/Design-and-Simulation-of-1-bit-adder/assets/133715179/9fda872d-1325-4726-b4ff-5ef8d390eb70)

Falling delay for inverter cell is 2.57E-10 and the occurrence time is 3.05E-09

NAND:

Symbol of a NAND Gate:

Layout of a NAND:

![NAND2lyt](https://github.com/RoshiniUdayaKumar/Design-and-Simulation-of-1-bit-adder/assets/133715179/df2be439-a112-4ad9-84ae-423176a7d2b9)

Circuit Under Test (CUT):

![NAND2crkt](https://github.com/RoshiniUdayaKumar/Design-and-Simulation-of-1-bit-adder/assets/133715179/a324e4a0-55e1-418b-9d7f-2402d5ca5144)

Input-Output voltage Plots:

![Plot1](https://github.com/RoshiniUdayaKumar/Design-and-Simulation-of-1-bit-adder/assets/133715179/93a4d608-cf33-4141-bc84-e20fb7eda2ed)

![image](https://github.com/RoshiniUdayaKumar/Design-and-Simulation-of-1-bit-adder/assets/133715179/cc6c4f16-a509-491c-be11-c587dda51aed)

Extracted Parasitic Plots:

![Combined plot](https://github.com/RoshiniUdayaKumar/Design-and-Simulation-of-1-bit-adder/assets/133715179/e53c3ae4-c919-4211-b94e-250ebd67e6ba)

![Split plot](https://github.com/RoshiniUdayaKumar/Design-and-Simulation-of-1-bit-adder/assets/133715179/0a949b68-a26b-468b-89ef-6ce62b721601)

Delay Curve:

![Delay curve](https://github.com/RoshiniUdayaKumar/Design-and-Simulation-of-1-bit-adder/assets/133715179/300256c0-53f0-4b5a-b282-89c5cfa8ee22)


