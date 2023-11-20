# AMSAT_IF100_Interface
Interfacing USB port EASYCOM-II rotor commands to IF100 rotor controller

There are still people using the AMSAT IF100 rotor controller together with Instanttrack.
This is great tracking-software but today there are programs that provide a lot more functions. 
The one I am using is GPREDICT, freeware and available for Windows en Linux.
The IF100 needs to be controlled via a parallel printer port and the software needs direct-access to this port. 
It is hard to find a PC with a printer-port and the latest versions of Windows does not allow direct access to the port.

So I designed a small program that you can run on a Arduino Nano. 
It simulates a Serial-port so you can connect it to Hamlib's ROTCTL (mode 202) for example and generate pulses to drive the IF100.
It accepts EASYCOM-II commands at 9600Bd

73's Danny - ON4ABR
