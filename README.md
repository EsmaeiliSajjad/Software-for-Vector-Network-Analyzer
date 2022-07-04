# Software-for-Vector-Network-Analyzer
In this project, automation software is designed to change the setting and configuration of a Vector Network Analyzer and save the data for further data analysis after measurement. The data can be stored in any database, such as SQL software since a large number of data will be generated for a single measurement. The data should be classified based on the measuring technique, frequency range, output type, Meas, and format, type of data. Every measurement can generate more than 300 data points.

# Table of Centent
1. [Description](#1)
2. [LabView Code](#2) 
3. [Upgrades](#3)
<a name="1"></a>
# Description
In this project, we are sharing an experience of automation and instrumentation, especially for software development, to monitor and control a Vector Network Analyzer, SIGLENT SVA-1032X. In the following video, a designed software was capable of controlling the following options, through a TCP/IP protocol by introducing IP to the server and the instrument:
1. Monitor the sending and receiving signals.
2. Control start and stop frequency between, besides other settings such as Meas and Stimulus, Format, Scale, Track, etc.
3. Fast Data Log option (less than 1 sec for reading/writing/storing).
4. Save data and generate the report in a form of a formatted text file, at a desired period of time with a specific time interval. The data file includes data/time, instrument serial number, instrument model, mode of measurement, signal specifications, and other relevant parameters for the measurement.
5. Plot the signal amplitude as a function of frequency or within the Smith chart.

https://user-images.githubusercontent.com/108043716/177027855-694a34ad-095b-42a3-a135-3c044f1bce77.mov

Fig. 1: Testing developed software for automation of SIGLENT Vector Network Analyzer.
<a name="2"></a>
# LabView Code
LabView computer coding software is employed here to write the code. Before running the code, we should introduce the device to the computer and connect it using Measurement and Automation Explorer (NI-MAX) software. We also have to configure the TCP/IP protocol for data communication between the PC and the instrument. The following figures show how to connect the instrument to the PC through NI-MAX software and also a part of the developed code.

![Screenshot 2022-07-03 001542](https://user-images.githubusercontent.com/108043716/177027512-f4d8cf2d-6325-4513-91e3-ba1b8de7cca6.png)
Fig. 2: LabView code for the automation software including control, monitor, and store data in formatted data file. 

<img src="https://user-images.githubusercontent.com/108043716/177028184-68b5754b-b804-4649-b808-9075ad1251cc.png" width="800" />

Fig. 3: Defining the instrument to computer in NI-MAX software. 

In order to communicate between the PC and instrument, you should be familiar with the buffer read and write concept. In addition to this, the proper command should be specified to be sent to the instrument. Some of these commands do not return any value; however, additional string functions should be added to the code to properly encode the return buffer.
<a name="3"></a>
# Upgrades
This software can be upgraded for other applications. For example, you can enable the tracking of signals or other options of Vector Network Analyzer.
