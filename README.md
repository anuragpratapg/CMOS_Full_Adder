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
      - Calculation of Propagation delay
      - Conclusions
      - Author
      - Acknowledgement
      - References
  
 #  Abstract
    This paper represents 28T conventional full adder design using standard CMOS design. This design is
    implemented on technology 28nm using Synopsys tool. The analysis is carried out using several parameters 
    like power consumption, delay and power delay product on various supply voltages. Full adders are the important 
    components in application such as Digital signal processor, microcontroller, processor and data processing units.
    Keywords— Full Adder, Technology, CMOS, Synopsys

 #  Introduction
    Designing of low-power and high speed Very Large-Scale Integration (VLSI) systems has pop up as highly demands in market 
    due to fast-paced growing technologies in telecommunication and other power applications. Binary addition is the basic 
    components found in most arithmetic and logic components. Hence the realization of Half adder and Full adder nowadays is 
    essential in terms of delay and power consumption. Full adder is designed for addition of two bits (A and B) with input carry C
    in such a way that can take eight inputs together from ‘000’ to ‘111’ and produces two one-bit output i.e. sum and carry out.
    
    Equations of full adder based on the truth table-
    SUM = A ⊕ (B ⊕ C) 
    COUT = AB + BC + AC OR 
    COUT = C (A ⊕ B) + AB
 
 ![image](https://user-images.githubusercontent.com/18648566/155888675-5adacaa7-41f3-4220-86af-073d04e762b6.png) 
    
                                Fig1: Block Diagram and Truth Table of Full Adder
    The advantages of complementary CMOS logic circuit based full adder design are its layout regularity and stability at low 
    voltage due to the complementary transistor pairs.
    
    A full adder is a digital circuit that performs addition. Full adders are implemented with logic gates in hardware. A full
    adder adds three one-bit binary numbers, two operands and a carry bit. The adder outputs two numbers, a sum and a carry bit. 
    The term is contrasted with a half adder, which adds two binary digits.
    A full adder takes two binary numbers plus a carry or overflow bit. The output is a sum and another carry bit. Full adders 
    are made from XOR, AND and OR gates in hardware. Full adders are commonly connected to each other to add bits to an arbitrary
    length of bits, such as 32 or 64 bits. A full adder is effectively two half adders, an XOR and an AND gate, connected by OR gate.
    
 #  Reference Circuit
    The Fig2 shows the schematic of 28T conventional CMOS design Full Adder. This design is based on complementary pull up and pull
    down topologies and having high noise margin and reliability. The CMOS full adder suffers from large power consumption and high 
    delay. 
    
   ![image](https://user-images.githubusercontent.com/18648566/155890043-a9cbd59c-58f2-472e-adeb-ab935804ea2e.png)
    
 #  Reference Waveform
    This section presents simulation of reference waveform as shown in below Fig3. Conventional CMOS full adder considered in this work
    are simulated for getting proper outputs along with estimation of propagation delay and average power consumption.
    
   ![image](https://user-images.githubusercontent.com/18648566/155890092-5abbae84-a28e-47e7-b8e0-ac6121cb6440.png)
    
 #  Tools used
    - Synopsys Custom Compiler: 
      The Synopsys Custom Compiler design environment includes features for mixed-signal design entry, design debug, 
    simulation management, analysis, and reporting. The Synopsys Custom Compiler™ design environment is a modern solution for
    full-custom analog, custom digital, and mixed-signal IC design. As the heart of the Synopsys Custom Design Platform, Custom 
    Compiler provides design entry, simulation management and analysis, and custom layout editing features. It delivers industry-leading
    productivity, performance, and ease-of-use while remaining easy to adopt for users of legacy tools.
    
    - Synopsys Primewave:
      PrimeWave Design Environment is a comprehensive and flexible environment for simulation setup and analysis of analog, RF,
      mixed-signal design, custom-digital and memory designs within the Synopsys Custom Design Platform. It delivers a seamless simulation
      experience around all the engines of Synopsys PrimeSim Continuum, with comprehensive analysis, improved productivity, and ease of
      use. PrimeWave Design Environment also offers powerful Tcl-based scripting capability enabling easy regressions across thousands of 
      corners.
      
    - Synopsys 28nm PDK kit:
       The Synopsys 28nm process design kit was used in creation and simulation of below design circuit.
       
 #  Schematic in Synopsys Custom Compiler
 #  Carry Block
    - Schematic of Carry block:
![carry_ou_schematic](https://user-images.githubusercontent.com/18648566/155888755-b55ac35e-5e20-4146-a8e5-dff07f46f716.PNG) 

    - Symbol of Carry block:
 ![carry_out_schematic](https://user-images.githubusercontent.com/18648566/155888812-18e3a456-e573-42c2-a2c5-98c1c6fafdc9.PNG)    

 #  Sum Block
    - Schematic of Sum Block:
![sum_schematic](https://user-images.githubusercontent.com/18648566/155888870-45ae726a-0eca-4777-bbe9-9ecf3c3979e7.PNG)      

    - Symbol of Sum Block:
![sum_symbol](https://user-images.githubusercontent.com/18648566/155888889-4cb1461c-98d2-473e-a021-31327c7d7b44.PNG)     

 #  Top level Full adder 
    - Schematic of Full adder:
 ![top_level_real](https://user-images.githubusercontent.com/18648566/155888922-b19db7cb-09a8-411c-9691-6b14420eacbd.PNG)     

    - Symbol of Full adder:
 ![full_adder_symbol](https://user-images.githubusercontent.com/18648566/155888949-ad5ea190-cd6d-450e-8747-de17f7b7a65c.PNG)     
   
    - Schematic for simulation of Full adder design
  ![top_level](https://user-images.githubusercontent.com/18648566/155888976-07c14035-1f07-4933-a3df-b206ad09b968.PNG)   

 #  Input voltage pulses for Inputs A,B and C
    - Input A:
 ![inputA](https://user-images.githubusercontent.com/18648566/155889006-01ec8bc8-d4c6-41ce-b770-303f4569c614.PNG)  

    - Input B:
 ![inputB](https://user-images.githubusercontent.com/18648566/155889015-5e54573d-f96b-4014-9ada-e30b529f8bac.PNG)   

    - Input C:
 ![inputC](https://user-images.githubusercontent.com/18648566/155889033-7246d40d-4391-4be3-8dbb-586d6689b2cc.PNG)    

 #  Output Waveform
 ![output_wf](https://user-images.githubusercontent.com/18648566/155889076-c4b53eb5-cd0b-41ac-af88-4aa6ed5969b0.PNG)
    

 #  Netlist
    *  Generated for: PrimeSim
*  Design library name: FULL_ADDER
*  Design cell name: sim_fulladder
*  Design view name: schematic


*Custom Compiler Version S-2021.09
*Sun Feb 27 12:14:17 2022

.global gnd!
********************************************************************************
* Library          : FULL_ADDER
* Cell             : carry_out
* View             : schematic
* View Search List : hspice hspiceD schematic spice veriloga
* View Stop List   : hspice hspiceD
********************************************************************************
.subckt carry_out a b c cout coutb gnd_1 vdd
xm51 cout coutb gnd_1 gnd_1 n105 w=0.1u l=0.03u nf=1 m=1
xm43 net2 a gnd_1 gnd_1 n105 w=0.4u l=0.03u nf=1 m=1
xm42 coutb b net2 gnd_1 n105 w=0.4u l=0.03u nf=1 m=1
xm41 net3 b gnd_1 gnd_1 n105 w=0.4u l=0.03u nf=1 m=1
xm40 net3 a gnd_1 gnd_1 n105 w=0.4u l=0.03u nf=1 m=1
xm39 coutb c net3 gnd_1 n105 w=0.4u l=0.03u nf=1 m=1
xm64 cout coutb vdd vdd p105 w=0.2u l=0.03u nf=1 m=1
xm56 net1 a vdd vdd p105 w=0.8u l=0.03u nf=1 m=1
xm55 coutb b net1 vdd p105 w=0.8u l=0.03u nf=1 m=1
xm54 net4 b vdd vdd p105 w=0.8u l=0.03u nf=1 m=1
xm53 net4 a vdd vdd p105 w=0.8u l=0.03u nf=1 m=1
xm52 coutb c net4 vdd p105 w=0.8u l=0.03u nf=1 m=1
.ends carry_out

********************************************************************************
* Library          : FULL_ADDER
* Cell             : sum
* View             : schematic
* View Search List : hspice hspiceD schematic spice veriloga
* View Stop List   : hspice hspiceD
********************************************************************************
.subckt sum a b c coutb gnd_1 sum vdd
xm66 sum net4 gnd_1 gnd_1 n105 w=0.1u l=0.03u nf=1 m=1
xm50 net8 a gnd_1 gnd_1 n105 w=0.3u l=0.03u nf=1 m=1
xm49 net7 b net8 gnd_1 n105 w=0.3u l=0.03u nf=1 m=1
xm48 net4 c net7 gnd_1 n105 w=0.3u l=0.03u nf=1 m=1
xm47 net4 coutb net9 gnd_1 n105 w=0.2u l=0.03u nf=1 m=1
xm46 net9 c gnd_1 gnd_1 n105 w=0.2u l=0.03u nf=1 m=1
xm45 net9 b gnd_1 gnd_1 n105 w=0.2u l=0.03u nf=1 m=1
xm44 net9 a gnd_1 gnd_1 n105 w=0.2u l=0.03u nf=1 m=1
xm65 sum net4 vdd vdd p105 w=0.2u l=0.03u nf=1 m=1
xm63 net5 a vdd vdd p105 w=0.6u l=0.03u nf=1 m=1
xm62 net6 b net5 vdd p105 w=0.6u l=0.03u nf=1 m=1
xm61 net4 c net6 vdd p105 w=0.6u l=0.03u nf=1 m=1
xm60 net10 c vdd vdd p105 w=0.4u l=0.03u nf=1 m=1
xm59 net10 a vdd vdd p105 w=0.4u l=0.03u nf=1 m=1
xm58 net10 b vdd vdd p105 w=0.4u l=0.03u nf=1 m=1
xm57 net4 coutb net10 vdd p105 w=0.4u l=0.03u nf=1 m=1
c3 sum gnd_1 c=2p
.ends sum

********************************************************************************
* Library          : FULL_ADDER
* Cell             : full_adder
* View             : schematic
* View Search List : hspice hspiceD schematic spice veriloga
* View Stop List   : hspice hspiceD
********************************************************************************
.subckt full_adder a b c cout gnd_1 sum vdd
xi0 a b c cout net16 gnd_1 vdd carry_out
xi1 a b c net16 gnd_1 sum vdd sum
.ends full_adder

********************************************************************************
* Library          : FULL_ADDER
* Cell             : sim_fulladder
* View             : schematic
* View Search List : hspice hspiceD schematic spice veriloga
* View Stop List   : hspice hspiceD
********************************************************************************
xi0 a b c cout gnd_1 sum vdd full_adder
v40 gnd_1 gnd! dc=0
v39 vdd gnd_1 dc=1.8
v43 a gnd_1 dc=0 pulse ( 1.8 0 0 10n 10n 5u 10u )
v42 b gnd_1 dc=0 pulse ( 1.8 0 0 10n 10n 10u 20u )
v41 c gnd_1 dc=0 pulse ( 1.8 0 0 10n 10n 20u 40u )
c2 cout gnd_1 c=2p
c1 sum gnd_1 c=2p

.option primesim_remove_probe_prefix = 0
.probe v(*) i(*) level=1

.temp 25

.option primesim_output=wdf

.option parhier = LOCAL

.end

 #  Calculation of Propagation delay 
 #  Conclusions
    The addition of single bit is achieved using 28T full adder. We get desired output waveform of Sum and Carry by 
    applying appropriate input supply.
    
 #  Author
    Anurag Pratap Singh
    Bangalore- 560100
    
 #  Acknowledgement
    1. [Cloud based Analog IC Design Hackathon]{https://hackathoniith.in/}
    2. [IIT, Hyderabad]{https://iith.ac.in/}
    3. [Synopsys India]{https://www.synopsys.com/}
    4. [VLSI System Design Pvt Ltd, India]{https://www.vlsisystemdesign.com/}
    5. Especial Thanks to [Kunal Ghosh]{https://www.linkedin.com/in/kunal-ghosh-vlsisystemdesign-com-28084836/}
       (Co-founder of VSD pvt ltd), Chinmaya Panda (IIT, Hyderabad), Sameer Durgoji and his colleagues.
    
 #  References
    1. Omid Kavehei, Mostafa Rahimi Azghadi, Keivan Navi and Amir-Pasha Mirbaha, Design of Robust and HighPerformance 1-Bit CMOS Full 
    Adder, IEEE Computer Society Annual Symposium on VLSI.
    2. CH. Haritha, L. Sarika, “Design of CMOS Full Adder Cells for Arithmetic Applications”, International Journal of Engineering
    Research & Technology (IJERT) Vol. 2 Issue 9, September–2013
    3. S. Wairya, Himanshu Pandey, R.K.Nagaria and S. Tiwari, Ultra Low Voltage High Speed 1-Bit CMOS Adder, Member, IEEE.

     
