# Oscilloscope Guide
<br> Prepared by Christopher Gardner, B.E.E. Candidate (Expected 2028) <br> <br>
One of the most important tools used by electrical and computer engineers is the oscilloscope. An oscilloscope measures voltage over time, allowing us to see electrical signals that would otherwise be impossible to observe. Digital oscilloscopes can also perform measurements like frequency (how often a signal repeats) and voltage calculations. This guide will cover the basic operation of a oscilloscope and how to use it to make simple measurements. Advanced topics such as sampling rate, bandwidth, input impedance, and transient analysis are NOT covered in this guide.

Oscilloscopes come in two main types: analog and digital. While analog oscilloscopes are still used in some specialized applications, digital oscilloscopes are the standard in most classrooms, laboratories, and industry because they can store measurements and act as advanced calculators. Since our laboratory uses digital oscilloscopes, this guide will focus entirely on their operation.

## Safety
1. Always connect the probe's ground clip to the circuit ground before taking measurements.
2. Ask instructor before placing probe connections if you're unsure.

## Basics
The purpose of the oscilloscope is to display voltage as it changes over time, for accuracy of reading there are many controls that dominant the face of the machine. The tool is then designed to see frequency of a signal (how often does it repeat), if a component is causing incorrect behavior (signal isn't what we designed around), and whether the signal is DC or AC.
<br>
#### Terminology
##### Note: Some of these ideas become much more important in college-level engineering. For now, focus on the basic definitions rather than the mathematics behind them.

1. Channel: a BNC port used to connect to probes, each channel is seen as a different color in the interface. (Below)
<img width="300" height="450" alt="BNC Port on Oscilloscope" src="Images/BNC_PORT.png" />

2. Vpp: Peak to peak voltage; what this means is we measure the voltage of a AC wave from the very bottom to the very top and find the _absolute_ value (absolute is the same as magnitude; think of it as making all parts of the number positive) of the voltage.
<img width="300" height="450" alt="Vpp Example" src="Images/Vpp.png" />

3. Frequency: Frequency tells us how many times a signal repeats every second. It is measured in hertz (Hz). For those adept in math, frequency is defined as being solved by doing <br>_f_=1/T<br> (T corresponds to the period); note that this math begins to enter euler's mathematics so don't worry about understanding the math just the simplified definition.
<img width="300" height="450" alt="Frequency graph" src="Images/Freq.jpg" />

4. Vmax: The top peak of a signal, representing the maximum positive value a signal hits.
<img width="300" height="450" alt="Vmax graph" src="Images/Vmax.png" />

5. Period: How long it takes for a signal to repeat its shape. For those adept in math, it is the reciprocal of the frequency calculation:<br> T=1/_f_ <br>(_f_ is the frequency).
<img width="400" height="450" alt="Period graph" src="Images/period.png" />


## Getting your first waveform
1. First switch on the scope (right image), connect your probe to the BNC port (whatever channel you'd like, the scope will detect whichever you use), and power on your circuit.
<p float="left">
<img width="350" height="350" alt="Probe" src="Images/Probe_Outline.png" />
<img width="350" height="350" alt="Power Button" src="Images/power.png" />
</p>

2. Connect the Grounding clip (above) to a common ground pin on the circuit; connect the Measuring Clip to the point you'd like to measure by pulling the retractable grey shielding back on the tip to expose the hook.

3. Press the 'start/stop' button on the top right on the oscillscope, you should see a signal on the screen appear like below (the line might look different).  If not call over a instructor for troubleshooting.
<img width="350" height="350" alt="Oscilloscope screen" src="Images/Example.png" />

4. Gather data you need to by navigating the side measurement tools. Press button next to each tool for use.

## Vertical and Horizontal Controls
### Vertical
1. There is a section on the control pannel that says 'Vertical', increasing the scale makes the waveform appear smaller, while decreasing it makes the waveform appear larger.
<img width="350" height="350" alt="Oscilloscope screen" src="Images/Vert_contr.jpg" />

2. To zero your inputs press in on the button, the dial will _scale_ our signal--till you hit the scopes limits--as desired

### Horizontal
1. There is a section on the control pannel that says 'Horizontal', these tools adjust the zoom and also the scale of capture we look at.
<img width="350" height="350" alt="Oscilloscope screen" src="Images/Hor_cont.jpg" />

2. To zero your inputs press in on the button, the dial will _scale_ our signal--till you hit the scopes limits--as desired

## Types of signals and their meanings
We have many types of signals that are used for different purposes such as power, communication, and other uses. To understand each signal we have we must remember the structure of voltage over time used in the oscillscope. <br>
<img width="400" height="450" alt="UI of oscilloscope" src="Images/screenshot.png" />

**1. Noise:** Noise is unwanted electrical signals that are added to the waveform. It can come from nearby electronics, power lines, radio signals, or the circuit itself.
<br>**Fun Fact:** This is what TV static is seen on the right (if your old enough to know what that is)
<br><p float="left">
<img width="400" height="450" alt="UI of oscilloscope" src="Images/Noise.png" />
<img width="400" height="450" alt="UI of oscilloscope" src="Images/static.png" />
</p>

**2. Square Wave:** A common wave used for communication and testing of equipment.
<br><br><img width="400" height="450" alt="UI of oscilloscope" src="Images/square_wave.png" />

**3. Sine Wave:** A sine wave is one of the most common waveforms you'll encounter. Household AC power is a sine wave.
<br><br><img width="400" height="450" alt="UI of oscilloscope" src="Images/sine_wave.png" />

**4. Sawtooth Wave:** Used in automobiles and control systems. This wave is not commonly used.
<br><br><img width="400" height="450" alt="UI of oscilloscope" src="Images/sawtooth_wave.png" />


## Basics of Triggering
Triggering tells the oscilloscope when to begin drawing the waveform. A good trigger makes the waveform appear steady instead of moving across the screen.



## Sources
- https://learn.sparkfun.com/tutorials/how-to-use-an-oscilloscope/all
- https://www.tek.com/en/documents/primer/oscilloscope-basics

# Image Credits
- https://www.alibaba.com/product-detail/Siglent-The-Oscilloscope-SDS1104x-u-Features_1601418064600.html
- https://shopdelta.eu/peak-to-peak-voltage-vpp_l2_aid796.html
- https://www.weschler.com/blog/line-frequency-measurements/
- http://musicweb.ucsd.edu/~trsmyth/sinusoids171/Waveform_period.html
- https://linhkienviet.vn/may-hien-song-hantek-dso5072p-2-kenh-70mhz-digital-storage-oscilloscope
- https://www.elexp.com/products/05spak110scope-probe-bnc-ic-sw-60mhz?srsltid=AfmBOopVTEC851GlVo0Oszrdn3fSPT5a2GyvUQqfLehnmmQq34nkxUk8
- https://en.wikipedia.org/wiki/White_noise
- https://www.electronics-tutorials.ws/accircuits/sine-wave.html
- https://www.geeksforgeeks.org/python/plotting-a-sawtooth-wave-using-matplotlib/
