# AMBA_APB
AMBA_APB


The AMBA APB (Advanced Peripheral Bus) is a low-power, low-bandwidth bus in the ARM AMBA (Advanced Microcontroller Bus Architecture) family, primarily used for connecting peripheral devices such as timers, UARTs, and GPIOs. It is designed for simplicity and minimal power consumption, making it suitable for peripherals that do not require high-speed communication.

Key Features:
•	Simple interface with minimal control logic.
•	Low power and low bandwidth.
•	Synchronous single-cycle data transfer.
•	Suitable for interfacing slow peripherals.

APB Signal Descriptions:

Signal	   Direction	  Description
PCLK	      Input	      APB clock signal.
PRESETn	    Input	      Active-low reset signal.
PADDR	      Input	      Address bus for peripheral selection.
PSELx	      Input	      Peripheral select signal (one per peripheral).
PENABLE	    Input	      Enables the transfer after address phase.
PWRITE	    Input	      High for write, low for read operation.
PWDATA	    Input	      Write data bus (from master to slave).
PRDATA	    Output	    Read data bus (from slave to master).
PREADY	    Output	    Indicates if the slave is ready.
PSLVERR	    Output	    Indicates an error response from the slave.

