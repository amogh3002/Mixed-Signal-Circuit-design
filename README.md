DESIGN OF DIFFERENT KINDS OF SAMPLE AND HOLD ARCHITECTURES IN 180nm TECHNOLOGY


A Sample and Hold Circuit, sometimes represented as S/H Circuit or S&H Circuit, is usually used with an Analog to Digital Converter to sample the input analog signal and hold the sampled signal.In the S/H Circuit, the analog signal is sampled for a short interval of time, usually in the range of 10 µS to 1 µS.After this, the sampled value is hold until the arrival of next input signal to be sampled.It forms the interface between analog world and the signal processing system- High precision and speed is required.Sampling circuits samples an analog signal and stores the value in a memory element until next sampling instant.Operation is periodic and it is stored in the form of voltage in capacitor.


<img width="558" height="312" alt="image" src="https://github.com/user-attachments/assets/beef8ca2-4f0d-48e7-9ebb-2c4ce5c0d125" />




During tracking phase/ Acquisition mode, the transient current drawn from the input by capacitor(CH) can introduce noise at the input.In hold mode, the voltage stored in the capacitor can be corrupted by any constant or transient current draw by the following circuit.

Need for Sample and Hold Circuits

If the input analog voltage of an ADC changes more than ±1/2 LSB, then there is a severe chance that the output digital value is an error.
For the ADC to produce accurate results, the input analog voltage should be held constant for the duration of the conversion.
As the name suggests, a S/H Circuit samples the input analog signal based on a sampling command and holds the output value at its output until the next sampling command is arrived.


Types of Sample and Hold architectures:

1.Open loop architecture.
2.Closed loop architecture.
3.Closed loop with pedestal error cancellation.
4.Switched capacitor architecture.
5.Current mode architecture.

1.Open loop architecture.

<img width="753" height="296" alt="image" src="https://github.com/user-attachments/assets/1efd9aab-9c83-4546-b4e0-1a3c78bf2f68" />

Used for high speed data conversion- stable if B1 and B2 are stable. The speed is decided by acquisition time and hold settling time.


2.Closed loop architecture.

<img width="816" height="365" alt="image" src="https://github.com/user-attachments/assets/d8ddb61a-6c0a-4fb2-9df7-d8be82c9714a" />

Closed loop configuration reduces the pedestal error.


3.Closed loop with pedestal error cancellation.

Pedestal error cancellation is a technique used in closed-loop systems to correct low-frequency errors in the system’s output signal.In a closed-loop system, a feedback mechanism continuously monitors theoutput and adjusts the input to reduce any errors. Pedestal errors, which are unwanted shifts in the signal baseline, can be subtracted out through feedback
and correction circuits.

4.Switched capacitor architecture.

<img width="636" height="304" alt="image" src="https://github.com/user-attachments/assets/406f0b75-beda-4a0a-8a30-b14dd619ba32" />

Consists of transconductance amplifier, sampling capacitor CH, s1-s3 switches. Widely used configuration- in ADC for capacitive load-Used in Pipelined AD

5.Current mode architecture.

<img width="726" height="233" alt="image" src="https://github.com/user-attachments/assets/37e192e0-7ed5-4338-abb3-c77cc9cd1c3a" />

Current Mode Architecture refers to a system design where current, rather than voltage, is used as the primary signal parameter. This approach is commonly used in high-speed analog circuits and communication systems.

Performance metrics 

• Acquisition time, tacq – time taken to stabilize the output.

• Hold settling time, ths – time taken to stabilize sampled output 

• Dynamic range  - ratio between the maximum and minimum signal levels that a system can process without distortion or significant loss of information. 

• Non-linearity error - non linear shift in the curve 

• Aperture jitter – time window for the output to settle after clock transition. 

• Pedestral error voltage - offset that appears in the signal, often due to system imperfections or drift. It results in the output signal being incorrectly displaced from the true baseline (zero or expected reference point). 

• Gain error  - 1-tan(𝜃) 

• Droop rate - the rate at which capacitor’s stored voltage value is reducing. 

• Signal to noise ratio (SNR) – signal power/rms of noise 

• Signal to (noise+distortion) ratio (SNDR) – signal power / signalpower – 1st harmonic amplitude





