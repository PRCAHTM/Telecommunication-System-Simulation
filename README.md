# Digital Communication System Simulation

This project is a complete simulation of a digital communication system, built as part of my Communication Systems course at Sharif University of Technology.

The goal was to design and implement an end-to-end communication chain — from generating bits at the transmitter to recovering them at the receiver — and analyze how different modulation methods perform under noise and channel limitations.

---

## What This Project Does

This simulation models a real digital communication system including:

- Bit generation and time-division multiplexing  
- Pulse shaping (NRZ / RZ)  
- Analog modulation (PAM, PSK, FSK)  
- Band-limited channel with noise (AWGN)  
- Coherent demodulation  
- Matched filtering  
- Bit detection and error analysis  
- 8-bit data transmission  
- μ-law companding  
- Quantization and SNR analysis  
- Real audio processing  

Each block was implemented separately and then integrated into a full working communication system.

---

## Modulation Schemes Compared

The system was tested using:

- PAM – Strong noise resistance  
- PSK – More power efficient  
- FSK – Higher bandwidth usage  

Each scheme was evaluated based on:

- Probability of error vs noise variance  
- Power efficiency  
- Bandwidth consumption  
- Detection complexity  

This allowed a practical comparison of theoretical trade-offs discussed in class.

---

## Performance Analysis

Key evaluations include:

- Error probability as noise variance increases  
- Signal constellation diagrams  
- Error distribution for multi-bit transmission  
- SNR behavior under different quantization levels  
- Effect of μ parameter in companding  

Main observations:

- Increasing noise leads to higher error probability  
- Increasing quantization levels increases SNR  
- μ has an optimal operating range (very large values degrade performance)  

---

## Audio Processing Section

To connect theory with real signals, the system was extended to process audio:

- Audio recording and normalization  
- μ-law compression and expansion  
- Uniform quantization  
- RMS reconstruction error calculation  
- Output SNR evaluation  

This demonstrates how digital communication concepts apply to real-world voice signals.

---

## Technologies Used

- Python  
- NumPy  
- SciPy  
- Matplotlib  
- SoundDevice  

---

## How to Run

Install dependencies:

```bash
pip install numpy scipy matplotlib sounddevice
```

Run the main script or notebook:

```bash
python main.py
```

Note: The audio recording section should not be re-run unless you want to overwrite the saved audio file.

---

## Course Information

Communication Systems  
Sharif University of Technology  
Winter 1402  

---

## Author

Parsa Hatami
