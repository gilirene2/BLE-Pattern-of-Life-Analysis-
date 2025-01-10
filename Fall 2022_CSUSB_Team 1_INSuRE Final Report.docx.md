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
 
Erik Brasile    

Project Supervisor:  

Tony Coulson  


**INSuRE Team - Fall 2022:**

Matthew Weir 

Jed Bajarias   

Frankie Bustamante  

Irene Gil 

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
  

Erik Brasile  


Project Supervisor: 

Tony Coulson  


**INSuRE Team - Fall 2022:**  

- Matthew Weir 

- Jed Bajarias 

- Frankie Bustamante

- Irene Gil   

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
<img src=".\BLE Image\Wireshark.png" alt="Wireshark" >
</p>
<p align="center">
Figure #9
</p>

<h2 align="center">G. Issues</h2>

### Hardware:

Previously, the team had planned to use a Sengled Smart Light Bulb as part of the devices to collect data from. Unfortunately, there was no use for it as it was found that the Apple Pen, the Finite Keyboard, and the TaoTronics BLE earbuds were better fit in what Bluetooth devices one would most likely have, in a home or office setting. And as well, the researchers had noted in their proposal anticipating the issue of having all three Ubertooth Ones with their respective data outputs, since each Ubertooth One will capture data on all three primary advertising channels. In that scenario, the team had originally asked the technical directors of the project what tools we could use to group our three data capture devices, in a comprehensive dashboard for viewing. Unfortunately, the team was  unable to properly group their three Ubertooth Ones in-tandem with all their devices due to circumstances beyond their control.

### Kismet (Data Collection):

The researchers had originally used Kismet to identify the 24-bit LAP (Lower Address Part) and 8-bit UAP (Upper Address Part) in determining a BLE device, from its MAC Address packet contents. However, it was noted before that using Ubertooth One with Kismet disables Ubertooth’s channel hopping functionality, as Kismet displays firmware and software errors when changing the advertising channel to anything but 37. And  those very issues were encountered when trying to find a workaround of the problem.
This issue was mentioned to the technical directors, who stated that tshark, a terminal-version of Wireshark, might help as well as using the command of ‘ubertooth-btle -f -A 38’ to sniff out all connections to another advertising channel, like 38. Unfortunately, understanding some of the suggested tools took some time, and the technical directors had mentioned that if there was no luck in finding results of using those tools, then it was best to use what works for the team within their device set-up. Which is why the use of Kismet had to be cut along the way, due to errors using it in-tandem with Ubertooth One.

### Python (Grouping Data):

There were originally some issues with adapting the Python MAC Address Randomization Correlation scripts created by the previous CSUSB INSuRE 2020 team to work with our data sets. MAC Address Randomization is a security design in Bluetooth standards  which causes devices to replace random values of their MAC Address. This security design is implemented to prevent malicious actors from tracing a public advertising address back to a specific Bluetooth device. When BLE devices are activated, they send out what is called a public advertising packet, which contains an IEEE 802 MAC address (Jouans et al., 2). This public advertising address is used to allow scanning devices to know the identity of a device, and choose to connect to the device if desired.
The goal of adapting these Python scripts was to group Bluetooth MAC addresses of all data captured from Bluetooth devices, as they randomize, by examining the advertising packet contents. The items pulled from these packets and used by these scripts include notable information, such as the advertising address, manufacturer length, manufacturer data type, manufacturer company id, flags, flag types, and packet headers. By utilizing several of these fields, the Python script is able to convert the six raw bytes of an advertising address into a MAC address. While it may be possible to distinguish the small changes of a couple of bytes in a MAC address when it randomizes, this problem becomes much more difficult when looking at several thousands of packets at once. Without utilizing the script, it can not be determined whether the packets used in graphing through RStudio were from the devices chosen by the researchers, or other devices outside of that. Issues in understanding the code were paramount, as after some analyzing and getting the assistance from one of the former team members from the 2020 CSUSB team who wrote the script, the researchers were able to have the code adapt to their data sets after changing certain parameters. The main issue occurring with our data set was ‘unpack’ errors at several functions in the script, as seen in Figure #10. 

<p align="center">
<img src=".\BLE Image\unpack_error.png" alt="Unpack Error" >
</p>
<p align="center">
Figure #10
</p>

Many of these issues can be solved by examining the data sets and removing packets that do not meet the criteria specified to be read in the script. For example, Figure #11 shows an ideal packet makeup for running through the script. 

<p align="center">
<img src=".\BLE Image\ideal_packet.png" alt="Ideal packet" >
</p>
<p align="center">
Figure #11
</p>

Many of the packets that refuse to work with the scripts are malformed packets, which are packets that cannot be dissected further in Wireshark, which can be for a number of reasons. These types of packets may contain a packet length that cannot be processed by the script, and thus will result in an unpack buffer error. Additionally, another issue the researchers ran into using the script was the “scanning address”. While some devices may emit a scanning address, it may not always be picked up with the scanner or software being used. As a result, this function had to be dropped, and the script relied on only using advertising addresses to return a MAC address. 

### Finite & TaoTronics Scans (Patterns-of-Life)

While the researchers were able to create a Pattern-of-Life for the Apple Pencil Generation 1 device, they were unable to complete the patterns for our two additional devices. Ultimately, they were not able to determine, with 100% accuracy, if the packets captured from a device were truly from their selected devices. Many techniques were used to attempt to determine the source of packets, such as:
- Destination Address = device to iPad Mac Address
- Packets captured did not directly reveal as being connected to the iPad
- Comparing scans of several types: Static, Followed, Promiscuous
  - Promiscuous does not print out advertisements, cannot be used in script to obtain MAC address
  - Static & Followed (both captured in the Faraday bag) suffered from outside packets being picked up.
- Comparing scans of Faraday Bag to Remote Environment Scans
  - Was able to decipher most packets from not being Finite or Taotronics based, however most scans left after were either malformed or had no discernible differences between them enough to make an educated guess on which packet was from which device.
- Manufacturer IDs and MAC Prefixes
  - Both device manufacturers of Taotronics and Finite, were not listed with a MAC/Advertising prefix.
  - Bluetooth Companies can request unique identifiers made up of a few bytes, that are uniquely assigned to them by Bluetooth SIG, both Taotronics (The Sunvalley Group) and Finite (Fintie LLC) do not own one.

<h2 align="center">H. Conclusions and Recommendations</h2>

### H.1 Conclusions

As the research went to its final stages, it was concluded that while the team was able to successfully follow similar steps in creating a Pattern-of-Life analysis for their Generation 1 Apple Pencil, and had greatly learned of how Bluetooth Low Energy functions had worked in the process, the goal of refining Phase 1 of the project ultimately, was not achieved. The researchers stated in their introductions that they planned to work off previous team findings and research, in which repurposing some of that information took time to align with their intentions. After some time, an efficient base system was established for capturing BLE device traffic by using a Raspberry Pi 4 device and an Ubertooth One, along with using Wireshark and the Python scripts. This enabled the researchers to capture device traffic, identify devices and filter out unwanted packets to ultimately be used for data analysis in RStudio. However, the researchers lacked experience and time as there was much trouble in collecting, as well as testing, the data. The researchers would have liked to see further progress, if they had a more thorough understanding of the tools and methods used by the previous teams. And because they were not able to look deeply into Phase 2 due to lack of time and experience, further research is needed in regards to machine learning algorithms. Ultimately, given the research done in analyzing the methods and data from the 2020 CSUSB team and UAH, as well as lacking pertaining experience, it was a learning experience in understanding how BLE devices were tracked and identified of their packet contents. Figuring out the means of dissecting and reading how Bluetooth data works, with respect to security, was something the team had learned deeply well throughout the project.

### H.2 Future Work

Working on this project in the future would include completing some of the steps our team planned on completing as well as working towards Phase 2 of the project. One of them is managing a full scan coverage of all devices with 3 Ubertooth One devices, and finding a way to view the outputted data in some sort of comprehensive dashboard for viewing. Another task is managing a scan of three Bluetooth devices, and properly inducing anomalies in all of them, such as restarting the device while in the middle of data collection. Some devices, such as the Apple Pencil the researchers used, may not fit well to that regard because it cannot be powered off unless the device dies. As a result, an Apple Pencil would constantly send out packets and disrupt our future scans. The team is also interested in researching more methods for identifying BTLE devices outside of advertising packets, as many of the problems from the chosen off-brand devices were much harder to identify than established brands such as Apple. Whether that be through the use of different Bluetooth sniffers, or software, the team would like to be able to identify with 100% accuracy, Bluetooth devices from both name brand and generic brand Bluetooth devices. Additionally, the team would be interested in examining the BrakTooth and SweynTooth as technical methods for purposely generating anomalies in our data sets. In the future, the researchers would also like to make better use of our Raspberry Pi devices and Ubertooths, as they would like to set up a scanning environment to determine if one can spot the location of a bluetooth device as it travels around on an individual.

<h2 align="center">I. References</h2>

- É. Helluy-Lafont, A. Boé, G. Grimaud and M. Hauspie, "Bluetooth devices fingerprinting using low cost SDR," 2020 Fifth International Conference on Fog and Mobile Edge Computing (FMEC), 2020, pp. 289-294, doi: 10.1109/FMEC49853.2020.9144756.
- R. Faragher and R. Harle, "Location Fingerprinting With Bluetooth Low Energy Beacons," in IEEE Journal on Selected Areas in Communications, vol. 33, no. 11, pp. 2418-2428, Nov. 2015, doi: 10.1109/JSAC.2015.2430281.
- S. M. Beyer, B. E. Mullins, S. R. Graham and J. M. Bindewald, "Pattern-of-Life Modeling in Smart Homes," in IEEE Internet of Things Journal, vol. 5, no. 6, pp. 5317-5325, Dec. 2018, doi: 10.1109/JIOT.2018.2840451.
- Bluetooth SIG. (n.d.). 2019-Bluetooth-Market-Update [Presentation]. bluetooth.com. https://www.bluetooth.com/wp-content/uploads/2018/04/2019-Bluetooth-Market-Update.pdf
- Loïc Jouans, Aline Carneiro Viana, Nadjib Achir, Anne Fladenmuller. Associating the Randomized Bluetooth MAC Addresses of a Device. CCNC 2021 - IEEE Consumer Communications & Networking Conference, Jan 2021, Las Vegas, United States. Ffhal-03045555
- Kumar, M., & Gupta, B. K. (2015, March). Security for Bluetooth enabled devices using BlipTrack Bluetooth detector. In 2015 International Conference on Advances in Computer Engineering and Applications (pp. 155-158). IEEE.

<h2 align="center">J. Team Bio Sketch</h2>

Jed Bajarias is a 4th-year undergraduate student here at CSUSB. He was a transfer student and is now obtaining his Bachelor’s Degree in Information Systems and Technology with a concentration in Cybersecurity. From his time up to here at CSUSB, he has learned many concepts from Network Fundamentals to Ethical Hacking as well as the use of packet analysis through Wireshark, and the configuration of a Raspberry Pi. Outside of school, he’s working as a Student Assistant at the Technology Services Center at CSUSB, where he has provided troubleshooting support for hardware and software issues for many within the campus community, as well as managing the campus computer lab. He’s had experience working in teams and has participated in many projects through the school’s Cybersecurity club.

Frankie Bustamante is a current 4th-year undergraduate student at CSUSB. He is currently attending to achieve his Bachelor’s degree in Information Systems and Technology with a concentration in Cybersecurity. Frankie has previously worked with developing Bluetooth devices and networks during his NASA project and has experience in creating Raspberry Pi projects. Frankie also has experience in using Wireshark, Python, and RStudio, through various courses and school projects over the course of his education. Frankie also works in a lab located on the CSUSB campus, where he has access to electronic resources the team could use to setup and run equipment.

Matthew Weir is completing his Bachelor’s Degree in Information Systems and Technology at CSUSB. He has worked on multiple school projects involving packet capturing with tools such as Wireshark and setting up Raspberry Pi’s and configuring Linux devices. Matthew has technical experience working for the Kern County Schools as a System Support Tech, where he configures network devices, troubleshoots technical issues, and supports end users.

Irene Gil has 5 years of experience in IT and customer service and is currently working towards her Bachelor’s degree in Information Technology with a concentration on Cyber Security, at CSUSB. Irene is a transfer student from Moreno Valley College where she earned an Associate of science in business administration, and in Information systems and Technology. While at Moreno Valley college she learned networking basics, and computer hardware and worked with a team to create python scripts for vulnerability scans. She currently holds a position as an IT Apprentice for the Moreno Valley City Hall Office. Her previous position included working as a technician at the Moreno Valley Unified School District, Riverside County Office of Education, Acorn Technology Services, and Moreno Valley College. Through these experiences, she gained knowledge in Microsoft Azure, Active Directory, project management, content creation, social media management, data analysis, Microsoft Office, and Virtual Machines.
