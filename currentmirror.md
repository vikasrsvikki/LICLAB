CURRENT MIRRORING EXPERIMENT

Introduction 

A current mirror is a circut designed to duplicate a current from one branch of a circut to another. it is often usde in analog design to provide a stable reference current that can be replicate through various part of the circut , typically in differential amplifier or other type of active circut current mirror are widly used due to their high output resistence , improved accuracy , and ability to maintain constant independent of voltage variation . the experiment involve simulating different currnt mirror circut ,such as basic current mirrors , ans cascade current mirrors to analyse their performence , current transfer accuracy , the voltage dependencies , by understanding their circuits , enginnners can design efficient current source and biasing networks for various analog and mixed-signal application


![image](https://github.com/user-attachments/assets/883dd7a3-66c1-4879-86a0-69c3bb39b6a7)


Purpose of current mirroring circuits:

-> to provide a constant current to part of the circut without relying on resistors

-> to creat a stable reference current for other parts of the circut .

-> to improve the matching of current source multiple transistors or stages.

How it Works :

a basic current mirror consist of two transistor , typically bipolar junction transistors (BJT) or MOSFET's, arrenged in a configuration where the current flowing through one transistor is mirrored in the second transistor . 

-> Reference Current (Iref) : the first transistor (often called the reference transistor ) is biased with a known reference current , which could be set using a resistor or another circut .

-> current Duplication : the second transistor (called the output transistor) is arrenged so that it mirrors the reference current . the base (or gate in MOSFETs) is also tied together , and ideally , the emmitor is also tied together , forcing the same current to flow through both transistors.

-> Matching Current : the current flowing through the second transistor id designed to be the same as the current in thr reference transistor , this is typically achived by ensuring that both transisitor have matching charectaristics , such as the same geometry , temperature , and other factors.

Types of current Mirrors : 

1) simple current mirror :- The most basic current mirror consists of two transistors. however , it may not provide precies current mirroring under all conditions.

2) Wilson current mirror :- this configuration adds the third transistor to improve the output current accuracy . it provide better performence by reducing the effect of early voltage (which cause the output current to depend on the output voltage )

3) Cascode Current Mirror :- a cascode current mirror adds additional transistor to future improvr performence by incresing the output impedence and reducing the impact and reducing the impact of variation in voltage , making the current more stable .

4) Active current Mirroes :-  uses additional circutary , often with feedback , to enhance the precision and stability of the current mirror , even in the presence of variation in temperature and supply voltage .

Advantages of Current Mirrors : 

1) Stability : they provide a stable current thai is less sensitive to supply voltage fluctuation .

2) Compactness : Current mirrors reduce the need for bulky resistors and offer a more integrated way of providing reference current .

3) Accuracy : With proper design, currnt mirror can provide very accurate current replication .

AIM OF THE EXP : 

The objective of this experiment is to design, analyze, and simulate a current mirror circuit used as a load in an amplifier to evaluate its performance characteristics. The experiment focuses on

1. Designing Current Mirror Circuits

->Implementing a basic current mirror with a 1:1 current ratio.
->Analyzing the impact of device dimensions (W/L ratios) on current mirroring accuracy.
->Extending the design for 1:2 current mirroring to observe scaling effects.

2. Performance Analysis

->Conducting DC analysis to evaluate current transfer accuracy.

->Performing AC analysis to determine the frequency response and stability.

->Measuring the maximum output voltage swing in transient simulations.

3. Integration with a Differential Amplifier

->Replacing passive resistive loads with an active current mirror load.

->Comparing performance with conventional resistor-loaded differential amplifiers.

->Investigating gain improvement and common-mode rejection in the modified design.

4. Simulation, Current Mirror Ratio Variation, and Analysis

->Using LTspice to simulate circuit behavior.

->Evaluating the impact of channel length variation (Lmin = 180nm, L = 500nm, L = 1µm) on performance.

->Varying the current mirror ratio and analyzing its effect on circuit performance.

->Studying the impact of current mirroring on gain, stability, and output swing.



DESIGN QUESTION :


![image](https://github.com/user-attachments/assets/268f634a-57a6-4b8f-8e07-d566d2b712b8)

![image](https://github.com/user-attachments/assets/772a30c3-3fd6-4def-8ed2-c97aa52d7bfa)

ANALYSIS : 

GIVEN:

VDD = 1.8V

P <= 1mW

AV > -10v/v

ITOTAL = P/VDD

ITOTAL <= 1/1.8

ITOTAL <= 0.555mA

ITOTAL = IREF + IX

For 1:1 Current mirror ratio. IREF = 0.277mA & IX = 0.277mA

For 1:2 Current mirror ratio IREF is 0.185mA & IX = 0.365mA

THE ASPECT RATIO'S OF MOSFET IS 16.66

THE ASPECT RATIO'S OF MOSFET FOR 1:1 CURRENT MIRROR:

M1 = 3um/180nm

M2 = 3um/180nm

M3 = 3um/180nm VGS = 0.838V

THE ASPECT RATIO'S OF MOSFET FOR 1:2 CURRENT MIRROR:

M1 = 3um/180nm

M2 = 6um/180nm

M3 = 6um/180nm VGS = 0.763V

SIMULATION OF CURRENT MIRROR LOAD COMMON SOURCE AMPLIFIER OF 1:1 MIRROR RATIO.

1. DC ANALYSIS

Built the circuit as per the circuit diagram below

![image](https://github.com/user-attachments/assets/e3271183-c3ab-43b0-b3cb-89785aff5372)

To perform the DC Analysis click the edit simulation and select the DC OP point(.op).   


![image](https://github.com/user-attachments/assets/bf6a580f-ebed-417d-ad2a-19383e296328)

ID M1 = 277uA , ID M2 = 277.5uA , ID M3 = 277.5uA .

2.TRANAIENT ANALYSIS

To perform Transient analysis click the edit Simulation then click on Transient Analysis.
Now give the stop time as 10ms and Run.

![image](https://github.com/user-attachments/assets/4e0bd29b-b125-41a1-a523-0e93fc24bc26)

The above Output shows the Amplified Signal with 180° Phase Shift of input signal of Amplitude 50mV.

The Gian from The Transient Analysis is -10.1 V/V.

3. AC ANALYSIS

To perform AC Analysis click the edit simulation then click on AC Analysis.

Now select the type of sweep as Decade , No.of points as 10m and then give Starting frequency as 1Hz & Ending as 1MHz then Run.

![image](https://github.com/user-attachments/assets/47cc3c7b-df4d-4019-897c-cc70e3e92a6c)

Gain in db is 22.1db & Bandwidth is 2.29GHz .

6. SIMULATION OF CURRENT MIRROR LOAD COMMON SOURCE AMPLIFIER OF 1:2 MIRROR RATIO.

1.DC ANALYSIS

![image](https://github.com/user-attachments/assets/5c550d32-9d8e-4f96-8536-3ddcc167162e)

Follow the same steps to perform DC Analysis.

![image](https://github.com/user-attachments/assets/7c1203b9-7259-4395-9ba8-522a631f63c9)

ID M1 = 185uA , ID M2 = 365.17uA , ID M3 = 365.17uA .

2.TRANAIENT ANALYSIS

Follow the same steps to perform Transient Analysis.

![image](https://github.com/user-attachments/assets/ee382430-139c-4f77-bbd7-0a19d958a15a)

The above Output shows the Amplified Signal with 180° Phase Shift of input signal of Amplitude 50mV.

The Gian from The Transient Analysis is -11.69 V/V.

3. AC ANALYSIS

Follow the same steps to perform AC Analysis. 

![image](https://github.com/user-attachments/assets/4ce72250-f4b9-48d5-b9ec-13ac40bc3789)

Gain in db is 22.96db & Bandwidth is 1.435GHz .

7. SIMULATION OF CURRENT MIRROR LOAD COMMON SOURCE AMPLIFIER OF 1:3 MIRROR RATIO.

For 1:3 Current mirror ratio IREF is 0.139mA & IX = 0.416mA

THE ASPECT RATIO'S OF MOSFET FOR 1:3 CURRENT MIRROR:

M1 = 6um/180nm

M2 = 18um/180nm

M3 = 18um/180nm VGS = 0.632V

1.DC ANALYSIS

![image](https://github.com/user-attachments/assets/6412f619-ddae-4f6c-81c1-e6d004ff0627)

Follow the same steps to perform DC Analysis. 

![image](https://github.com/user-attachments/assets/5855e8b7-5a6f-48c0-8d92-9bd7f6877118)

ID M1 = 139uA , ID M2 = 416.08uA , ID M3 = 416.08uA .

2.TRANAIENT ANALYSIS

Follow the same steps to perform Transient Analysis.

![image](https://github.com/user-attachments/assets/c727dc38-16b7-47d9-9a1a-c9565c83de2c)

The above Output shows the Amplified Signal with 180° Phase Shift of input signal of Amplitude 50mV.

The Gian from The Transient Analysis is -14.69 V/V.

3. AC ANALYSIS

Follow the same steps to perform AC Analysis. 


![image](https://github.com/user-attachments/assets/2c4cc076-3f5a-42bc-9d30-1238fb381bc7)

Gain in db is 27.3db & Bandwidth is 493.415MHz .

8. SIMULATION OF CURRENT MIRROR LOAD COMMON SOURCE AMPLIFIER OF 1:4 MIRROR RATIO.

For 1:4 Current mirror ratio IREF is 0.111mA & IX = 0.444mA

THE ASPECT RATIO'S OF MOSFET FOR 1:4 CURRENT MIRROR:

M1 = 9um/180nm

M2 = 36um/180nm

M3 = 36um/180nm VGS = 0.604V

1.DC ANALYSIS


![image](https://github.com/user-attachments/assets/0f70651e-26bc-48a9-823f-c74ab4ed56f4)

![image](https://github.com/user-attachments/assets/3aac8186-9ec0-4dfd-b82c-e4c02e2b83f0)

ID M1 = 111uA , ID M2 = 444.39uA , ID M3 = 444.39uA .

2.TRANAIENT ANALYSIS

Follow the same steps to perform Transient Analysis.

![image](https://github.com/user-attachments/assets/baa04229-b320-44d6-af72-613475d24e4e)

The above Output shows the Amplified Signal with 180° Phase Shift of input signal of Amplitude 50mV.

The Gian from The Transient Analysis is -15.6 V/V.

3. AC ANALYSIS

Follow the same steps to perform AC Analysis.

![image](https://github.com/user-attachments/assets/be379a92-b735-4ec3-a877-c188c0ac3aef)

Gain in db is 28.4db & Bandwidth is 246.09MHz .

9.VARRIYING L VALUE:

I) L=500nm then w = 8.334um NOW PERFORMING THE DC ANALYSIS:

![image](https://github.com/user-attachments/assets/8fdc4b56-2f51-4988-b658-9fcaabd77500)

ID M1 = 82.7mA , ID M2 = 0.768pA , ID M3 = 2.52pA .

II)L = 1um then W = 16.667u NOW PERFORMING THE DC ANALYSIS:


![image](https://github.com/user-attachments/assets/5163a313-d98a-40c0-8daa-25b3712edaf6)

ID M1 = 167.101mA , ID M2 = 2.74pA , ID M3 = 4.766pA .

10. PART B:DESIGN OF DIFFERENTIAL AMPLIFIER USING CURRENT MIRROR

The circuit comprises six MOSFETs (M1 to M6) with distinct (W/L) ratios, designed to operate in the saturation region to maintain accurate current mirroring and signal amplification. The aspect ratios of the transistors are carefully chosen to optimize transconductance (gm), output resistance (ro), and overall circuit stability.

M1, M2, M3: (W/L) = 108μm / 180nm

→ These transistors form the current mirror pair, ensuring precise current replication.

M4: (W/L) = 49.1μm / 180nm

→ Acts as an active load, influencing the gain and linearity of the circuit.

M5, M6: (W/L) = 57.33μm / 180nm

→ Function as differential pair transistors, determining the circuit's input impedance and common-mode rejection ratio (CMRR).

1.DC ANALYSIS

Built the circuit as per the circuit diagram below

![image](https://github.com/user-attachments/assets/c29a25ff-316d-4e69-bf45-70d37b4dce8e)

To perform the DC Analysis click the edit simulation and select the DC OP point(.op).

![image](https://github.com/user-attachments/assets/1eb017e5-f3e3-48e6-b9fb-6fda1f21ad9d)

2.TRANSIENT ANALYSIS

Follow the same steps to perform Transient

![image](https://github.com/user-attachments/assets/8fb2ee26-4d05-4da1-bc5a-5d0ba56b2b5f)

GAIN is -29.6/20 = 1.45 v/v.

3.AC ANALYSIS

![image](https://github.com/user-attachments/assets/b5384803-8c02-45cb-8bdf-72bcb22ac2a1)

The Gain is 25.3db.

RESULT : 

Performance Comparision table wrt Current Mirror Ratio:


![image](https://github.com/user-attachments/assets/c3e99dde-4122-4c1f-80ba-690481c10651)

12.INFERENCE

From the experiment and simulations, the following technical inferences can be drawn regarding the Current Mirror Load Common Source Amplifier and the impact of varying the current mirror ratio:

1. Impact of Current Mirror Ratio on Gain and Bandwidth

As the current mirror ratio increases, the gain increases, as seen from the values in the comparison table:

1:1 ratio → Gain = -10.1 V/V

1:2 ratio → Gain = -11.69 V/V

1:3 ratio → Gain = -14.69 V/V

1:4 ratio → Gain = -15.6 V/V

This happens because a larger IX (mirrored current) increases the transconductance (gm), which directly impacts the voltage gain:

[ A_v = -g_m \cdot r_o ]

However, as gain increases, bandwidth decreases significantly due to the trade-off between gain and frequency response:

1:1 ratio → Bandwidth = 2290 MHz

1:2 ratio → Bandwidth = 1435 MHz

1:3 ratio → Bandwidth = 493.4 MHz

1:4 ratio → Bandwidth = 246.1 MHz

The higher gain reduces the bandwidth because increasing the W/L ratio of the MOSFETs increases capacitance, which limits high-frequency response.

2. Voltage Variations and Threshold Effects

The gate-source voltage (VGS) decreases as the current mirror ratio increases:

1:1 ratio → VGS = 0.838V

1:2 ratio → VGS = 0.763V

1:3 ratio → VGS = 0.632V

1:4 ratio → VGS = 0.604V

This happens because, in a current mirror, the MOSFET aspect ratio (W/L) is adjusted to achieve the required current ratio.
A lower VGS suggests that the MOSFETs are operating deeper in the saturation region, which improves current replication accuracy.

3. Effect of MOSFET Aspect Ratio (W/L)

As the current mirror ratio increases, the W/L ratio of the current mirror transistors (M2, M3) increases significantly:

1:1 ratio → (M2, M3) = 3µm/180nm

1:2 ratio → (M2, M3) = 6µm/180nm

1:3 ratio → (M2, M3) = 18µm/180nm

1:4 ratio → (M2, M3) = 36µm/180nm

Increasing W/L improves current mirroring accuracy but increases parasitic capacitance, affecting speed and stability.
A larger MOSFET results in higher output resistance (r_o), which enhances gain but reduces bandwidth.

4. DC Accuracy and Current Matching

From the DC Analysis, it is observed that ID (drain current) values closely match the expected current mirror ratios:

Example for 1:2 ratio:

IREF = 185 µA, IX (mirrored current) = 365 µA, which is very close to the expected 1:2 ratio.

Example for 1:3 ratio:

IREF = 139 µA, IX = 416 µA, which is also accurate.

This confirms that the current mirror circuit effectively replicates the reference current, proving its reliability in biasing applications.

5. Trade-offs Between Gain, Bandwidth, and Stability

->Higher current mirror ratios provide more gain but reduce bandwidth.

->Large W/L ratios enhance current mirroring accuracy but introduce higher parasitic capacitance, affecting high-frequency performance.

->The circuit shows 180° phase shift, as expected for a common-source amplifier with active load.

->For applications requiring higher bandwidth (e.g., RF amplifiers), a lower current mirror ratio (1:1 or 1:2) is preferable.

->For applications needing high gain (e.g., precision analog circuits), a higher current mirror ratio (1:3 or 1:4) is beneficial.

6.Gain and Bandwidth Are Lower in Differential Mode

->In differential mode, both gain and bandwidth are typically lower compared to single-ended operation due to the way signals are processed and shared between transistors. 

->Since the amplifier responds only to the difference between two input signals, each transistor receives only half of the total signal, effectively reducing the gain. Additionally, the load is shared between both transistors, further decreasing the overall amplification. 

->Bandwidth reduction occurs due to increased parasitic capacitances introduced by current mirror loads and common-mode rejection circuits, which limit high-frequency performance. Moreover, the input capacitance is effectively doubled in differential mode, leading to a lower bandwidth compared to single-ended operation. 

->These factors create a trade-off where differential amplifiers provide better noise immunity and rejection of common-mode signals but at the cost of reduced gain and bandwidth.

7.Effect of Changing L Value in a Current Mirror

->In a current mirror circuit, the length (L) of the MOSFET channel plays a crucial role in determining the device characteristics.

->When the L value is changed, it affects the output current due to variations in channel resistance and output conductance. A longer channel length (higher L) increases channel resistance, reducing short-channel effects and improving output resistance, which helps maintain a more stable current. 

->Conversely, a shorter channel length (lower L) results in increased channel modulation, causing greater variations in output current due to drain voltage changes. This explains why modifying the L value alters the mirrored current, impacting the circuit's performance and accuracy.

13. Conclusion

->The experiment successfully demonstrates how varying the current mirror ratio impacts the performance of an amplifier.

->Current mirror loads provide significant gain enhancement over resistive loads, making them ideal for differential amplifiers and operational amplifiers.

->A balance between gain and bandwidth must be considered based on circuit requirements.

->The results validate theoretical expectations, confirming the accuracy and efficiency of current mirrors in analog design.






