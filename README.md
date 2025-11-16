# Exp 5 Experimental verification of frequency response of Digital fiber optic link
# Digital Fiber Optic Link Analysis (600nm)

## AIM:
To analyze the relationship between input and received signal of a 600nm fiber optic cable using digital link.

---

## EQUIPMENTS REQUIRED:
- Fiber optic trainer kit ST 2502  
- Power supply  
- Patch cords  
- CRO (Cathode Ray Oscilloscope)  
- 660 nm fiber cable  

---

## THEORY:

Fiber optic links can be used for transmission of digital as well as analog signals. A fiber optic link typically consists of three main elements:
- **Transmitter**: Converts the electrical input signal into optical (light) energy.
- **Optical Fiber**: Serves as the transmission medium for the light signal.
- **Receiver**: Converts the received light back into an electrical signal, preserving the original signal pattern.

---

## PROCEDURE:

1. Connect the power supply to the board.  
2. Ensure that all switched faults are set to ‘Off’.  
3. Make the following connections:  
   a. Connect the 1 KHz square wave output to emitter 1's input.  
   b. Connect the fiber optic cable between emitter output and detector input.  
   c. Connect detector 1's output to comparator 1’s input.  
   d. Connect comparator 1's output to AC amplifier 1's input.  
4. On the board, switch emitter 1's driver to digital mode.  
5. Switch on the power.  
6. Monitor both the inputs to comparator 1 (TP13 & TP14). Slowly adjust the comparator's bias preset until the DC level on TP13 lies midway between the high and low levels of the signal on TP14.  
7. Observe the input to emitter 1 (TP5) and the output from AC amplifier 1 (TP28). Verify that both signals are identical.  
8. Vary the frequency between 10 Hz to 1 MHz and observe the output voltage for a constant input voltage of 5V.  
9. Calculate the bandwidth by determining the gain in decibels (dB).  

---


## BLOCK DIAGRAM:
<img width="525" height="302" alt="image" src="https://github.com/user-attachments/assets/9aa4dd86-6fff-44b5-aee5-f7c4ee789b1a" />

## TABULATION:  

**Transmission through Digital Link**
| Frequency (Hz) | Output Signal Amplitude (Vo) | Gain = Vo/Vi | Gain in dB |
|----------------|------------------------------|--------------|------------|
|     800        |             2.5 v            |     0.5      |  -6.02     |
|     1k         |             32 v             |     6.4      |   16.12    |
|     2k         |             34 v             |     6.8      |   16.65    |
|     5k         |             36 v             |     7.2      |   17.14    |
|     10k        |             37 v             |     7.4      |   17.38    |
|     20k        |             37 v             |     7.4      |   17.38    |
|     50k        |             37 v             |     7.4      |   17.38    |
|     100k       |             27 v             |     5.4      |   14.64    |
|     250k       |             12.7 v           |     2.54     |   8.096    |

## MODEL GRAPH:
<img width="520" height="258" alt="image" src="https://github.com/user-attachments/assets/35cf94a3-bc56-413a-854b-3fc580396d78" />

## GRAPH:
![WhatsApp Image 2025-11-17 at 00 01 30_2105e0f7](https://github.com/user-attachments/assets/f0aa1a6c-740c-4314-afb8-7d93325af60c)



## RESULT:

   Thus, the frequency response of the digital fiber optic link was successfully verified. The system exhibited a stable response up to its cutoff frequency, beyond which the signal amplitude decreased due to attenuation. The measured bandwidth of the digital fiber optic link is approximately 200 kHz, confirming the expected performance characteristics of digital optical transmission.
