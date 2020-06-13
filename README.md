# ITRY SCDF IBM Challenge 2020
This repository contains the files neccessary for the description of the project as well as installation guides.

## Contents

1.[Short Description](#Short-Description)

2.[Pitch Video](#Ptich-Video)

3.[Architecture of project](#Architecture-of-project)

4.[Detailed Description](#Detailed-description)

5.[Prerequisites](#Prerequisites)

6.[Getting started](#Getting-started)

7.[Test Results](Tests-results)

8.[Live Demo](#Live-Demo)

9.[Built With](#Built-with)

10.[Authors](#Authors)

11.[Acknowledgements](#Acknowledgements)

## Short Description
### 1.1 What's the problem ? 
With the increasingly aging population and a growing segment of vulnerable populations specifically the increasing trend of elderly with no next of kin, Community First Responders (CFRs) must be alerted at the onset of incidents which require emergency response (e.g. cardiac arrests, falls, unattended cooking fires etc.) and mobilise CFRs for effective early intervention. Meaning to deploy the CFRs when an elderly person falls or when an unattended stove becomes a cooking fire. CFRs work closely with SCDF to provide timely relief and response to emergency situations.

### 1.2 How does technology help?
With the advancement of technology and transformation of data, effective early interventions can be built in place through the usage of analytical data for better sense-making decisions at the onset of incidents to provide emergency response from CFRs. IOT devices have been developed to collect and transmit data from the device to the cloud for analytics and visualisation.

### 1.3 Idea of project
Our team has decided to make use of Internet of Things (IOT) devices to collect data, transmit data to the cloud and make use of IBM Watson Studio to analyse and visualise the data to SCDF in order to improve their sense-making to be alerted at the onset of incidents which require emergency response and mobilise the CFRs for effective early intervention for the elderly population.

## Pitch video

## Architecture of project
![Architecture of project](https://github.com/Bet365619/ITRY/blob/master/Timeline/Architecture-of-Project.jpg)


## Detailed description
[More detail is available here](DESCRIPTION.md)
## Prerequisites
1. An IBM Cloud account; if you do not have an existing IBM Cloud account, [start your free trial](https://cloud.ibm.com/registration?cm_sp=ibmdev-_-developer-tutorials-_-cloudreg). Learn more about IBM Cloud by reviewing the [Getting Started documentation](https://cloud.ibm.com/docs).
2. Download and install the [IBM Cloud CLI and Developer Tools](https://cloud.ibm.com/docs/cli?topic=cli-getting-started).
3. A smartphone (an Android or iOS device)

## Getting started
### Step by step guide to build the analytical device
#### Step 1 Creating an IOT app in IBM cloud
Work through the steps in this tutorial to create a [Node-RED and Watson IoT Platform starter app in IBM Cloud](https://developer.ibm.com/tutorials/how-to-create-an-internet-of-things-platform-starter-application/).

As a result, you will have a Node-RED Starter Kit application connected to the IBM IoT platform.As a result, you will have a Node-RED Starter Kit application connected to the IBM IoT platform.

### Step 2 Add a device that will send MQTT messages to the IBM Watson IoT Platform
1. After completing the setup in step 1, the  IBM Watson IoT Platform console is opened.
![IOT Platform](https://github.com/Bet365619/ITRY/blob/master/Setup_IMG/IOT/IOT-Platform.jpg)
An organisation id is being assigned to your app, as shown in the picture labelled as 1.
![IOT-Label1](https://github.com/Bet365619/ITRY/blob/master/Setup_IMG/IOT/IOT-1.png)

In this case, the organisation id is pu3272 which is located at the top right corner of the dashboard. 

2. Click Add Device Type. In your organization, you can have multiple device types each with multiple devices. A device type is a group of devices that share characteristics; for example, they might provide the same sensor data. In our case, the device type name must be “Android” (this device type name is required by the app that you will use later).

3. Click Next. A page is displayed where you can enter metadata about the device type, such as a serial number or model. You don’t need to specify this information for this tutorial. Just click Finish.
![IOT-label2](https://github.com/Bet365619/ITRY/blob/master/Setup_IMG/IOT/IOT-2.png)

4. Click Register Devices. Enter the device ID. The device ID can be, for example, the MAC address of your smartphone. However, it must be unique within your organization only. For example in this instance, the device ID is "andriodchris".
![IOT-label3](https://github.com/Bet365619/ITRY/blob/master/Setup_IMG/IOT/IOT-3.png)
5. Click Next. A page is displayed where you could enter metadata about the device. Leave it blank, and click Next.

6. On the security page, enter a value for the authentication token. Remember this value for later. Then, click Next.

7. Messages are now ready to be sent from registered device to IOT platform.

### Step 3 Downloading and installing App on mobile device

You will use the IoT Starter for Android app to read and send sensor data on your smartphone. The source code and documentation of the app are in the [iot-starter-for-android GitHub project](https://github.com/ibm-watson-iot/iot-starter-for-android). The [Apk installation file](https://github.com/deveops/iot-starter-for-android/releases) for andriod devices can be found here.

### Step 4 Allow permission of IOT starter on mobile device
1. Go to Settings on mobile phone.

2. Go to Application Management. ![Setting-1](https://github.com/Bet365619/ITRY/blob/master/Setup_IMG/Settings/Settings-1.png)

3. Search for application called IOT Starter. ![Setting-2](https://github.com/Bet365619/ITRY/blob/master/Setup_IMG/Settings/Settings-2.png)

4. Go to Permissions. ![Setting-3](https://github.com/Bet365619/ITRY/blob/master/Setup_IMG/Settings/Settings-3.png)

5. CLick on allow "location" to allow data to flow. ![Setting-4](https://github.com/Bet365619/ITRY/blob/master/Setup_IMG/Settings/Settings-4.png)

6. Turn on share "location" before starting application. ![Setting-5](https://github.com/Bet365619/ITRY/blob/master/Setup_IMG/Settings/Settings-5.png)

### Step 5 Configuring the mobile device
1. Start the IoT Starter app.
2. Click Skip tutorial.
3. Enter the following parameters:
Organization: The organization ID that was displayed on the IBM IoT server at the top right corner of dashboard. For example, pu3272 in this tutorial.
Device ID: The device ID that you configured above. For example, “andriodchris” in this tutorial.
Auth Token: The authorization token that you specified earlier.
Make sure that USE SSL is checked.
![Login](https://github.com/Bet365619/ITRY/blob/master/Setup_IMG/Settings/Login.png)
Upon clicking on Activate Sensor, the app collects data from the acceleration sensor in your smartphone and sends the data to the IBM IoT server. The app displays the accelerometer data and the number of messages that were published or received.
![Sensor-data](https://github.com/Bet365619/ITRY/blob/master/Setup_IMG/Settings/Sensor-Data.png)



Step 5

Step 6

Step 7

### Software to required
Jupyter Notebook

RStudio

IBM Watson Studio

IBM Node-Red

## Test results

## Live Demo 

## Built with
* [IBM Cloudant](https://cloud.ibm.com/catalog?search=cloudant#search_results) - The NoSQL database used
* [IBM Cloud Functions](https://cloud.ibm.com/catalog?search=cloud%20functions#search_results) - The compute platform for handing logi
* [IBM IOT platform](https://cloud.ibm.com/catalog/services/internet-of-things-platform) -  The hub for IBM Watson IoT and lets you communicate with and consume data from connected devices and gateways
## Authors 
* **Rui Jie** - *Bet365* 
* **Ismail** - *Bet365*
* **Yu Da** - *Bet365*
* **Zhi Hao** - *Bet365*


