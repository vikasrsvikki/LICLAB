Expeiment-3 Aim: Design and Analyze the MOS differential amplifier circuit for the following specifcations and Perform DC analysis,Transient Analysis,Frequency response and extract parmeter

VDD=2v,P<=1mW,Vicm=1v,Vocm=1.1v,Vp=0.4v

Differential Amplifier: differential amplifiers consist of two transistors M1 and M2, whose sources are joined together. If two transistor are connected to the different voltage input then there current across M1 and M2 are different due to gate voltage.If in case the voltage supply at gate terminal is same then the current through the M1 and M2 are same.This configuration is called "Common Mode input voltage differential Amplifier".WHatever may be the load resistor, the MOSFET M1 and M2 should not go to the Triode region. It should be verified that MOSFET should be in Saturation Region.

For all this circuit we need find out the AC analysis ,Transient analysis And Frequency Response. Components Required: MOSFET(M1,M2), Resistor,voltage supply's Circuit-1
![image](https://github.com/user-attachments/assets/7d1ba1b0-648e-42ec-bff8-acc0112e59d3)
Procedure : Make the circuit connection as given above. connect the resister at the source terminal of both mosfet now calculate the value of Iss as power and vdd is given and calculate the Id1 and Id2 now calculate the Rss and Rd

Now to get the desired values of output voltage and current we have to vary the width and length of both the mosfet we got L=4um and W=184.5um

![iHere in dc analysis we got the vocm as expected and id1 and id2 we got the same

Transient analysis: To perform transient analysis we have to select the transient analysis in the edit simulation and give the stop time as 5ms and run the simulation . and the graph velow shows the transient response of the design.
![image](https://github.com/user-attachments/assets/e3575761-0316-436b-87b7-f74aea229e5a)
![image](https://github.com/user-attachments/assets/909f5026-ba49-4a02-91a8-0090cd33f45e)
AC analysis: TO perform AC analysis we have to select the ac analysis in the edit simulation command given the values as shown below
![image](https://github.com/user-attachments/assets/98709ff0-c1d6-4a4b-96a7-3a3b5653216f)
![image](https://github.com/user-attachments/assets/e0e01084-8d0b-4af4-8902-d3fcf4ff6c41)
Circuit-2: Now replace the R3 resister with a current source : connect a current souce of 1mA

CR2
![image](https://github.com/user-attachments/assets/1033badf-26a2-453f-b21d-5f694c9b75d6)
DC analysis: To perform the DC analysis we have to select the {DC op pnt} in the edit simulation command and run the simulation the figure below is the values obtained from the DC analysis

![image](https://github.com/user-attachments/assets/06e7d777-3bd1-4a07-ab77-c3cd067a9ce7)
Trasient analysis: To perform transient analysis we have to select the transient analysis in the edit simulation and give the stop time as 5ms and run the simulation . and the graph velow shows the transient response of the design

we have to give deg of 180deg to one mosfet and 0deg to the other mosfet and ac amplitude 1 for one mosfet and 0 for other mosfet
![image](https://github.com/user-attachments/assets/023e0960-e6ac-494e-b1e4-31f2289771f1)
ac analysis:
Circuit-3: Now replace the R3 resister with a Mosfet : Given vp=0.4v and wkt vt=0.36v we got the gate voltage of the new mosfet as 0.76v 
![image](https://github.com/user-attachments/assets/11b8db66-4344-4c20-a072-6509811ca9ef)

![image](https://github.com/user-attachments/assets/45b9603f-a70c-46ad-98cf-517b9399fc29)
DC analysis:

![image](https://github.com/user-attachments/assets/27c9b195-99bb-47d4-8bbb-96351f0e997f)
Transient analysis: give ac amplitude as 1 for one mosfet and 0 gor other mosfet
![image](https://github.com/user-attachments/assets/22f47f89-e3d5-4bd8-b47c-426330841343)
ac analysis
![image](https://github.com/user-attachments/assets/b98ba704-f772-4f8f-a2b3-e108ab68cb02)
README
Expeiment-3 Aim: Design and Analyze the MOS differential amplifier circuit for the following specifcations and Perform DC analysis,Transient Analysis,Frequency response and extract parmeter

VDD=2v,P<=1mW,Vicm=1v,Vocm=1.1v,Vp=0.4v

Differential Amplifier: differential amplifiers consist of two transistors M1 and M2, whose sources are joined together. If two transistor are connected to the different voltage input then there current across M1 and M2 are different due to gate voltage.If in case the voltage supply at gate terminal is same then the current through the M1 and M2 are same.This configuration is called "Common Mode input voltage differential Amplifier".WHatever may be the load resistor, the MOSFET M1 and M2 should not go to the Triode region. It should be verified that MOSFET should be in Saturation Region.

For all this circuit we need find out the AC analysis ,Transient analysis And Frequency Response. Components Required: MOSFET(M1,M2), Resistor,voltage supply's Circuit-1 Screenshot 2025-03-03 185706 Procedure : Make the circuit connection as given above. connect the resister at the source terminal of both mosfet now calculate the value of Iss as power and vdd is given and calculate the Id1 and Id2 now calculate the Rss and Rd

Now to get the desired values of output voltage and current we have to vary the width and length of both the mosfet we got L=4um and W=184.5um

Screenshot 2025-03-03 185640 DC analysis: To perform the DC analysis we have to select the {DC op pnt} in the edit simulation command and run the simulation the figure below is the values obtained from the DC analysis Screenshot 2025-03-03 185657 Here in dc analysis we got the vocm as expected and id1 and id2 we got the same

Transient analysis: To perform transient analysis we have to select the transient analysis in the edit simulation and give the stop time as 5ms and run the simulation . and the graph velow shows the transient response of the design. image AC analysis: TO perform AC analysis we have to select the ac analysis in the edit simulation command given the values as shown below image image Circuit-2: Now replace the R3 resister with a current source : connect a current souce of 1mA

CR2 Screenshot 2025-03-03 191456 DC analysis: To perform the DC analysis we have to select the {DC op pnt} in the edit simulation command and run the simulation the figure below is the values obtained from the DC analysis Screenshot 2025-03-03 192125 Trasient analysis: To perform transient analysis we have to select the transient analysis in the edit simulation and give the stop time as 5ms and run the simulation . and the graph velow shows the transient response of the design

we have to give deg of 180deg to one mosfet and 0deg to the other mosfet and ac amplitude 1 for one mosfet and 0 for other mosfet image AC analysis: image Circuit-3: Now replace the R3 resister with a Mosfet : Given vp=0.4v and wkt vt=0.36v we got the gate voltage of the new mosfet as 0.76v Screenshot 2025-03-03 194319 to get the output voltage and vp and current desired value we have to vary the width and length of the new mosfet Screenshot 2025-03-03 194311 DC analysis: Screenshot 2025-03-03 194331 Transient analysis: give ac amplitude as 1 for one mosfet and 0 gor other mosfet image AC analysis: image Result 1)VDD = 2V for power supply. 2)Biasing: The gate-source voltage (V_GS) of each transistor is set to 0.4V, with the differential pair's tail current adjusted to ensure proper saturation. 3)Input Voltage: The differential input is represented as a small signal Vin , with a DC bias point of 1.1V for the operating voltage.

After performing DC, transient, and frequency response analyses in PSIM, the amplifier shows stable biasing and good amplification of the differential signal with a high voltage gain at low frequencies, while the gain decreases as frequency increases, which is typical for such amplifiers. Inference The amplifier effectively amplifies small differential signals with a stable DC operating point, but its high-frequency response starts to degrade due to the inherent capacitances of the transistors. The extracted small-signal parameters indicate a decent voltage gain and manageable input/output resistances, making it suitable for low-frequency applications with moderate bandwidth.




