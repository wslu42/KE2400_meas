# KE2400_meas

This code provides quick IVc measurement and visualization with Keithley 2400 (KE2400) via QCoDeS vi control protocol and Pandas data collection. One example of hardware connection is using laptop to communicate through GPIB-USB adapter currently attached to the rear panel of KE2400. Please follow below step for software confuguration:

1. Install driver on laptop for GPIB-USB adapter by downloading NI 488.2, please make sure you select the oldest driver version 17.6 since any newer driver does not support our adapter (the model of our adapter is GPIB-USB-B specifically)
https://www.ni.com/en-us/support/downloads/drivers/download.ni-488-2.html#306147

2. Connect your laptop to the outlet first and then connect GPIB-USB to the laptop. The reason is laptop operating with battery has ground level floated and might cause the GPIB devices malfuntioned or even damaged.

3. Open NI-MAX (Meas. and Autoamation Explorer) which comes along with your LabVIEW installation, and check if you can find GPIB-USB interface under it. Right click on the GPIB-USB interface and click "scan instrument". If you can see Keithley 2400 with GPIB address # 25 then you are good to go to try out the code.

4. Hook up a resistor with known value and see if you can get the nominal resistance, enjoy!

WS 191206
