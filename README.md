# AM-USING-PYTHON-
AIM

To generate an amplitude-modulated (AM) signal using Python.

EQUIPMENTS REQUIRED

• Computer with i3 Processor

• Colab

THEORY:
Amplitude Modulation (AM) is a process used in analog communication where the strength (amplitude) of a high-frequency carrier wave is varied in accordance with the instantaneous value of a low-frequency message signal. The main purpose of modulation is to enable the transmission of information signals over long distances without significant loss or distortion.

In AM, the carrier frequency remains constant, but its amplitude changes as per the variations in the message signal. This results in a new waveform that carries the original information within its envelope. The modulated signal occupies a specific range of frequencies around the carrier, known as the bandwidth.

The AM signal contains the carrier and two additional components called sidebands, which carry the actual information. The upper and lower sidebands are symmetrically located around the carrier frequency.

Amplitude Modulation is widely used in radio broadcasting, aircraft communication, and public address systems because of its simplicity and ease of generation and reception. However, it is less efficient in terms of power and bandwidth compared to other modulation techniques like FM and PM.



Algorithm

Start the program.

Set the values for carrier frequency, message frequency, modulation index, sampling rate, and duration.

Generate a time vector for the given duration.

Create the message signal (low-frequency waveform).

Create the carrier signal (high-frequency waveform).

Vary the amplitude of the carrier signal according to the message signal to obtain the AM wave.

Plot the message, carrier, and modulated signals.

Display the results.

Stop the program.

Program
````````
Am=2.9;
fm=184;
Ac=5.8;
fc=1840;
fs=18400;
t=0:1/fs:2/fm;
m=Am*cos(2*3.14*fm*t);
subplot(3,1,1);
plot(t,m);
c=Ac*cos(2*3.14*fc*t);
subplot(3,1,2);
plot(t,c);
s=(Ac+m).*cos(2*3.14*fc*t);
subplot(3,1,3);
plot(t,s);
````````

Output Waveform
<img width="1920" height="1200" alt="Screenshot (98)" src="https://github.com/user-attachments/assets/30fb73af-c294-48aa-a204-2d06146c4170" />
TABULATION:
![WhatsApp Image 2025-10-23 at 22 33 05_5580a556](https://github.com/user-attachments/assets/2ddfdf46-717a-4eae-bca8-04db300de0e3)

Calculation

ma (Theory) = am/ac =0.5

ma(Practical) = (Emax-Emin)/(Emax+Emin) =0.3333

MODEL GRAPH 
<img width="919" height="1290" alt="image" src="https://github.com/user-attachments/assets/2ecdab70-dd2b-4af9-8639-cc02cc8d3ef2" />

RESULT: Thus the amplitude modulation and demodulation is experimentally done and the output is verified.
