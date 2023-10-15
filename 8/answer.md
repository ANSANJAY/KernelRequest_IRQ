How can a device driver know if the interrupt handler was activated by an interrupt generated by the device it manages?
=================================================================================================================

All devices that offer interrupt support have a status register that can be read in the handling routine to see if the interrupt was or was not generated by the device 

Example:  For 8250 serial port, this status register is IIR - Interrupt Information Register