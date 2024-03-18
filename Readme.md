# Bluetooth Low Energy DTM decoder
---
### Are you intrigued about this machine and the waveform it displays ?

![BLE DTM on CBT ](Images/BLE.jpg)
---
### Its a Bluetooth Low Energy analyzer called CBT. In this repository, I have included all the files that I created to decode a BLE based DTM(Direct Test Mode) packet.

### Here is my hardware setup.
---
![Software defined radio attached with DUT using RF-Link](Images/Hardware_Setup.jpg)

### There are different groups of files included in this repository.
---

### The hackrf_radio_DTM_capture folder contains RAW data of different DTM data patterns (0 through 7) at channel 4 (2410MHz) with a 20M sample rate.

---

### The Logic_Analyzer_DTM_Capture folder contains the logic analyzer data from the host that produced the radio frequency data of DTM data patterns (0 thorugh 7) at channel 4 (2410MHz).

---

![The GNU radio companion flow diagram](Images/GnuRadio_Flow.png)

---

### The BLE_DTM_Decoder.grc is the GnuRadioCompanion file that is used to experiment with the different recorded DTM capture files to decode them into hex data files for further analysis.

---

![Resulting Hex data file from analysis](Images/Packet_decoding.png)

---
### The Preamble_OtherInformation text file contains various different data such as Preamble, Access Address, Header data, Data packets, CRC information used for comparison.

---

![Logic analyzer data and Radio decoding comparison](Images/Comparison.png)

## Youtube video presentation - Part 1 - Pre-requisite know-how - click on the image below:

[![Part - 1](https://img.youtube.com/vi/K1_faNC7W3E/0.jpg)](https://www.youtube.com/watch?v=K1_faNC7W3E)

## Youtube video presentation - Part 2 - Hands-on demo - click on the image below:

[![Part - 2](https://img.youtube.com/vi/fmAM97e1No0/0.jpg)](https://www.youtube.com/watch?v=fmAM97e1No0)

## There is  no hardware required for this experimentation as all the RAW data have already been recorded. Install GnuRadioCompanion and try the various recorded RAW files to get different decoded hex output files.
