# Home Audio System  
This project was all about building a complete **home audio system** that combines signal processing, power amplification, and real-time visualization. 
The final system featured a **3-band graphic equalizer**, a **Class-D amplifier**, and both an **OLED** and **TFT display** for spectrogram output.

## Features
- **3-Band Graphic Equalizer**: Active bandpass filters for bass (100–500 Hz), mid (500 Hz–2 kHz), and treble (2–8 kHz), each adjustable by ±10 dB using potentiometers  
- **Class-D Amplifier**: MOSFET switching with dead-time control, efficient PWM modulation at 80 kHz, and a 2nd-order RLC filter for clean audio reconstruction  
- **Spectrogram Display**: Real-time visualization of frequency levels on an OLED screen, plus an extended **2.2” TFT SPI LCD** with color graphics  
- **Extended Output Options** *(beyond requirements)*: Designed for headphones originally, but we added support for both **headphones and speaker outputs**, giving the user flexibility to switch between two loads  

## Tools & Hardware
- **Analog Circuits**: Bandpass filters, op-amps, MOSFET output stage, RLC filter
- **Software**: simulations in LTspice, Arduino IDE, Analog Filter Design Wizard 
- **Microcontrollers**: Arduino Uno (for PWM + display control)  
- **Displays**: OLED + TFT SPI LCD  

## Repo Structure
- `demo/` → System demonstration videos
- `figures/` → Key design and implementation images  
  - High-level system design diagram  
  - Annotated breadboard circuit of equalizer & Class-D amplifier
  - Annotated breadboard Speaker and headphone connections
  - OLED display screen

## Validation
- Frequency responses of each BPF matched simulation within <2 dB ripple  
- Amplifier produced clean waveforms with THD ~2.3%
- OLED/TFT spectrogram updated in real-time at ~16 kHz sampling  
- System demoed live with both headphones and speaker playback


