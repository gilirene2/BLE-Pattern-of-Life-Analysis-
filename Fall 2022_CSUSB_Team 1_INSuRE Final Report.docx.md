<h1 align="center">FINAL REPORT</h1>

<h2 align="center">Pattern-of-Life Analysis and Deviations for Bluetooth and Bluetooth Low Energy Devices</h2>
<img src="CSUSB_logo.png" alt="CSUSB Logo">
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

The goal is to use previously researched tools and findings to capture and analyze BLE packets, then create a Pattern-of-Life analysis that will help to better understand the way Bluetooth Low Energy functions. Through understanding of BLE functions and packet behavior, BLE security is also better understood. Reviewing prior INSuRE work to this project, the researchers found the 2020 team from California State University, San Bernardino (CSUSB) and the teams from the University of Alabama in Huntsville (UAH) as best fit for the goal the researchers are aiming to achieve. However, since the team will analyze and build up research from those previous teams, there is a matter of differing knowledge and experience, as those teams had more relevant skills pertaining to the project at hand. Despite this, they hope to utilize...
