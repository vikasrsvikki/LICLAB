CURRENT MIRRORING EXPERIMENT

Introduction 

A current mirror is a circut designed to duplicate a current from one branch of a circut to another. it is often usde in analog design to provide a stable reference current that can be replicate through various part of the circut , typically in differential amplifier or other type of active circut current mirror are widly used due to their high output resistence , improved accuracy , and ability to maintain constant independent of voltage variation . the experiment involve simulating different currnt mirror circut ,such as basic current mirrors , ans cascade current mirrors to analyse their performence , current transfer accuracy , the voltage dependencies , by understanding their circuits , enginnners can design efficient current source and biasing networks for various analog and mixed-signal application

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









