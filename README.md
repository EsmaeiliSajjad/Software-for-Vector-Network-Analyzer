# Software-for-Vector-Network-Analyzer
In this project, an automation software is designed to change the setting and configuration of a vector network analyzer and save the data for furthur data analysis. The data can be stored in SQL software as a large number of data will be generated for a measurement.
# Table of Centent
1. [Description](#1)
2. [LabView Code](#2) 
3. [Upgrades](#3)

<a name="1"></a>
# Description
Here we are sharing an experience with automation and instrumentation, especially for software development, to monitor and control a Vector Network Analyzer, SIGLENT SVA-1032X. In the following video, a designed software was capable of controlling the following options, through a TCP/IP protocol by introducing IP to the server and the instrument:
1. Monitor the sending and receiving signals.
2. Control start and stop frequency between, besides other settings such as Meas and Stimulus, Format, Scale, Track, etc.
3. Fast Data Log option.
4. Save data and generate the report in a form of a formatted text file, at a desired period of time with a specific time interval. The data file includes data/time, instrument serial number, instrument model, mode of measurement, signal specifications, and other relevant parameters for the measurement.
5. Plot the signal amplitude as a function of frequency or within the Smith chart.
This is simple software and can be upgraded for other applications.

(https://user-images.githubusercontent.com/108043716/177027473-95ea5dea-e7f2-4646-abad-8217d68bbe0d.png) 

Fig. 1: LabView code for the software.

<a name="2"></a>
# Required Devices

<a name="3"></a>
# Upgrades
The designed circuit board in this project is able to control up to 12 Relay Output channels. However, another version for 24 channels is also designed. Also, to support a high-amp device (e.g. Vacuum pump), you can change the type of relay to achieve this goal.
