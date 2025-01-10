<h1 align="center">FINAL REPORT</h1>

<h2 align="center">Pattern-of-Life Analysis and Deviations for Bluetooth and Bluetooth Low Energy Devices</h2>
<img src=".\BLE Image\CSUSB_logo.png" alt="CSUSB Logo">
<h3 align="center">Department of Information and Decision Sciences<br>California State University, San Bernardino<br>5500 University Parkway,<br>San Bernardino CA 92407</h3>

## TABLE OF CONTENTS

## TABLE OF CONTENTS
1. [TABLE OF CONTENTS](#table-of-contents)
2. [A. PROJECT SUMMARY](#a-project-summary)
    - [A.1 Short Phrase:](#a1-short-phrase)
    - [A.2 Keywords:](#a2-keywords)
    - [A.3 Project Description:](#a3-project-description)
3. [B. EXECUTIVE SUMMARY](#b-executive-summary)
   - [B.1 Keywords:](#b1-keywords)
   - [B.2 Summary:](#b2-summary)
4. [C. INTRODUCTION](#c-introduction)
   - [C.1 Problem Statement:](#c1-problem-statement)
   - [C.2 Purpose Statement:](#c2-purpose-statement)
   - [C.3 Motivation:](#c3-motivation)
5. [D. Literature Review](#d-literature-review)
   - [D.1 Organization:](#d1-organization)
   - [D.2 Motivation:](#d2-motivation)
   - [D.3 Alternative Views:](#d3-alternative-views)
   - [D.4 Reasoning:](#d4-reasoning)
6. [E. Methods and Procedures](#e-methods-and-procedures)
   - [E.1 Defined Approach](#e1-defined-approach)
   - [E.2 Plan Overview](#e2-plan-overview)
   - [E.3 Limitations/Delimitations](#e3-limitationsdelimitations)
7. [F. Findings](#f-findings)
   - [F.1 Findings Overview](#f1-findings-overview)
   - [F.2 Pattern-of-Life (RStudio)](#f2-pattern-of-life-rstudio)
   - [F.3 Wireshark](#f3-wireshark)
8. [G. Issues](#g-issues)
9. [H. Conclusions and Recommendations](#h-conclusions-and-recommendations)
    - [H.1 Conclusions](#h1-conclusions)
    - [H.2 Future Work](#h2-future-work)
10. [I. References](#i-references)
11. [J. Team Bio sketch](#j-team-bio-sketch)

<h2 align="center">A. PROJECT SUMMARY</h2>

**Pattern-of-Life Analysis and Deviations for Bluetooth and Bluetooth Low Energy Devices**  
*December 9, 2022*  
*California State University, San Bernardino*  

Technical Directors:  
Stephanie Polczynski  
sdpolcz@uwe.nsa.gov  

Erik Brasile  
eabrasi@uwe.nsa.gov  

Project Supervisor:  
Tony Coulson  
tcoulson@csusb.edu  

**INSuRE Team - Fall 2022:**  
Matthew Weir - 007476255@coyote.csusb.edu  
Jed Bajarias - 007747942@coyote.csusb.edu  
Frankie Bustamante - 007690885@coyote.csusb.edu  
Irene Gil - 007202553@coyote.csusb.edu  

### A.1 Short Phrase:

The objective of the researchers for this project is to refine and enhance the systems developed by previous INSuRE teams to analyze and fingerprint the Pattern-of-Life for Bluetooth and BLE devices that accomplish the same function.

### A.2 Keywords:

Pattern-of-Life, Bluetooth, Baseline, Bluetooth Low Energy, Deviations, BLE, devices, packets

### A.3 Project Description:

The researchers will use previously researched methods and tools from previous INSuRE teams for capturing and analyzing BLE packets. Using similar hardware and software setups, the team will create a Pattern-of-Life analysis for multiple Bluetooth devices, and compare Patterns-of-Life data to determine baseline traffic, and ascertain ‘abnormal’ data patterns from that.

<h2 align="center">B. EXECUTIVE SUMMARY</h2>

**Pattern-of-life Analysis and Deviations for Bluetooth and Bluetooth Low Energy Devices**  
*December 9, 2022*  
*California State University, San Bernardino*  

Technical Directors:  
Stephanie Polczynski  
sdpolcz@uwe.nsa.gov  

Erik Brasile  
eabrasi@uwe.nsa.gov  

Project Supervisor:  
Tony Coulson  
tcoulson@csusb.edu  

**INSuRE Team - Fall 2022:**  
Matthew Weir - 007476255@coyote.csusb.edu  
Jed Bajarias - 007747942@coyote.csusb.edu  
Frankie Bustamante - 007690885@coyote.csusb.edu  
Irene Gil - 007202553@coyote.csusb.edu  

### B.1 Keywords:

Pattern-of-Life, Bluetooth, Baseline, Bluetooth Low Energy, Deviations, BLE, devices, packets

### B.2 Summary:

This project will use previously gathered researched methods and tools from previous INSuRE teams for capturing and analyzing BLE packets. Previous INSuRE teams have worked off the research conducted by one another and have outlined a path toward capturing and analyzing BLE traffic. The researchers for this project will take advantage of previously done research, and refine the collection of Bluetooth traffic and its determining factor for normal or abnormal traffic. After learning to identify packet contents and the makeup of MAC randomization, they will develop a Pattern-of-Life for their selected devices. From there, they will use Wireshark to analyze their results and develop an analysis technique that may potentially lead to an analysis technique that may lend itself to being automated.

<h2 align="center">C. INTRODUCTION</h2>

### C.1 Problem Statement:

The goal is to use previously researched tools and findings to capture and analyze BLE packets, then create a Pattern-of-Life analysis that will help to better understand the way Bluetooth Low Energy functions. Through understanding of BLE functions and packet behavior, BLE security is also better understood. Reviewing prior INSuRE work to this project, the researchers found the 2020 team from California State University, San Bernardino (CSUSB) and the teams from the University of Alabama in Huntsville (UAH) as best fit for the goal the researchers are aiming to achieve. However, since the team will analyze and build up research from those previous teams, there is a matter of differing knowledge and experience, as those teams had more relevant skills pertaining to the project at hand. Despite this, they hope to utilize their different backgrounds to add and improve upon the findings from what the 2020 CSUSB team and UAH teams had found. As well, because it was found that each team who was previously involved in the project had built on top of each other’s results, there’s also the problem of putting it all together coherently in specific aims for the project. 

### C.2 Purpose Statement

As the use of Bluetooth and Bluetooth Low Energy devices continues to increase, the vulnerability of these devices becomes a more pressing issue. Refining the methods, tools, and scripts developed by previous INSuRE teams informed this research on BLE to create a more in-depth Pattern-of-Life analysis. By building off of the research from the previous 2020 CSUSB team and teams from UAH, the researchers can analyze their data collection methods and refine them, as the project is able to be followed in similar steps. The researchers have the confidence to anticipate obstacles that might impede the process of refining Phase 1 of the project, as doing so provides a more polished picture to work from. Having a large data set to analyze from, establishing a clear Pattern-of-Life analysis, and visualizing its daily ‘baseline’ patterns from the ‘abnormal,’ will assist in the efforts of monitoring one's own devices in a home or office environment.

### C.3 Motivation

By studying and analyzing the results found from the previous INSuRE teams, such as from UAH and the previous CSUSB team from 2020 who had also worked on this project. From what was analyzed in their resulting methods in working on Phase 1 of the project, the researchers felt that Phase 1 could be refined much further. The researchers found it best to start this process by focusing on the UAH team from 2021, as well as addressing some of the concerns they outlined in their project. For UAH, they expressed concern about possibly rushing Phase 1 (e.g., not having enough data from anomaly scenarios, or datasets being too small for robust Patterns-of-Life). Comparatively, other teams such as the 2020 CSUSB team had noted that their Pattern-of-Life data may have been exposed to outside influence. Throughout the project, researchers revisited these steps and compared the results gathered from different solutions, such as capturing data in remote locations versus capturing data inside Faraday cages/bags.

To a larger extent, securing Bluetooth traffic and developing a detection system are crucial for protecting work and home networks. It was noted especially, that the rapid development of the IoT market, rapid device development, and other device constraints had driven developers to especially poor security implementation, leaving behind a proper security design. (Beyer, 2018, pg. 8). Consequently, it led to the widespread use of Bluetooth attacks that resulted in new areas that were not as heavily connected as they were several years ago. Furthermore, outlets, locks, and light bulbs were not part of the functioning network of smart devices, just as vehicles were not connected to the Internet, until now. Because of that, it was further stated that BLE devices were especially vulnerable because their advertising packets are not made private (Beyer, 2018, pg. 8). This problem will continue to grow as many Bluetooth devices continue to grow in use. The researchers aim to develop the research conducted throughout this project, to help better understand Bluetooth and BLE and better secure home and work networks.

<h2 align="center">D. Literature Review</h2>

### D.1 Organization

The researchers conducted scans on low-cost Bluetooth devices with the intention of creating a Pattern-of-Life analysis, to better understand Bluetooth and Bluetooth Low Energy. Their intention was to focus on current research built from previous teams, specifically the 2020 CSUSB team and the UAH team from 2022, because they in particular were able to culminate their respective research in regards to Phase 1 of the project. The research will be used with the intention of building from previous research rather than completely altering or disregarding the previous team’s results. Ultimately, the team will have the project smooth out the details in Phase 1, so that moving forward to Phase 2 will yield the best possible results. Previous research suggests that Bluetooth devices are falling victim to Denial-of-Service attacks, passive/active eavesdropping, Man-In-The-Middle Attacks, message modifications, and resource misappropriation. (Gupta & Kumar, 2015) The 2020 CSUSB team referenced this research in which the Bluetooth data transmission was intercepted, with the use of an Adafruit Bluetooth LE sniffer and Raspberry Pi.

### D.2 Motivation

As the market continues to grow, and more Bluetooth devices are introduced to many people’s networks, one should also be aware of how secure their devices really are. Bluetooth technology in the past decade has expanded greatly, finding its way into smart home appliances, to items people carry daily such as smartwatches or fitness trackers. In 2019, Bluetooth SIG (Bluetooth Special Interest Group), reported that the “Bluetooth Smart Home will see an increase in device shipments in the next few years” with an estimated “1.15 billion devices” to ship in 2023 alone (Bluetooth SIG, n.d.). This surge in connected devices plays a large role in why people should be concerned about the types of data their devices control, and how susceptible their devices are to malicious attacks. The team’s research and the work done in this project has made everyone aware of the importance of developing a system that can detect changes in the behavior of their devices.

### D.3 Alternative Views

New BLE protocols have been implemented to improve the security of BLE devices, and strides have been made for manufacturers to update device firmware and updates. Bluetooth and BLE researchers in this field have also noted the importance of improving and implementing more secure protocols for BLE devices as well.

### D.4 Reasoning

Through this project, the researchers had achieved their main goal of creating a system that allows users to be more secure in a highly populated Bluetooth environment by identifying devices that may be acting abnormally. As the Internet of Things (IoT) technology is ever-expanding, with many IoT devices using Bluetooth it is necessary to have a system in place to detect abnormalities. This system is intended to work off open source tools and software which the average home user of Bluetooth devices will be able to utilize. The researchers intend to test and collect data on popular devices frequently used in day-to-day tasks, which include an Apple Pencil, a Finite Bluetooth Keyboard, and TaoTronics BLE earbuds. Developing this system can expose risks in network security and improve our awareness of the types of devices people bring into our networks. Going beyond the scope of the home network, this system can also have importance in improving workplace infrastructure that seeks to improve the security of their Bluetooth devices.

<h2 align="center">E. Methods and Procedures</h2>

### E.1 Defined Approach

To begin with, the team’s device configuration consisted of the following:

**Devices Used**
- 2x Raspberry Pi 400 kits
- 3x Ubertooth One version 2020-12-R1
- 1x Raspberry Pi 4, Model B 8GB
- 3x Samsung EVO Plus 128GB SD cards
- 1x Apple Pencil (1st Generation)
- 1x Finite Wireless Bluetooth Keyboard
- 1x TaoTronics SoundLiberty 79 Bluetooth earbuds

*Figure #1*

In addition, here was the software used during the project:

**Software Used**
- RStudio version “Spotted Wakerobin”
- Scapy version 2.5.0
- Python version 3.10.8
- Wireshark version 4.0.1
- Kismet 2022-08-R1

*Figure #2*

Since the project is heavily influenced by the prior team from CSUSB on certain aspects, researchers noted many of their approaches in scanning and gathering information from nearby BLE devices. They initially used an Ubertooth One device to conduct Bluetooth captures, but found it insufficient for their needs when collecting data. They also attempted to use a BLE Texas Instruments CC2541 Mini Development Kit to sniff out Bluetooth data, but found it ultimately incompatible with Wireshark. To that regard, the researchers still proceeded to use an Ubertooth One because, despite its limitations, the UAH team from 2021 had noted that using an Ubertooth One had allowed tracking of individual packets, related to specific MAC addresses.

Because the researchers had analyzed some of the methods the previous teams had used, including errors and solutions, they were able to streamline their approaches while working towards the goal of refining Phase 1. The UAH team from 2021 noted that using an Ubertooth One, it only had a 33% chance of finding the right advertising channels of 37, 38, and 39. They recommended not to use more than one Ubertooth One device unless there were multiple Raspberry Pi devices involved, and to that end, the team directly addressed that concern by acquiring those devices. Data collection methods were according to what had the most success, as the researchers analyzed various teams who were previously involved in the project, and the CSUSB team from 2020 and UAH were the most prominent of all in results of their data collection methods.

### E.2 Plan Overview

- Developed an efficient way to collect data using information from the team’s research and findings for the previous teams.
- Setting up Raspberry Pi devices, these would function with the Ubertooth One devices to collect data on the BLE packets. With Kismet, the 24-bit LAP (Lower Address Part) and 8-bit UAP (Upper Address Part) can be identified to determine a BLE device, from within its packet contents.
- Reexamined the Python scripts from the previous team in order to deal with MAC Address Randomization. This script was intended to help in identifying the team's Bluetooth devices and so in order to help this process, the team attempted to minimize device interference during the process when it occurred.
- Once the data was refined, and a controlled data set was present, the packets from that were collected to create Time Series graphs using RStudio to illustrate the Bluetooth Pattern-of-Life.
- After the initial Pattern-of-life was created, the team conducted another capture of their devices, but this time of induced abnormalities to the BLE devices by turning the device on and off frequently.

### E.3 Limitations/Delimitations

There were many experiments conducted based on various data, and resulting information from the 2020 CSUSB team and UAH teams. As the team progressed, many limitations were revealed in regards to relevant experience, in handling the software and hardware used throughout the project. The impact of software limitations occurred during the data collection portion, as the decision to use Kismet limited the channels it could scan on, and much time was spent in order to find a solution to the errors in Kismet. In addition, there were also issues isolating their software and encountered interference even with the use of a Faraday bag. After decreasing their data set by conducting scans in a remote location, the researchers began examining the Python script from the previous CSUSB team. After making needed alterations, the team ran into an exception error, requiring them to alter the script so it could handle more bytes in order to avoid the error shown below in Figure #3.

<img src=".\BLE Image\Python_Script.png" alt="Python Script With Error" >

*Figure #3*

Adjusting the Python script to work with the team’s data set required a lot of trial and error, however, they were able to rewrite the script so that it functioned with their .PCAP files. The images below display the Python script functioning with no exception error as shown in Figure #4.
<p align="center">
<img src=".\BLE Image\Python_NoError.png" alt="Python Script With no Error" >
</p>
<p align="center">
Figure #4
</p>

<h2 align="center">F. Findings</h2>

### F.1 Findings Overview
The team's aim was to create a Pattern-of-Life analysis on BLE devices in order to better understand how Bluetooth Low-Energy devices function and to better understand the behavior of BLE packets. The first step was establishing an effective method to collect Bluetooth data, and when reviewing previous research data, it was concluded that the best choice to most effectively collect that data was by using the Ubertooth One. Despite their efforts to minimize time spent on data collection, they ran into some errors with device interference. After collecting the needed information, it was saved in the form of a .PCAP file then efforts were made to filter out unnecessary information using Python scripts written by previous teams, and the filter feature on Wireshark.  Other methods were also used by the previous CSUSB 2020 team, as the team  understood the reasons why they chose not to go those routes, with Scapy being notable as shown in Figure #6.

<p align="center">
<img src=".\BLE Image\Scapy.png" alt="Scapy" >
</p>
<p align="center">
Figure #6
</p>
It was a partial replication of the steps in their attempts of a Pattern-of-Life analysis through Scapy. Their goal was to find useful information in the form of a hex-dump, and they ultimately determined that the data outputted by Scapy was insufficient. Replicating how they did the process allowed the researchers in further understanding of determining the best ways in analyzing Bluetooth traffic data, in a measure of small achievement.

### F.2 Pattern-of-Life (RStudio)
Consistent with prior research teams, RStudio was also used to conduct a Pattern-of-Life analysis for the team’s chosen devices. The reason for doing so is because the researchers found that the 2020 CSUSB team had regarded RStudio to be the best way of statistical analysis of Bluetooth data captures, and all-around displaying an aggregated collection of data. And in following the goal of ultimately refining Phase 1 of the project, the team had gone in similar steps of using RStudio as well. While the previous 2020 CSUSB team discontinued the use of the Ubertooth One due to insufficient evidence of proper data collection properties, the researchers still went on with using the Ubertooth One, because as mentioned before, the UAH team from 2021 noted that the Ubertooth One allowed tracking of individual packets, related to specific MAC addresses, despite its limitations. In visualizing a Pattern-of-Life, the 2020 CSUSB team concluded that a Time Series analysis graph was the best way to get a picture of ‘baseline’ Bluetooth traffic. In addition, the columns of Time, RF.Channel, Signal.dBm, and Length were chosen as the most relevant items to display in a Time Series graph, as while the columns are slightly different names from what the 2020 CSUSB team had for their Time Series graph, they are essentially the same.
	After some understanding of how RStudio worked, the researchers had converted their .PCAP file to a CSV file for it to be read, then replicated the code from how it was done. Below was the resulting visualization of  Bluetooth data coming from the Apple Pencil device.

<p align="center">
<img src=".\BLE Image\RStudio.jpg" alt="RStudio" >
</p>
<p align="center">
Figure #7
</p>
In the actual file format, the information can be interacted by moving the mouse and seeing the numbers change accordingly. Each column was color-coded to show each section, such as the  Length column overlapping with the RF.Channel column. For this singular instance, the data set of our Apple Pencil was added and imported following the guide in how the previous CSUSB team had done it so. With this, the researchers were able to visualize what a graphed Pattern-of-Life looked like for their Apple Pencil device. And shown the image of Figure #8, is the data set and code used to produce the Time Series analysis image above.
<p align="center">
<img src=".\BLE Image\Timeseries_Analysis.jpg" alt="Timeseries" >
</p>
<p align="center">
Figure #8
</p>

### F.3 Wireshark
By utilizing Wireshark, the researchers were able to inspect the packet contents and make out more information than one would be able to view in Kismet, such as the contents of the packets.  It shows the contents of the packet header, the source, and destination of packets, and if the packet was sent on a primary or secondary advertising channel. Figure #9 below shows the packet content as it is shown in Wireshark for the advertising information utilized to establish a connection between two devices, flags, latency, and access address are shown, as well as other important information. 

<p align="center">
<img src=".\BLE Image\Timeseries_Analysis.jpg" alt="Timeseries" >
</p>
<p align="center">
Figure #9
</p>
