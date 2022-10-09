# CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso
### 2-input CMOS XNOR Gate Design and Analysis with Layout using Cadence Virtuoso

---
<!-- Cadence Project (Transient, DC, AC & Noise Response With Layout) -->

I’m really glad to share that, this is my sixth project on __Cadence Virtuoso__. I am designing here a 2-input CMOS XNOR Gate Design by 4 CMOS NOR Gate, with it's Layout using Cadence Virtuoso.

___Before I start explaining my project in details, you should know a few things !___     

### What is CMOS XNOR Gate?  
The XNOR gate ( Exclusive NOR ) is a digital logic gate whose function is the logical complement of the Exclusive OR (XOR) gate. It is equivalent to the logical connective from mathematical logic, also known as the material biconditional. The two-input version implements logical equality, behaving according to the truth table to the right, and hence the gate is sometimes called an "equivalence gate". A high output (1) results if both of the inputs to the gate are the same. If one but not both inputs are high (1), a low output (0) results.

### The Project details of mine :
Here i have use __gpdk90n__ :-
1. 8T pmos1v and 8T nmos1v.
2. For vdd i have use vdc (1.1v)
3. For input i have use two vpulse (1.1v)
4. Here I am doing four types of Analysis :  
    i ) Transient Response  
    ii ) DC Response  
    iii ) AC Response  
    iv ) Noise Response, Noise Figure & Noise Factor  
    N.B. I'm measuring here 2 inputs & output plots and Current (I) in VDD node.
5. In Layout - Metals Used ( Metal1 ) and Poly Layer
6. The minimum width of metal utilized for routing is 0.12
7. DRC and LVS clean (there are no error)

So I designed a Schematic of the CMOS XNOR Gate, where the whole thing is based on gpdk90n. I have use 8 pmos for 1v and 8 nmos for 1v. I also designed a symbol of it, so that i can utilise that for further schematic creation.  

The below figure shows a 2-input CMOS XNOR Gate. For Designing a XNOR Gate i have use to 4 NOR Gate.

Considering all steps will show that Vout is following the expected value as in 2-input XNOR Gate Truth Table.

![Scametic_gif](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/Scametic.gif?raw=true)
![Scametic](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/Scametic.PNG?raw=true)
![Symbol](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/Symbol.PNG?raw=true)
![Symbol_Scametic](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/Symbol_Scametic.PNG?raw=true)

#### DC, AC, Transient :
_Here I am doing four types of Analysis - DC, AC, Transient and Noise_.  
In DC and Transient Analysis i have measured Va, Vb & Vout as Voltage, and Current (I) in VDD node. In AC Analysis i have measured Va, Vb & Vout as Voltage Frequency and Current (I) Frequency in VDD node. For DC and Transient Analysis the plots of _Va_ , _Vb_ and _Vout_ shows the _voltages_, on the otherhand _VDD(I4)_ shows the _current (I)_. For AC Analysis the plots of _Va_ , _Vb_ and _Vout_ shows the _voltage frequency_, on the otherhand _VDD(I4)_ shows the _current (I) frequency_. 
![output](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/Output.PNG?raw=true)  
![output2](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/Output_2.PNG?raw=true)

#### Noise Response, Noise Figure and Noise Factor :  
For measuring of Noise Response, Noise Figure and Noise Factor i had to use PORTS instead of Vpulse. For Noise Analysis i have measured input, output & VN2 noise and also Noise Figure. In Noise Response the plots shows the input, output & VN2 noise and also Noise Figure.  
![noise_figure_scametic](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/Noise%20Analysis_Scametic.PNG?raw=true)
![noise_output](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/Noise_Output(IN.OUT,Noise%20Figure,Noise%20Factor).PNG?raw=true)
![noise_output_2](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/Noise_Output(IN.OUT,Noise%20Figure,Noise%20Factor)_2.PNG?raw=true)

#### Layout :
In Layout i have use  Metal1 and Poly Layer. I have use here X & Y snap spacing is 0.01m and also the minimum width of metal utilized for routing is 0.12.  
![Layout_gif](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/Layout.gif?raw=true)
![Layout](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/Layout.PNG?raw=true)

#### Design Rule Check (DRC)  
DRC is clean. There are no error in DRC.
![DRC](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/DRC%20Check.PNG?raw=true)  

#### Layout Versus Schematic (LVS)  
LVS is clean. There are no error in LVS.  
![LVS](https://github.com/wreasin/CMOS-XNOR-Gate-Design-using-Cadence-Virtuoso/blob/main/image/LVS%20Check.jpg?raw=true)
