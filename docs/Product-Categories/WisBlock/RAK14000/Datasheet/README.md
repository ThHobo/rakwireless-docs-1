---
prev: ../Overview/
next: false
tags:
  - datasheet
  - wisblock
---

# RAK14000 E-Ink Display Module Datasheet

## Overview

<!-- <rk-img
  src="/assets/images/wisblock/rak14000/overview/RAK14000_illustrated.png"
  width="70%"
  caption="RAK14000 E-Ink Display Module"
/> -->
### Description

The **RAK14000 WisBlock E-Ink Display Module** is designed to be part of a production-ready IoT solution in a modular way and must be combined with a WisBlock Core and a Base module.

The **RAK14000** module provides an interface to connect an E-Ink Display, which is known to be an extremely power-efficient display. It also allows you to connect a Three-Button Module, which can be used on a different application. All of this can be controlled through a WisBlock Core. 

### Features 

*   Input Voltage: 3.3&nbsp;V
*   Display Size: 2.9 inches
*   Wide Viewing Angles, with display Resolution of 296 x 128 pixels
*   Pure Reflective Mode. Very viewable displays!  
*   On-chip display RAM and oscillator
*   Extremely Low Power Consumption! Perfect for power-conscious applications.  
*   Comes with a 3-Button Module. Application can be customized.
*   Uses FPC (Flexible PCB) for its Display and Button modules

## Specifications

### Overview

#### Mounting

The **RAK14000 E-Ink Display Module** is mounted to the IO Slot of a WisBlock Base Board. Figure 1 shows the mounting mechanism of the RAK14000 on a WisBlock Base, such as the RAK5005-O.  

<rk-img
  src="/assets/images/wisblock/rak14000/datasheet/RAK14000-mounting.png"
  width="50%"
  caption="RAK14000 Module Mounting"
/>
  
### Hardware

The hardware specification covers the pinouts of the board and its functionalities and diagrams. It also presents the parameters and their standard values.

#### Pin Definition

The **RAK14000 WisBlock E-Ink Display Module** comprises a standard WisIO connector. The WisIO connector allows the RAK14000 module to be mounted on a WisBlock baseboard, such as RAK5005-O. The pin order of the connector and the pinout definition is shown in Figure 2.

<rk-img
  src="/assets/images/wisblock/rak14000/datasheet/rak14000-pins.png"
  width="60%"
  caption="RAK14000 Module Pinout"
/>  

| Pin Number | Pin Name  |   Description   | Pin Number |  Pin Name  |          Description          |
| :--------: | :-------: | :-------------: | :--------: | :--------: | :---------------------------: |
|     2      |    NC     |  Not Connected  |     1      |     NC     |         Not Connected         |
|     4      |    GND    |     Ground      |     3      |    GND     |            Ground             |
|     6      |    3v3    |      3.3V       |     5      |     NC     |         Not Connected         |
|     8      |    NC     |  Not Connected  |     7      |     NC     |         Not Connected         |
|     10     |    NC     |  Not Connected  |     9      |     NC     |         Not Connected         |
|     12     |    NC     |  Not Connected  |     11     |     NC     |         Not Connected         |
|     14     |    NC     |  Not Connected  |     13     | EINK_RESET | EPD Reset signal. Active Low. |
|     16     |    NC     |  Not Connected  |     15     |     NC     |         Not Connected         |
|     18     |    NC     |  Not Connected  |     17     |     NC     |         Not Connected         |
|     20     |    NC     |  Not Connected  |     19     |     NC     |         Not Connected         |
|     22     |    NC     |  Not Connected  |     21     |     NC     |         Not Connected         |
|     24     |    NC     |  Not Connected  |     23     |     NC     |         Not Connected         |
|     26     | EINK_CSK  |  Serial Clock   |     25     |  EINK_CS   |   Chip select. Active Low.    |
|     28     | EINK_SDIN |   Serial Data   |     27     | EINK_SDIN  |          Serial Data          |
|     30     |    NC     |  Not Connected  |     29     |    D/C#    |     Data /Command control     |
|     32     | EINK_BUSY |   Busy state    |     31     |     S1     |        Button Signal 1        |
|     34     |    NC     |  Not Connected  |     33     |     NC     |         Not Connected         |
|     36     |    NC     |  Not Connected  |     35     |     NC     |         Not Connected         |
|     38     |    S3     | Button Signal 3 |     37     |     S2     |        Button Signal 2        |
|     40     |    GND    |     Ground      |     39     |    GND     |            Ground             |

:::tip 📝 NOTE:
SPI_CS, SPI_MISO, SPI_MOSI, SPI_CLK, IO1, IO3-IO7 are connected to WisIO connector.
:::
  
#### Electrical Characteristics  
  
##### DC Characteristics    
  
The following specifications apply for: VSS = 0V, VCI = 3.0&nbsp;V, TOPR = 25&nbsp;ºC
  
| Symbol           | Description               | Min. | Nom. | Max. | Unit |
| ---------------- | ------------------------- | ---- | ---- | ---- | ---- |
| V<sub>CI</sub>   | Logic supply voltage      | 2.2  | 3.0  | 3.7  | V    |
| V<sub>DD</sub>   | Core logic voltage        | 1.7  | 1.8  | 1.9  | V    |
| I<sub>slp</sub>  | Sleep mode current        | -    | 20   | -    | µA   |
| I<sub>dslp</sub> | Deep sleep mode current   | -    | 1    | 5    | µA   |
| I<sub>opr</sub>  | Typical operating current | -    | 4.3  | 4.5  | mA   |
  
#### Mechanical Characteristics  
  
 
Figure 3 shows the dimensions and mechanical drawing of the RAK14000 module.  
  
<rk-img
  src="/assets/images/wisblock/rak14000/datasheet/rak14000-dimensions.png"
  width="60%"
  caption="RAK14000 Module Mechanical Characteristics"
/>  

#### Schematic Diagram

Figure 4 shows the schematic diagram of WisIO connector:
  
<rk-img
  src="/assets/images/wisblock/rak14000/datasheet/rak14000-wisio.png"
  width="40%"
  caption="RAK14000 WisIO Connection Schematic"
/>


Figure 5 shows the E-Ink Display Connector Schematic:  
  
<rk-img
  src="/assets/images/wisblock/rak14000/datasheet/rak14000-sch1.png"
  width="60%"
  caption="RAK14000 E-Ink Display Connection Schematic"
/> 

Figure 6 shows the E-Ink Display Driver Schematic:  
  
<rk-img
  src="/assets/images/wisblock/rak14000/datasheet/rak14000-sch2.png"
  width="60%"
  caption="RAK14000 E-Ink Display Driver Schematic"
/> 

Figure 7 shows the Three-Button Module Schematic, connected through FPC (Flexible PCB) cable:  
  
<rk-img
  src="/assets/images/wisblock/rak14000/datasheet/rak14000-sch3.png"
  width="60%"
  caption="RAK14000 Three-Button Module Schematic"
/> 
  

