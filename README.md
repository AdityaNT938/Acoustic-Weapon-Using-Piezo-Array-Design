# Acoustic-Weapon-Using-Piezo-Array-Design
A wireless-controlled directional acoustic system combining an FM transceiver, a Class-D power amplifier, and a piezoelectric speaker array for acoustic beamforming. Simulated in LTSpice and MATLAB Simulink.

1. Introduction
The Acoustic Noise Weapon project is a wireless-controlled directional acoustic system designed to demonstrate the principles of sound propagation, wireless communication, amplification, and beamforming. The system combines an FM transmitter–receiver architecture with a high-gain audio amplification stage and a piezoelectric speaker array. Unlike conventional loudspeakers that distribute sound uniformly in all directions, the proposed system concentrates acoustic energy in a desired direction through constructive interference between multiple speaker elements.

The project is intended as an educational and research-oriented platform for studying acoustic beamforming, wireless triggering, analog communication systems, and speaker array behavior. The design emphasizes low cost, simplicity, and safe operation while still demonstrating the underlying engineering concepts.

2. Problem Definition
Conventional public-address and warning systems often suffer from poor directionality, causing sound energy to be wasted in unwanted directions. This leads to reduced efficiency and increased disturbance to surrounding areas. There is a growing need for systems capable of directing sound toward a specific region while minimizing sound spread elsewhere.

This project addresses this challenge by combining FM-based wireless communication with a directional speaker array capable of focusing acoustic energy using constructive interference techniques.

4. Objectives
Primary Objective:
To design and simulate a wireless-controlled acoustic system integrating FM transmission with directional sound propagation.

Secondary Objectives:
• Design a pre-amplifier for conditioning low-level audio signals.
• Generate a stable RF carrier using a Colpitts oscillator.
• Implement FM modulation and demodulation.
• Establish wireless communication between transmitter and receiver.
• Amplify recovered audio signals.
• Demonstrate acoustic beamforming using a piezo speaker array.
• Analyze system performance through simulation.

5. Methodology
The methodology consists of several stages. First, an audio signal is generated and conditioned using a pre-amplifier. The signal is then used to modulate a carrier produced by a Colpitts oscillator. The modulated signal is transmitted wirelessly using an FM transmitter.
 <img width="940" height="525" alt="image" src="https://github.com/user-attachments/assets/18e64833-17a3-43fd-b85e-20b7adb462e5" />



At the receiver side, the signal is demodulated and passed through a power amplifier. The amplified signal is supplied to multiple speaker elements arranged as an array. Small phase delays are introduced between adjacent speakers. These phase shifts create constructive interference in the desired direction and destructive interference elsewhere, producing a directional acoustic beam.
6. Circuit Description


FM Transmitter:
The transmitter combines the audio signal with the carrier signal through frequency modulation and transmits it wirelessly.
 
<img width="940" height="430" alt="image" src="https://github.com/user-attachments/assets/b8ab37ad-d5cd-4c04-ac2a-23b970cbca72" />



FM Receiver and Demodulator:
The receiver captures the transmitted signal and recovers the original audio information through demodulation.

 <img width="940" height="250" alt="image" src="https://github.com/user-attachments/assets/ca7db506-9b6c-4997-81e0-5afa90ebf751" />



Power Amplifier:
The power amplifier increases the signal strength sufficiently to drive the speaker array and produce the required acoustic intensity.
 <img width="940" height="706" alt="image" src="https://github.com/user-attachments/assets/0b9c2947-6016-41c7-899e-05540173c30d" />


7. Simulink Model and Beamforming
A MATLAB Simulink model was developed to represent the signal path from source generation to acoustic output. The model consists of a signal generator, gain blocks, delay elements, individual speaker blocks, and a summation block.

Each gain block represents amplification provided to an individual speaker. Delay elements introduce phase differences between speakers. The summation block represents the combination of acoustic waves emitted by all speakers.
 
<img width="940" height="580" alt="image" src="https://github.com/user-attachments/assets/ec6eb124-b6d7-45c0-a09e-04fe990538d9" />


The simulation demonstrates constructive interference where sound waves add together in phase, increasing overall acoustic intensity. This behavior validates the beamforming principle used in the project.
