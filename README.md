# PLC_3_pump_sequencing
3-Pump Sequencing cf. https://www.plctalk.net/qanda/showthread.php?t=82543

Ladder logic implementation of three vacuum pumps, in a lead-lag1-lag2 configuration,
automatically attempting to maintain a minimum vacuum level against a load using two vacuum sensors.

Lead, lag1 and lag2 designation will vary, when pumps are in Automatic mode, to attempt to even out accumulated runtime across all pumps.
Each pump can be placed into Manual mode to run continuously, or into Maintenance mode to prevent running;
remaining pumps in Automatic mode will continue to turn on and off to control vacuum,
and lead-lag1-lag2 designations will continue to vary to balance runtime.

Code is configured for RSLogix™ 500/RSLogix™ Micro Starter Lite software and MicroLogix 1100 Series B; it may be possible to use it in other similar PLCs (SLC 5/xx; PLC-5)

