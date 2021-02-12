[![MCHP](images/microchip.png)](https://www.microchip.com)

# Getting Started with Timer/Counter Type B (TCB) Examples (MPLAB® X)

This repository contains examples of MCC-generated source code for Timer/Counter Type B (TCB), as described in [TB3214-Getting Started with Timer/Counter Type B (TCB)](https://ww1.microchip.com/downloads/en/Appnotes/TB3214-Getting-Started-with-TCB-90003214A.pdf) document from Microchip. The repository contains three MPLAB® X projects inside:

* [<strong>Using TCB in 8-bit PWM Mode:</strong>](Using_TCB_in_8-bit_PWM_Mode) This use case shows how to configure the TCB to produce a PWM signal with a 1 second period (for more details, see [<strong>Using TCB in 8-bit PWM Mode</strong>](Using_TCB_in_8-bit_PWM_Mode)).
* [<strong>Using TCB in Sleep Mode:</strong>](Using_TCB_in_Sleep_Mode) This use case shows how to configure the TCB to operate during sleep and periodically wake up the device and toggle an LED (for more details, see [<strong>Using TCB in Sleep Mode</strong>](Using_TCB_in_Sleep_Mode)).
* [<strong>Using TCB in Time-out Check Mode:</strong>](Using_TCB_in_Time-out_Check_Mode) This use case shows how to configure the TCB to toggle an LED if the input signal is longer than the time-out period (for more details, see [<strong>Using TCB in Time-out Check Mode</strong>](Using_TCB_in_Time-out_Check_Mode)).

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
- MPLAB® Code Configurator (MCC) Device Libraries 8-bit AVR MCUs 2.5.0 or newer [(microchip.com/mplab/mplab-code-configurator)](https://www.microchip.com/mplab/mplab-code-configurator)
- AVR-Dx 1.4.75 or newer Device Pack


## Hardware Used
- AVR128DA48 Curiosity Nano [(DM164151)](https://www.microchip.com/Developmenttools/ProductDetails/DM164151)
