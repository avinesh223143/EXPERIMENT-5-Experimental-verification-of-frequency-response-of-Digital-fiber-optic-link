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

Fiber optic links can be used for transmission of digital as well as analog signals. Basically a fiber optic link contains three main elements, a transmitter, an optical fiber and a receiver. The transmitter module takes the input signal in electrical form and then transforms it into optical (light) energy containing the same information. The optical fiber is the medium which takes the energy to the receiver. At the receiver light is converted back into electrical form with the same pattern as originally fed to the transmitter.

TRANSMITTER:

LED, digital DC coupled transmitters are one of the most popular varieties due to their ease of fabrication. We have used a standard TTL gate to drive a NPN transistor, which modulates the LED SFH450V or SFH 756V source. (Turns it on and off).

RECEIVER:

SFH-551V is a digital optodetector. It delivers a digital output, which can be processed directly with little additional external circuitry. The integrated circuit inside the SFH551V optodetector comprises the photodiode device, a transimpedance amplifier, a comparator and a level shifter.

The photodiode converts the detected light into a photocurrent. With the aid of an integrated lens the light emanating from the plastic Fiber is almost entirely focused on the surface of the diode. At the next stage the trans-impedance amplifier converts the photocurrent into a voltage. In the comparator, the voltage is compared to a reference voltage. In over to ensure good synchronism between the reference and the trans- impedance output voltage, the former is derived from a second circuit of a similar kind, which incorporates a “blind” photodiode. The comparator derives a level shifter with an open collector output stages. Here a catch diode (similar to Schottky-TTL) prevents the saturation of the output transistor, thus limiting the output voltage to the supply voltage.


## PROCEDURE:

1-	Refer to the block diagram & carry out the following connections and settings.
-	Connect the power supply with proper polarity to the kit link-B and switch it on.
-	Keep all Switch Faults in OFF position.
-	Keep switch SW8 towards TX position.
-	Keep switch SW9 towards TX1 position.
-	Keep switch SW10 towards TTL position.
-	Keep Jumper JP5 towards +5V position.
-	Keep Jumpers JP6 shorted.
-	Keep Jumper JP8 towards Pulse position.
-	Feed TTL Square wave signal of 1KHz from the function generator to the IN post of Digital Buffer.

<img width="507" height="295" alt="image" src="https://github.com/user-attachments/assets/6267363b-e383-452b-9e42-0a84fb077b02" />
 
-	Connect the output post OUT of Digital Buffer to the post TX IN of Transmitter.
-	Slightly unscrew the cap of SFH756V (660nm). Do not remove the cap from the connector. Once the cap is loosened, insert the one meter fiber into the cap. Now tighten the cap by screwing it back.
-	Connect the other end of the Fiber to detector SFH551V (Photo Transistor Detector) very carefully.
-	Observe the detected signal at post TTL OUT on oscilloscope.

 <img width="507" height="295" alt="image" src="https://github.com/user-attachments/assets/b9b81581-4572-465b-b7f5-c19945b1c3fe" />

-	To measure the digital bandwidth of the phototransistor vary the input signal frequency and observe the detected signal at various frequencies.
-	Determine the frequency at which the detector stops recovering the signal. This determines the max. bit rate on the digital link.
-	Keep switch SW9 towards TX2 position.
-	Keep Jumper JP7 towards +5V position.
-	Remove fiber cable from SFH756V (660nm) and slightly unscrew the cap of SFH450V (950nm). Do not remove the cap from the connector. Once the cap is loosened, insert the one meter fiber into the cap. Now tighten the cap by screwing it back.
-	Observe the detected signal at post TTL OUT on oscilloscope.

<img width="507" height="295" alt="image" src="https://github.com/user-attachments/assets/28db90ea-6a22-4570-bf4a-6727e34cc2e5" />


---


## BLOCK DIAGRAM:
<img width="525" height="302" alt="image" src="https://github.com/user-attachments/assets/9aa4dd86-6fff-44b5-aee5-f7c4ee789b1a" />

## CONNECTION DIAGRAM
![517821167-6ff5af5c-c081-4722-b2e6-b20cb84aadab](https://github.com/user-attachments/assets/6285d55a-b826-4d41-80f7-edb09d6702cc)

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
![WhatsApp Image 2025-11-16 at 22 09 16_19c73223](https://github.com/user-attachments/assets/6434da9a-6548-428b-be68-86b3c8c2d012)


## RESULT:

   Thus, the frequency response of the digital fiber optic link was successfully verified. The system exhibited a stable response up to its cutoff frequency, beyond which the signal amplitude decreased due to attenuation. The measured bandwidth of the digital fiber optic link is approximately 200 kHz, confirming the expected performance characteristics of digital optical transmission.
