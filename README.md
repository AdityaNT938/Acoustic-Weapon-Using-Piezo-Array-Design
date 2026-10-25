# Acoustic-Weapon-Using-Piezo-Array-Design
A wireless-controlled directional acoustic system combining an FM transceiver, a Class-D power amplifier, and a piezoelectric speaker array for acoustic beamforming. Simulated in LTSpice and MATLAB Simulink.

1. Introduction :
   
The Acoustic Noise Weapon project is a wireless-controlled directional acoustic system designed to demonstrate the principles of sound propagation, wireless communication, amplification, and beamforming. The system combines an FM transmitter–receiver architecture with a high-gain audio amplification stage and a piezoelectric speaker array. Unlike conventional loudspeakers that distribute sound uniformly in all directions, the proposed system concentrates acoustic energy in a desired direction through constructive interference between multiple speaker elements.

The project is intended as an educational and research-oriented platform for studying acoustic beamforming, wireless triggering, analog communication systems, and speaker array behavior. The design emphasizes low cost, simplicity, and safe operation while still demonstrating the underlying engineering concepts.

2. Problem Definition:
   
Conventional public-address and warning systems often suffer from poor directionality, causing sound energy to be wasted in unwanted directions. This leads to reduced efficiency and increased disturbance to surrounding areas. There is a growing need for systems capable of directing sound toward a specific region while minimizing sound spread elsewhere.

This project addresses this challenge by combining FM-based wireless communication with a directional speaker array capable of focusing acoustic energy using constructive interference techniques.

4. Objectives: 
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

5. Methodology :
6. 
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
<img width="940" height="580" alt="image" src="https://github.com/user-attachments/assets/6e2d50dd-ed76-4060-88e2-2031fe2eb4b4" />

8. Results and Discussion
Simulation results confirmed successful operation of all major subsystems. The Colpitts oscillator generated a stable carrier signal. FM modulation and demodulation were verified through waveform analysis.
 <img width="944" height="418" alt="image" src="https://github.com/user-attachments/assets/020ab2f9-eedb-47bb-91b2-1e5221baafcd" />



 The recovered audio signal maintained acceptable integrity after transmission.

The speaker-array simulation produced significantly higher output amplitude than a single speaker. A single speaker generated approximately ±20 amplitude units, while the combined array output reached approximately ±105 amplitude units. This increase demonstrates constructive interference and validates the directional sound generation concept.
  

<img width="940" height="829" alt="image" src="https://github.com/user-attachments/assets/460ad0d8-d438-4a02-ba49-8202d18192a6" />


The results indicate that beamforming can substantially improve acoustic intensity in the desired direction while reducing unwanted sound dispersion.

9. Expected Outcomes and Applications
    
Expected outcomes include successful wireless transmission of audio signals, demonstration of FM communication principles, validation of speaker-array beamforming, and analysis of directional acoustic propagation.

Potential applications include:
• Public warning systems
• Crowd management systems
• Industrial safety alerts
• Smart city communication infrastructure
• Targeted audio delivery systems
• Educational demonstrations of beamforming and wireless communication
10. Conclusion
The Acoustic Noise Weapon project successfully integrates wireless FM communication, analog signal processing, amplification, and directional acoustic output into a single system. Simulation results demonstrate stable signal generation, successful modulation and demodulation, and effective beamforming through a speaker array.

The project establishes a strong foundation for future work involving advanced beamforming algorithms, digital signal processing, smart audio systems, and targeted communication technologies. The work also provides valuable practical experience in communication engineering, analog electronics, acoustics, and system simulation.


 



The simulation demonstrates constructive interference where sound waves add together in phase, increasing overall acoustic intensity. This behavior validates the beamforming principle used in the project.
