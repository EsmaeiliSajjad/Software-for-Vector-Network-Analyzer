# Software-for-Vector-Network-Analyzer
In this project, an automation software is designed to change the setting and configuration of a vector network analyzer and save the data for furthur data analysis. The data can be stored in SQL software as a large number of data will be generated for a measurement.
# Table of Centent
1. [Description](#1)
2. [LabView Code](#2) 
3. [Upgrades](#3)
<a name="1"></a>
# Description
Here we are sharing an experience of automation and instrumentation, especially for software development, to monitor and control a Vector Network Analyzer, SIGLENT SVA-1032X. In the following video, a designed software was capable of controlling the following options, through a TCP/IP protocol by introducing IP to the server and the instrument:
1. Monitor the sending and receiving signals.
2. Control start and stop frequency between, besides other settings such as Meas and Stimulus, Format, Scale, Track, etc.
3. Fast Data Log option.
4. Save data and generate the report in a form of a formatted text file, at a desired period of time with a specific time interval. The data file includes data/time, instrument serial number, instrument model, mode of measurement, signal specifications, and other relevant parameters for the measurement.
5. Plot the signal amplitude as a function of frequency or within the Smith chart.



https://user-images.githubusercontent.com/108043716/177027855-694a34ad-095b-42a3-a135-3c044f1bce77.mov



<a name="2"></a>
# LabView Code
LabView software is employed here to write the code. Before running the code, you should introduce the device to the computer and connect it using NI-Max software. You also have to configurate the TCP/IP protocol for data communication between the PC and the instrument. The following is a part of the code developed for the softare.

![Screenshot 2022-07-03 001542](https://user-images.githubusercontent.com/108043716/177027512-f4d8cf2d-6325-4513-91e3-ba1b8de7cca6.png)

Fig. 1: LabView code for the software.

In order to communicate between the PC and instrument, you should be familiar with buffer read and write concept. In addition to this, the proper command should be specified to be sent to the instrument. Some of these commends do not return any value; however, additional string functions should be added to the code to properly encode the return buffer.
<a name="3"></a>
# Upgrades
This is simple software and can be upgraded for other applications. For example, you can enable the tracking of signal or other options of Vector Network Analyzer.
