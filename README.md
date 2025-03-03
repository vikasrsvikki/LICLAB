Experiment-1
Question : Given that POWER, P=100µ W; Perform DC Analysis, Transient Analysis and AC Analysis for the Given Circuit Designs and also check what happens when the width is increased or decreased of each mosfet;

Design-1 :
![image](https://github.com/user-attachments/assets/e96b0504-3a42-4e5a-abf9-a6a98479f59b)
Using the Formula for Power,

P=V*I

We will get the Values of Id as,

Id= 5.56 * 10^-5 A

we have to get the output current, Id for the given circuits by adjusting the values of L & W( Length and Width of the Channel of the MOSFET)

Length and Width of the Channel used to obtain the given Current is shown in the figure below;
![image](https://github.com/user-attachments/assets/c5a923bd-e64c-4e15-8074-bcd728b540d2)
1)DC ANALYSIS:

Procedure for Performing DC Analysis: we have to select the dc output print(DC op pnt) in the Edit Simulation Command and Run the Simulation
![image](https://github.com/user-attachments/assets/6bbe022f-34e8-49db-8357-5db322f2e768)
The Figure below shows the Values obtained from the DC Analysis :
![image](https://github.com/user-attachments/assets/d74b31b6-6d08-4dc0-aa08-628d0d965447)
2)Transient Analysis:

Procedure for Performing Transient Analysis: we have to select the Transient Analysis in the Edit Simulation Command, Give the stop time as 1ms and Run the Simulation.
![image](https://github.com/user-attachments/assets/3523e3f9-fa0c-4ee1-ab32-ae9c5eb452f6)
The Graphs below shows the Transient Response of the Given Design;
![image](https://github.com/user-attachments/assets/0507f75e-b836-4ae2-b211-91c8d6af7eda)
![image](https://github.com/user-attachments/assets/77484715-c9e3-4d6e-86d8-200786517473)
3)AC Analysis:

Procedure for Performing AC Analysis: we have to select the AC Analysis in the Edit Simulation Command, Give the values as shown in the figure beowl and Run th Simulation.
![image](https://github.com/user-attachments/assets/09885c9d-5273-4447-b7e5-2417134bd2a6)
The Graph below shows the AC Analysis of the Given Design;
![image](https://github.com/user-attachments/assets/070ce873-e414-49a0-b092-7401e64916b6)
RESULT( Design-1):
DC Analysis:

The calculated drain current (Id) matches the expected value based on power and voltage, Id = 5.56*10^-5 A.
By adjusting the MOSFET’s channel dimensions (L & W) where L=180nm and W= 203nm, The current requirement was succesfully achecived.
The circuit behaves as expected under DC conditions.
Transient Analysis:

The transient response graph shows how the circuit behaves over time.
The response is smooth, with no unexpected delays or distortions.
The circuit reacts well to changes, confirming its stability.
The gain obtained is 1.85.
AC Analysis:

The AC response graph confirms that the circuit remains stable at different frequencies.
The gain(2 dB) and phase shift(which is nearly 180deg) align with theoretical expectations.
The circuit maintains its performance across the tested frequency range.
INFERENCE( Design-1):
The experiment confirms that by properly selecting the MOSFET dimensions, we can control the drain current effectively.
Impact of Width Adjustments:
M1 has a influence on Id, meaning its width affects the output current.
The circuit performs well in all three analyses—DC, transient, and AC—demonstrating its reliability.
Overall, the design works as intended, following theoretical predictions and proving its practical feasibility.
Design-2
![image](https://github.com/user-attachments/assets/2d545fa6-4ac7-4650-acd3-1ae02eb50443)
Using the Formula for Power,

P=V*I/n

We will get the Values of Id as,

Id= 5.56 * 10^-5 A

we have to get the output current, Id for the given circuits by adjusting the values of L & W of both the MOSFETS M1 & M2 ( Length and Width of the Channel of the MOSFET)

DC SWEEP Analysis: This analysis is done for obataing the value of Vin in Saturation range;

we have to select the DC SWEEP in the Edit Simulation Command, Give the values as shown in the figure below and Run th Simulation.
![image](https://github.com/user-attachments/assets/783a9d9f-3d54-4b33-aeba-1c597dac0999)
The Graph below represents the VTC Curve and the value of the vin is selected as 0.7V as it is present in the saturation region of the VTC Curve
![image](https://github.com/user-attachments/assets/75d5bb60-52cf-4c44-bdef-1f5cf13330f0)
Then the input voltage parameters are given as;
![image](https://github.com/user-attachments/assets/934417f1-8150-4b7c-a448-0ad41927a7e8)
Length and Width of the Channel of the two MOSFETS used to obtain the given Current is shown in the figure below;
![image](https://github.com/user-attachments/assets/b4e96c67-f973-4d34-ad7e-31f234b0ea9f)
![image](https://github.com/user-attachments/assets/3489aba3-b4db-4a36-95ac-d7a0b9df5a46)
Now we will be performing the DC, Transient and AC Anlaysis;

1)DC ANALYSIS:

rocedure for Performing DC Analysis: we have to select the dc output print(DC op pnt) in the Edit Simulation Command and Run the Simulation.
![image](https://github.com/user-attachments/assets/f4d7172b-561f-451a-ad24-f581a9eb2f77)
The Figure below shows the Values obtained from the DC Analysis :
![image](https://github.com/user-attachments/assets/acf1b0bb-c6e7-4133-80e8-239a1a2d2c86)
2)Transient Analysis:

Procedure for Performing Transient Analysis: we have to select the Transient Analysis in the Edit Simulation Command, Give the stop time as 1ms and Run the Simulation.
![image](https://github.com/user-attachments/assets/57fef40b-0ff9-46b0-a1e6-3ef46159c251)
The Graphs below shows the Transient Response of the Given Design;
![image](https://github.com/user-attachments/assets/e423f318-ddb5-48e5-9691-edeab7e9b4b5)
![image](https://github.com/user-attachments/assets/55417146-f794-4d42-9e17-298d15709954)
3)AC Analysis:

Procedure for Performing AC Analysis: we have to select the AC Analysis in the Edit Simulation Command, Give the values as shown in the figure beowl and Run th Simulation.
![image](https://github.com/user-attachments/assets/9b1ab294-eb4b-4ddf-bc30-ef1514c774ea)
the Graph below shows the AC Analysis of the Given Design;
![image](https://github.com/user-attachments/assets/78b182f9-6fec-4a9e-87cc-fafcc55a0c88)
RESULT(DESIGN-2)
1.DC Analysis:

The calculated drain current (Id) aligns with the expected value based on power and voltage, where the value of Id = 5.56*10^-5 A .
By fine-tuning the channel dimensions (L & W) of both MOSFETs ( M1 & M2), the desired current was achieved,
M1 : L= 180nm , W= 1105nm.
M2 : L= 180nm , W= 1105nm.
The circuit operates correctly within the selected DC parameters.
2.Transient Analysis:

The transient response graph confirms that the circuit transitions smoothly over time.
The circuit responds effectively to input variations, indicating stable operation.
The gain obtained is 2.28.
3.AC Analysis:

The AC response graph confirms that the circuit maintains stability over the tested frequency range.
The gain(5.5 dB) and phase shift (which is nearly 180deg) align with theoretical expectations.
The circuit functions as expected under AC conditions.
Inference (Design-2):
The experiment validates that by appropriately selecting the MOSFET dimensions (L & W), the drain current can be precisely controlled.

The voltage transfer characteristics (VTC) helped in selecting the correct operating voltage (0.7V) for saturation.

Impact of Width Adjustments:

M2 has a stronger influence on Id, meaning its width significantly affects the output current.
M1 has a smaller influence, meaning changes in its width result in only minor variations in Id.
The design meets the expected performance criteria and follows theoretical predictions, demonstrating its feasibility in practical applications.



