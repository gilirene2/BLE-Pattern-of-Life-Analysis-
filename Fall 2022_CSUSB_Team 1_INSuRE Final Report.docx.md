# FINAL REPORT
![CSUSB Logo](CSUSB_Logo.png)

## Pattern-of-Life Analysis and Deviations for Bluetooth and Bluetooth Low Energy Devices

**Department of Information and Decision Sciences**  
California State University, San Bernardino  
5500 University Parkway,  
San Bernardino CA 92407

---

## TABLE OF CONTENTS

1. [TABLE OF CONTENTS](#table-of-contents)
2. [A. PROJECT SUMMARY](#a-project-summary)
   1. [A.1 Short Phrase](#a1-short-phrase)
   2. [A.2 Keywords](#a2-keywords)
   3. [A.3 Project Description](#a3-project-description)
3. [B. EXECUTIVE SUMMARY](#b-executive-summary)
   1. [B.1 Keywords](#b1-keywords)
   2. [B.2 Summary](#b2-summary)
4. [C. INTRODUCTION](#c-introduction)
   1. [C.1 Problem Statement](#c1-problem-statement)
   2. [C.2 Purpose Statement](#c2-purpose-statement)
   3. [C.3 Motivation](#c3-motivation)
5. [D. Literature Review](#d-literature-review)
   1. [D.1 Organization](#d1-organization)
   2. [D.2 Motivation](#d2-motivation)
   3. [D.3 Alternative Views](#d3-alternative-views)
   4. [D.4 Reasoning](#d4-reasoning)
6. [E. Methods and Procedures](#e-methods-and-procedures)
   1. [E.1 Defined Approach](#e1-defined-approach)
   2. [E.2 Plan Overview](#e2-plan-overview)
   3. [E.3 Limitations/Delimitations](#e3-limitationsdelimitations)

---

## A. PROJECT SUMMARY

**Pattern-of-Life Analysis and Deviations for Bluetooth and Bluetooth Low Energy Devices**  
**December 9, 2022**  
California State University, San Bernardino  

### Technical Directors:
- **Stephanie Polczynski**  
  Email: [sdpolcz@uwe.nsa.gov](mailto:sdpolcz@uwe.nsa.gov)  
- **Erik Brasile**  
  Email: [eabrasi@uwe.nsa.gov](mailto:eabrasi@uwe.nsa.gov)

### Project Supervisor:
- **Tony Coulson**  
  Email: [tcoulson@csusb.edu](mailto:tcoulson@csusb.edu)

### INSuRE Team - Fall 2022:
- **Matthew Weir**: [007476255@coyote.csusb.edu](mailto:007476255@coyote.csusb.edu)
- **Jed Bajarias**: [007747942@coyore.csusb.edu](mailto:007747942@coyore.csusb.edu)
- **Frankie Bustamante**: [007690885@coyote.csusb.edu](mailto:007690885@coyote.csusb.edu)
- **Irene Gil**: [007202553@coyote.csusb.edu](mailto:007202553@coyote.csusb.edu)

### A.1 Short Phrase
The objective of the researchers for this project is to refine and enhance the systems developed by previous INSuRE teams to analyze and fingerprint the Pattern-of-Life for Bluetooth and BLE devices that accomplish the same function.

### A.2 Keywords
Pattern-of-Life, Bluetooth, Baseline, Bluetooth Low Energy, Deviations, BLE, devices, packets

### A.3 Project Description
The researchers will use previously researched methods and tools from previous INSuRE teams for capturing and analyzing BLE packets. Using similar hardware and software setups, the team will create a Pattern-of-Life analysis for multiple Bluetooth devices, and compare Patterns-of-Life data to determine baseline traffic, and ascertain ‘abnormal’ data patterns from that.

---

## B. EXECUTIVE SUMMARY

**Pattern-of-life Analysis and Deviations for Bluetooth and Bluetooth Low Energy Devices**  
**December 9, 2022**  
California State University, San Bernardino  

### Technical Directors:
- **Stephanie Polczynski**  
  Email: [sdpolcz@uwe.nsa.gov](mailto:sdpolcz@uwe.nsa.gov)  
- **Erik Brasile**  
  Email: [eabrasi@uwe.nsa.gov](mailto:eabrasi@uwe.nsa.gov)

### Project Supervisor:
- **Tony Coulson**  
  Email: [tcoulson@csusb.edu](mailto:tcoulson@csusb.edu)

### INSuRE Team - Fall 2022:
- **Matthew Weir**: [007476255@coyote.csusb.edu](mailto:007476255@coyote.csusb.edu)
- **Jed Bajarias**: [007747942@coyore.csusb.edu](mailto:007747942@coyore.csusb.edu)
- **Frankie Bustamante**: [007690885@coyote.csusb.edu](mailto:007690885@coyote.csusb.edu)
- **Irene Gil**: [007202553@coyote.csusb.edu](mailto:007202553@coyote.csusb.edu)

### B.1 Keywords
Pattern-of-Life, Bluetooth, Baseline, Bluetooth Low Energy, Deviations, BLE, devices, packets

### B.2 Summary
This project will use previously gathered researched methods and tools from previous INSuRE teams for capturing and analyzing BLE packets. Previous INSuRE teams have worked off the research conducted by one another and have outlined a path toward capturing and analyzing BLE traffic. The researchers for this project will take advantage of previously done research and refine the collection of Bluetooth traffic and its determining factor for normal or abnormal traffic. After learning to identify packet contents and the makeup of MAC randomization, they will develop a Pattern-of-Life for their selected devices. From there, they will use Wireshark to analyze their results and develop an analysis technique that may potentially lend itself to automation.

---

## C. INTRODUCTION

### C.1 Problem Statement
The goal is to use previously researched tools and findings to capture and analyze BLE packets, then create a Pattern-of-Life analysis that will help to better understand the way Bluetooth Low Energy functions. Through understanding of BLE functions and packet behavior, BLE security is also better understood. Reviewing prior INSuRE work to this project, the researchers found the 2020 team from California State University, San Bernardino (CSUSB) and the teams from the University of Alabama in Huntsville (UAH) as best fit for the goal the researchers are aiming to achieve. However, since the team will analyze and build up research from those previous teams, there is a matter of differing knowledge and experience, as those teams had more relevant skills pertaining to the project at hand. Despite this, they hope to utilize their different backgrounds to add and improve upon the findings from what the 2020 CSUSB team and UAH teams had found. As well, because it was found that each team who was previously involved in the project had built on top of each other’s results, there’s also the problem of putting it all together coherently in specific aims for the project.

### C.2 Purpose Statement
As the use of Bluetooth and Bluetooth Low Energy devices continues to increase, the vulnerability of these devices becomes a more pressing issue. Refining the methods, tools, and scripts developed by previous INSuRE teams informed this research on BLE to create a more in-depth Pattern-of-Life analysis. By building off of the research from the previous 2020 CSUSB team and teams from UAH, the researchers can analyze their data collection methods and refine them, as the project is able to be followed in similar steps. The researchers have the confidence to anticipate obstacles that might impede the process of refining Phase 1 of the project, as doing so provides a more polished picture to work from. Having a large data set to analyze from, establishing a clear Pattern-of-Life analysis, and visualizing its daily ‘baseline’ patterns from the ‘abnormal,’ will assist in the efforts of monitoring one's own devices in a home or office environment.

### C.3 Motivation
By studying and analyzing the results found from the previous INSuRE teams, such as from UAH and the previous CSUSB team from 2020 who had also worked on this project. From what was analyzed in their resulting methods in working on Phase 1 of the project, the researchers felt that Phase 1 could be refined much further. The researchers found it best to start this process by focusing on the UAH team from 2021, as well as addressing some of the concerns they outlined in their project. For UAH, they expressed concern about possibly rushing Phase 1 (e.g., not having enough data from anomaly scenarios, or datasets being too small for robust Patterns-of-Life). Comparatively, other teams such as the 2020 CSUSB team had noted that their Pattern-of-Life data may have been exposed to outside influence. Throughout the project, researchers revisited these steps and compared the results gathered from different solutions, such as capturing data in remote locations versus capturing data inside Faraday cages/bags.

To a larger extent, securing Bluetooth traffic and developing a detection system are crucial for protecting work and home networks. It was noted especially, that the rapid development of the IoT market, rapid device development, and other device constraints had driven developers to especially poor security implementation, leaving behind a proper security design. Consequently, it led to the widespread use of Bluetooth attacks that resulted in new areas that were not as heavily connected as they were several years ago. Furthermore, outlets, locks, and light bulbs were not part of the functioning network of smart devices, just as vehicles were not connected to the Internet, until now. Because of that, it was further stated that BLE devices were especially vulnerable because their advertising packets are not made private. This problem will continue to grow as many Bluetooth devices continue to grow in use. The researchers aim to develop the research conducted throughout this project, to help better understand Bluetooth and BLE and better secure home and work networks.

---

## D. Literature Review

### D.1 Organization
The researchers conducted scans on low-cost Bluetooth devices with the intention of creating a Pattern-of-Life analysis, to better understand Bluetooth and Bluetooth Low Energy. Their intention was to focus on current research built from previous teams, specifically the 2020 CSUSB team and the UAH team from 2022, because they in particular were able to culminate their respective research in regards to Phase 1 of the project. The research will be used with the intention of building from previous research rather than completely altering or disregarding the previous team’s results. Ultimately, the team will have the project smooth out the details in Phase 1, so that moving forward to Phase 2 will yield the best possible results. Previous research suggests that Bluetooth devices are falling victim to Denial-of-Service attacks, passive/active eavesdropping, Man-In-The-Middle Attacks, message modifications, and resource misappropriation. The 2020 CSUSB team referenced this research in which the Bluetooth data transmission was intercepted, with the use of an Adafruit Bluetooth LE sniffer and Raspberry Pi.

### D.2 Motivation
As the market continues to grow, and more Bluetooth devices are introduced to many people’s networks, one should also be aware of how secure their devices really are. Bluetooth technology in the past decade has expanded greatly, finding its way into smart home appliances, to items people carry daily such as smartwatches or fitness trackers. In 2019, Bluetooth SIG (Bluetooth Special Interest Group), reported that the “Bluetooth Smart Home will see an increase in device shipments in the next few years” with an estimated “1.15 billion devices” to ship in 2023 alone. This surge in connected devices plays a large role in why people should be concerned about the types of data their devices control, and how susceptible their devices are to malicious attacks. The team’s research and the work done in this project has made everyone aware of the importance of developing a system that can detect changes in the behavior of their devices.

### D.3 Alternative Views
New BLE protocols have been implemented to improve the security of BLE devices, and strides have been made for manufacturers to update device firmware and updates. Bluetooth and BLE researchers in this field have also noted the importance of improving and implementing more secure protocols for BLE devices as well.

### D.4 Reasoning
Through this project, the researchers had achieved their main goal of creating a system that allows users to be more secure in a highly populated Bluetooth environment by identifying devices that may be acting abnormally. As the Internet of Things (IoT) technology is ever-expanding, with many IoT devices using Bluetooth, it is necessary to have a system in place to detect abnormalities. This system is intended to work off open-source tools and software which the average home user of Bluetooth devices will be able to utilize. The researchers intend to test and collect data on popular devices frequently used in day-to-day tasks, which include an Apple Pencil, a Finite Bluetooth Keyboard, and TaoTronics BLE earbuds. Developing this system can expose risks in network security and improve our awareness of the types of devices people bring into our networks. Going beyond the scope of the home network, this system can also have importance in improving workplace infrastructure that seeks to improve the security of their Bluetooth devices.

---

## E. Methods and Procedures

### E.1 Defined Approach
To begin with, the team’s device configuration consisted of the following:

#### Devices Used
- 2x Raspberry Pi 400 kits
- 3x Ubertooth One version 2020-12-R1
- 1x Raspberry Pi 4, Model B 8GB
- 3x Samsung EVO Plus 128GB SD cards
- 1x Apple Pencil (1st Generation)
- 1x Finite Wireless Bluetooth Keyboard
- 1x TaoTronics SoundLiberty 79 Bluetooth earbuds

#### Software Used
- RStudio version “Spotted Wakerobin”
- Scapy version 2.5.0
- Python version 3.10.8
- Wireshark version 4.0.1
- Kismet 2022-08-R1
