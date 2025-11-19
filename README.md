# -Amplitude-Modulation-and-Demodulation-using-NumPy-and-Matplotlib

__Aim__: 

To implement and analyze amplitude modulation (AM) using Python's NumPy and Matplotlib libraries. 

__Apparatus Required__: 

Software: Python with NumPy and Matplotlib libraries 
Hardware: Personal Computer 

__Theory__: 

Amplitude Modulation (AM) is a technique used in electronic communication, primarily for transmitting 
information via a radio carrier wave. In AM, the amplitude of the carrier wave is varied in proportion to that of 
the message signal. The general form of an AM signal is: 


__Algorithm__:
1. Initialize Parameters: Set the values for carrier frequency, message frequency, and sampling frequency. 
2. Generate Time Axis: Create a time vector for the signal duration. 
3. Generate Message Signal: Define the message signal as a cosine wave. 
4. Generate Carrier Signal: Define the carrier signal as a cosine wave. 
5. Modulate Signal: Apply the AM formula to obtain the modulated signal. 
6. Plot the Signals: Use Matplotlib to plot the message signal, carrier signal, and modulated signal.

__Program__:
import numpy as np

import matplotlib.pyplot as plt

Am = 5.3

Ac = 10.6

fm = 424

fc = 4240

fs = 42400

t = np.arange(0, 3/fm, 1/fs)

m = Am * np.cos(2 * np.pi * fm * t)

c = Ac * np.cos(2 * np.pi * fc * t)

s = (Ac + m) * np.cos(2 * np.pi * fc * t)

plt.figure(figsize=(10, 6))

plt.subplot(3,1,1)

plt.plot(t, m)

plt.xlabel("Time")

plt.ylabel("Amplitude")

plt.grid()

plt.subplot(3,1,2)

plt.plot(t, c)

plt.xlabel("Time")

plt.ylabel("Amplitude")

plt.grid()

plt.subplot(3,1,3)

plt.plot(t, s)

plt.xlabel("Time")

plt.ylabel("Amplitude")

plt.grid()

plt.tight_layout()

plt.show()


__Tabulation__:

![WhatsApp Image 2025-11-19 at 10 21 38_a8aab1a5](https://github.com/user-attachments/assets/bf3c624b-b3cd-41b8-92da-71dc3dc81c21)


 __Output__:

<img width="1238" height="738" alt="image" src="https://github.com/user-attachments/assets/a0372b65-00a8-492f-b8e9-1685c93a8b69" />


 __Result__:

The message signal, carrier signal, and amplitude modulated (AM) signal will be displayed in separate plots. Thus AM is implemented using numPy and Matplotlib.
