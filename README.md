# Signal-Generator-OrCAD
# Outlines
I designed a signal generator that provides a rectangular signal of variable amplitude {4V, 7V}, and a triangular signal of 4V amplitude. The frequency of the signal should range between [2400; 9100][Hz], the power supply has the amplitudes [-15;+15] [V] and the load resitance has a value of 10[Ω].
# Implementation
A Block diagram would contain a Rectangular Wave Generator (an Op-Amp multivibrator, or a positive feedback comparator), then a Triangular Wave Generator (an Integrator, or an active low pass filter, fed with the square wave from the predecessor) and then a Frequency Adjuster (structure based on a potentiometer and a resistor). The signal will pass then through an Amplitude Adjustemnt block to achieve either 4V or 7V. Finnaly, since the OpAMp can't provide such a large current (400mA-700mA), the signal has to be amplified before reaching the load (Class AB Power Amplifier).    
