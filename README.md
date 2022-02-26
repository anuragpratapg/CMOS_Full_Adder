# 28T Conventional CMOS Full Adder design
   This repository presents the detailed documentation on designing of Conventional CMOS Full Adder on 28nm CMOS Technology by using Synopsis Custom Compiler.
# Table of Contents
     - Abstract
     - Introduction
     - Reference Circuit
     - Reference Waveform
     - Tools used
     - Schematic in Synopsys Custom Compiler
             - Carry Block
             - Sum Block
             - Top level Full adder 
             - Input pulses for Inputs A,B and C
      - Output Waveform
      - Netlist
      - Calculation of Propagation delay and Power Consumption
      - Conclusions
      - Author
      - Acknowledgement
      - References
  
 #  Abstract
    This paper represents 28T conventional full adder design using standard CMOS design. This design is implemented on technology 28 nm using Synopsis tool. The analysis is    carried out using several parameters like power consumption, delay and power delay product on various supply voltages. Full adders are the important components in application such as Digital signal processor, microcontroller, processor and data processing units.
Keywords— Full Adder, Technology, CMOS, Synopsys

 #  Introduction
    Designing of low-power and high speed Very Large-Scale Integration (VLSI) systems has pop up as highly demands in market due to fast-paced growing technologies in telecommunication and other power applications. Binary addition is the basic components found in most arithmetic and logic components. Hence the realization of Half adder and Full adder nowadays is essential in terms of delay and power consumption.
    Full adder is designed for addition of two bits (A and B) with input carry C in such a way that can take eight inputs together from ‘000’ to ‘111’ and produces two one-bit output i.e. sum and carry out.
Equations of full adder based on the truth table-
SUM = A  (B  C) 
COUT = AB + BC + AC OR 
COUT = C (A ⊕ B) + AB
    
    ![image](https://user-images.githubusercontent.com/18648566/155855026-08b52406-acd0-4aa8-8270-00cd5e3a2f09.png)
     Fig1: Block Diagram and Truth Table of Full Adder
 The advantages of complementary CMOS logic circuit based full adder design are its layout regularity and stability at low voltage due to the complementary transistor pairs.
 
 #  Reference Circuit
    The Fig2 shows the schematic of 28T conventional CMOS design Full Adder. This design is based on complementary pull up and pull down topologies and having high noise margin and reliability. The CMOS full adder suffers from large power consumption and high delay. We will also calculate average power consumption by the above circuit.
    
 #  Reference Waveform
    This section presents simulation of reference waveform as shown in below Fig3. Conventional CMOS full adder considered in this work are simulated for getting proper outputs along with estimation of propagation delay and average power consumption.
    
 #  Tools used
 #  Schematic in Synopsys Custom Compiler
 #  Carry Block
 #  Sum Block
 #  Top level Full adder 
 #  Input voltage pulses for Inputs A,B and C
 #  Output Waveform
 #  Netlist
 #  Calculation of Propagation delay and Power Consumption
 #  Conclusions
 #  Author
    Anurag Pratap Singh
    Bangalore- 560100
    
 #  Acknowledgement
    1. Cloud based Analog IC Design Hackathon
    2. IIT, Hyderabad
    3. Synopsys India
    4. VLSI System Design Pvt Ltd, India
    5. Especial Thanks to Kunal Ghosh(Co-founder of VSD pvt ltd), Chinmaya Panda (IIT, Hyderabad), Sameer Durgoji and his colleagues.
 #  References
    1. Omid Kavehei, Mostafa Rahimi Azghadi, Keivan Navi and Amir-Pasha Mirbaha, Design of Robust and HighPerformance 1-Bit CMOS Full Adder, IEEE Computer Society Annual Symposium on VLSI.
    2. CH. Haritha, L. Sarika, “Design of CMOS Full Adder Cells for Arithmetic Applications”, International Journal of Engineering Research & Technology (IJERT) Vol. 2 Issue 9, September–2013
    3. S. Wairya, Himanshu Pandey, R.K.Nagaria and S. Tiwari, Ultra Low Voltage High Speed 1-Bit CMOS Adder, Member, IEEE.

     
