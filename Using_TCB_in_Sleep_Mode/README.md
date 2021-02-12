[![MCHP](../images/microchip.png)](https://www.microchip.com)

 # Using TCB in Sleep Mode

This program shows how to configure the Timer/Counter Type B (TCB) to operate in sleep mode. The TCB0 is configured to generate an overflow interrupt every second. The interrupt wakes up the device and toggles an LED.

## Related Documentation
More details and code examples on the AVR128DA48 can be found at the following links:
- [TB3214-Getting Started with Timer/Counter Type B (TCB)](https://ww1.microchip.com/downloads/en/Appnotes/TB3214-Getting-Started-with-TCB-90003214A.pdf)
- [AVR128DA48 Product Page](https://www.microchip.com/wwwproducts/en/AVR128DA48)
- [AVR128DA48 Code Examples on GitHub](https://github.com/microchip-pic-avr-examples?q=avr128da48)
- [AVR128DA48 Project Examples in START](https://start.atmel.com/#examples/AVR128DA48CuriosityNano)

## Software Used
- MPLAB® X IDE 5.40 or newer [(microchip.com/mplab/mplab-x-ide)](http://www.microchip.com/mplab/mplab-x-ide)
- MPLAB® XC8 2.30 or a newer compiler [(microchip.com/mplab/compilers)](http://www.microchip.com/mplab/compilers)
- MPLAB® Code Configurator (MCC) 4.0.1 or newer [(microchip.com/mplab/mplab-code-configurator)](https://www.microchip.com/mplab/mplab-code-configurator)
- MPLAB® Code Configurator (MCC) Device Libraries 8-bit AVR® MCUs 2.5.0 or newer [(microchip.com/mplab/mplab-code-configurator)](https://www.microchip.com/mplab/mplab-code-configurator)
- AVR-Dx 1.4.75 or newer Device Pack

## Hardware Used
- AVR128DA48 Curiosity Nano [(DM164151)](https://www.microchip.com/Developmenttools/ProductDetails/DM164151)


## Setup

The AVR128DA48 Curiosity Nano Development Board is used as test platform.

<br><img src="../images/AVR128DA48_CNANO_instructions.PNG" width="500">

The following configurations must be made for this project:

Set the main clock to the Internal Ultra Low Power Oscillator at 32.768 kHz and the prescaler disabled.

TCB0:
- Configured in Periodic Interrupt mode with 1 second period (0x7FFF)
- Run Standby ON and Capture/Time-out Interrupt enabled

The sleep controller is enabled and set to Standby sleep mode

Global interrupts are enabled and TCB0 Interrupt INT option is enabled



 |Pin                       | Configuration      |
 | :---------------------:  | :----------------: |
 | PC6 (LED)                | Digital Output     |

 ## Operation
1.  Connect the board to the PC.

2.  Open the Using_TCB_in_Sleep_Mode.X project in MPLAB® X IDE.

3.  Set the Using_TCB_in_Sleep_Mode.X project as main project. Right click on the project in the **Projects** tab and click **Set as Main Project**.

<br><img src="../images/Set_as_Main_Project.PNG" height="500">

4.  Clean and build the Using_TCB_in_Sleep_Mode.X project. Right click on the **Using_TCB_in_Sleep_Mode.X** project and select **Clean and Build**.

<br><img src="../images/Clean_and_Build.PNG" height="500">

5.  Select the **AVR128DA48 Curiosity Nano** in the Connected Hardware Tool section of the project settings:

- Right click on the project and click **Properties**
- Click on the arrow under the Connected Hardware Tool
- Select the **AVR128DA48 Curiosity Nano** (click on the **SN**), click **Apply** and then click **OK**:

<br><img src="../images/Tool_Selection.PNG" height="400">

6.  Program the project to the board. Right click on the project and click **Make and Program Device**.

<br><img src="../images/Make_and_Program_Device.PNG" height="500">
 
Demo:

 <br><img src="images/demo.PNG">

This image shows the produced waveform on pin PC6 (LED).

 ## Summary

This program shows how to configure the TCB to operate during sleep mode, wakes up the microcontroller and toggles the LED every second.
