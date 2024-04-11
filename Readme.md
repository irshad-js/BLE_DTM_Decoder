# Bluetooth Low Energy DTM decoder

---
### Accompanying blog post here : [Irshad's technical blog](https://irshad-js.github.io/posts/Experimentations_with_BLE_part_2/)

### My hardware setup.
---
![Software defined radio attached with DUT using RF-Link](Images/Hardware_Setup.jpg)

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
