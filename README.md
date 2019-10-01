# Amiga PSU Enclosure for Mean Well RT-50B
A 3d-printable Amiga PSU Enclosure for the Mean Well RT-50B Power Supply

3d-model is created in DesignSpark Mechanical 4.0

<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic1.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic1.jpg" width="303" height="227">
</a>
<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic2.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic2.jpg" width="303" height="227">
</a>
<br />
<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic3.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic3.jpg" width="303" height="227">
</a>
<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic4.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic4.jpg" width="303" height="227">
</a>

***

For 3d-printing scroll further down!

Cabling is taken from an old dead Amiga 500 PSU. Also the power switch is reused and a couple of power resistors is added to put a dummy load to satisfy the minimum load requirements stated in the datasheet for the Mean Well RT-50B PSU.

Attention: Read the <a href="LEGAL_DISCLAIMER.md">Legal Disclaimer</a> before doing any electrical work yourself.

<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic5.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic5.jpg" width="504" height="378">
</a>

***

First strip the two leads on the power switch and attach two terminal blocks. Adjust the cable length and cut the Line lead (brown) and connect to the terminal blocks like in picture. Blue is Neutral (return lead) and green/yellow is GND/Earth. Carefully cut the isolation if needed. Do not cut into the leads themselves.

<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic6.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic6.jpg" width="202" height="151">
</a>
<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic7.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic7.jpg" width="202" height="151">
</a>
<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic8.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic8.jpg" width="151" height="202">
</a>
<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic9.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic9.jpg" width="151" height="202">
</a>

***

Now time to fit the Mean Well RT-50B PSU, but first unscrew the left-front screw and use that screw as in picture. Don't screw it all the way down but rather leave some room for the metal chassi to fit in between for a snug fit.

<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic10.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic10.jpg" width="151" height="202">
</a>
<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic11.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic11.jpg" width="202" height="151">
</a>
<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic12.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic12.jpg" width="303" height="227">
</a>

***

Now secure the PSU with a couple of other suitable screws and then connect and secure the leads.


<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic13.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic13.jpg" width="151" height="202">
</a>
<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic14.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic14.jpg" width="303" height="227">
</a>

***
Plugging the power cord in and turning the power switch on we can verify we got 230V AC input working.

<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic15.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic15.jpg" width="504" height="378">
</a>

***
### Dummy load (optional)

Looking at the datasheet for Mean Well RT-50B we can see that minimum current requirements are specified, this means for the PSU to operate reliably we need to have a minimum draw just above the minimum threshold on each rail. The Amiga almost exclusively use the +5V rail so no problem there but on -12V and +12V we might need to put dummy loads on.

<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic16.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic16.jpg" width="868" height="166">
</a>

***

However, Checking another Mean Well datasheet says differently. Hmm maybe newer versions of the PSU doesn't need it?

<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic17.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic17.jpg" width="868" height="166">
</a>

***

Anyway, I will show how to do this dummy load config for those who might need it.

To get the minimum 0.2A on +12V and 0.1 on -12V we can use Power Resistors that will be connected to Common Signal GND. The draw will dissipate as heat so good to place them near a heatsink and ventilation if possible.

Let's calculate Ohm and Wattage to pick suitable resistors. This can easily be done manually or by using a online-calculator like this one: https://www.rapidtables.com/calc/electric/watt-volt-amp-calculator.html




We see that using a 100 Ohm, 3 watt capable resistor is perfect for the -12V rail dummy load and a 47 Ohm, 5 watt capable resistor is suitable for the 12V.

<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic18.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic18.jpg" width="305" height="210">
</a>
<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic19.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic19.jpg" width="305" height="210">
</a>
<br />
<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic20.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic20.jpg" width="504" height="378">
</a>

Verifying theory with practice IRL:

Checking the Currents (Amps)...Shows 120mA and 250mA, just as excpected! I put some shrink tube on the resistors legs for safety reasons.

<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic21.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic21.jpg" width="202" height="151">
</a>
<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic22.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic22.jpg" width="202" height="151">
</a>
<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic23.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic23.jpg" width="202" height="151">
</a>

***

Now let's check voltages:

<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic24.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic24.jpg" width="202" height="151">
</a>
<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic25.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic25.jpg" width="202" height="151">
</a>
<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic26.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic26.jpg" width="202" height="151">
</a>

***

And wire it up:


<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic27.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic27.jpg" width="504" height="378">
</a>
<br />
<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic28.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic28.jpg" width="202" height="151">
</a>
And verify pinout
<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic29.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic29.jpg" width="202" height="151">
</a>
<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic30.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic30.jpg" width="202" height="151">
</a>
<a href="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic31.jpg">
<img src="images/Amiga_PSU_enclosure_for_Mean_Well_RT-50B_pic31.jpg" width="202" height="151">
</a>

