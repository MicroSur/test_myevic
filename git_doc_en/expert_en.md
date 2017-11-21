### Expert Menu

Settings that require understanding of what, why and when they need to change. 
Be responsible for the consequences only to yourself.
The designation of icons in this menu: 

* __BVO__

Menu battery voltage. 
It is recommended to calibrate the readings before using fashion software charge control (all the many battery mods and Pico 25).

Depending on the fashion model and the characteristics of the scheme, measured mod the voltage of batteries may differ from the actual.
This can lead to incorrect results when working: 
 - mod can ahead of time to block the guy, when the battery still has a charge;
- can be retriggered during the actual drawdown of the batteries (odnobatareynogo fashion), without knowing the exact condition of the battery;
- can try to continue to charge the battery when it is fully charged (only in mod software charge control);

Fully charge the batteries in an external charger. Using multimeter, perform measurements of stresses on banks. 
Insert the batteries in the box and make adjustments if required. 
 For mods with built in batteries is difficult to know their actual tension, without opening fashion.
At the discharge accum, their testimonies may float relative to each other, there's nothing you can do about it.

Limits of adjustment in each of the installed accum +-1.00 Volts with a step of 10 mV. 

* __X32__

He's LXT, 32768 Hz oscillator.
To enable or disable support for this exact generator. 
For some pukavik boxes with hardware clock shutdown this generator saved from the Frisians. 
 If the box cannot use this crystal for real time clock, this setting will turn off and mode Light sleep (LSL). 
*This option is useless and off if the box is physically absent this generator.* 

* __LSL__

Mode light sleep. 
*This mode is useless and is off by default, if the box has support for X32 generator. And is enabled by default, if no support.* 
 In this mode, the real time clock will always be fairly accurate HIRC oscillator ( 12 MHz ) is not accurate internal oscillator LIRC (10 kHz), not in sleep mod or not. 
Adjusts the rate of the clock (Speed) this mode is not required. But the consumption will grow by about 50 mAh per day. 
The precision in this mode is comparable to the accuracy in the boxes with embedded clock (LXT generator). But the clock reset when removing the batteries as there is no backup power on the Board.

* __SHR__

Adjustment of shunt 
 *Warning: Improper installation of the item means for the life of your box. Can cause excess current through the atomizer and fading. 
The shunt is used in the circuit to calculate (via the voltage) of current, resistance and power the atomizer. 
The program indicates the resistance of the shunt and in this paragraph you can change it. This makes for a more precise fit of the calculated resistance of the atomizer.
Readings on the screen at the same time - current resistance of the atomizer. Do not change this parameter strongly and only when absolutely necessary. 
 To reset the shunt default for this mod is a long holding the start button (2s).

* __UCH__

Charging via USB. 
*Only for mnogoserijnyj mods and Pico 25.* 
Enables/disables the possibility of charging fashion USB.
Odnobatareynogo fashion are separate from the General pattern of exercises on the Board and not allow her the control. 
USB continues to work in normal mode for flashing, monitoring, etc. 
Recommended adjustment BVO before charging fashion USB. 

* __BAT__

Model battery (battery profile). 
 The firmware converts the battery voltage into a percentage. For how this is done and meets this setting.
There are several predefined types of conversion for different batteries: 25R, 30Q, HG2, HE4, VTC4, VTC5, VTC6. They are more accurate than GEN and to set the current limit for each (according to the test results Mooch).
"GEN" is a universal battery, the default from the manufacturer fashion. Use it in the pits with built-in accum.

Custom battery (CUS): 
 It's a special battery, the values of conversion for which you can change directly into fashion, the menu CUS. By default, the indications of interest correspond to level of battery while hovering about 30 Watts. 


* __USB__

The default mode HID this is the main mode and always works, for PC communication, firmware or monitoring.
An additional mode for USB COM. The interface creates a virtual COM port to use a terminal program on a PC, mainly for testing purposes of the programmer.

* __Temp__

 Allows you to adjust the readings of the internal temperature sensor boards closer to the real.
Let fashion sleep (cool down) around the home thermometer temperature in the room. Then quickly set this value on fashion.

* __CUS__

Change menu of the translation table of the voltage of the battery (always used the ACC with the lowest voltage) to the indications in percent for the custom batteries.
The default corresponds to the current readings of the battery 18650 at the soaring to 30 Watts. In this case the interest will be more realistically reflect the capability of the battery at this capacity.
 0% and 100% immutable, they must be the same always. Other interest and all voltages can be changed in the direction of increasing from the previous value.
After checking the validity table will be written into the nonvolatile parameters memory (dataflash).

* __MAX__

This menu allows you to set the maximum allowable values for:
- power to the atomizer
- the voltage at the atomizer
- charging current for USB (for mods where the management charge is)
- PCB temperature

-----

← Previous page: [interface Menu](interface_en.md) -- Next page: [How to compile](howtobuild_en.md)→
