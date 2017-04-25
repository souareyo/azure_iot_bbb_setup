Development Platform
---

|Platform | Device | Language|
|:-------:|:-------:|:-------:|
|Debian|Beaglebone Black Rev C| C |

---

Microsoft Azure Internet of things: Connecting Beaglebone Black to azure iothub
===
---

# Table of Contents

-   [Introduction](#Introduction)
-   [Step 1: Prerequisites](#Step-1-Prerequisites)
-   [Step 2: Prepare your Device](#Step-2-PrepareDevice)
-   [Step 3: Build and Run the Sample](#Step-3-Build)
-   [Tips](#tips)


<a name="Introduction"></a>
# Introduction

**About this document**

This document describes how to connect BeagleBone Black device running Debian distribution with Azure IoT SDK. This process includes the following:
-   Creation and Configuring Azure IoTHub
-   Creation and Registering  IoT device
-   Build and deploy Azure IoT SDK on device
In order to perform these  steps, the following prerequisites are required:

<a name="Step-1-Prerequisites"></a>
# Step 1: Prerequisites

-   Computer with Git client installed and access to the in order to access
    [azure-iot-sdks](https://github.com/azure/azure-iot-sdk-c)GitHub
    public repository.
-   BeagleBone Black Rev C device with.
-   SSH client on your desktop computer, if we are on linux platform there is nothing to do because SSH is available from terminal. For Windows users one can install a SSH Client such as [PuTTY](http://www.putty.org/), so you can remotely access the command line on the BeagleBone Black.
-   USB Mini cable.
-   Ethernet cable or Wi-Fi dongle.
-   [Setup your IoT hub][lnk-setup-iot-hub]
-   [Provision Beaglebone Black device and get its credentials][lnk-manage-iot-hub]

<a name="Step-2-PrepareDevice"></a>
# Step 2: Prepare Beaglebone Black Rev C Device
To perform this step, we asume that the following steps are successfully done.
-   Follow the instructions on the [beagleboard.org](http://beagleboard.org/getting-started) site to set up your BeagleBone Black device and connect it to your computer.
-   Connect your BeagleBone Black to your network using an ethernet cable or by using a WiFi dongle on the device.
-   Follow the instructions on this [wiki](http://elinux.org/Beagleboard:Terminal_Shells) to obtain your device's IP address.
-   Open an SSH terminal program, such as [PuTTY](http://www.putty.org/), on your desktop machine and connect to your device using the IP address from the previous step.
-   Connection settings:
    -   Port = 22
    -   Connection Type = SSH
-   When prompted, log in with username **root** (no password by default). You will need the username and password in case of another user.

<a name="Step-3-Build"></a>
# Step 3: Build and Run the sample with C code.

<a name="Step-3-1-Load"></a>
## 3.1 Build SDK and sample

-   From Linux terminal  or a PuTTY session one can remotely connect to Beaglebone Black Rev C device.

-   Install the prerequisite packages for the Microsoft Azure IoT Device SDK for C by issuing the following commands from the command line on your board:
		
        sudo apt-get update
        sudo apt-get upgrade

        sudo apt-get install -y curl libcurl4-openssl-dev build-essential cmake git

    ***Note:*** *This setup process requires cmake version 3.2.2 or higher.* 
    
    *You can verify the current version installed in your environment using the  following command:*

        cmake --version

    *This library also requires gcc version 4.9 or higher. You can verify the current version installed in your environment using the following command:*
    
        gcc --version 

-   Download the Microsoft Azure IoT Device SDK for C to the board by issuing the following command on the board::

        git clone --recursive https://github.com/Azure/azure-iot-sdk-c.git

-   Edit the following file using any text editor of your choice:

        azure-iot-sdks-c/serializer/samples/simplesample_amqp/simplesample_amqp.c

-   Find the following place holder for IoT connection string:

        static const char* connectionString = "[device connection string]";

-   Replace the above placeholder with device connection string you obtained in [Step 1](#Step-1-Prerequisites) and save the changes.

-   Build the SDK samples using the following command:

        sudo ./azure-iot-sdk-c/build_all/linux/build.sh

## 3.2 Send Device Events to IoT Hub

-   Run the sample by issuing following command:

        azure-iot-sdk-c/cmake/iotsdk_linux/serializer/samples/simplesample_amqp/simplesample_amqp

-   See [Manage IoT Hub][lnk-manage-iot-hub] to learn how to observe the messages IoT Hub receives from the application.

## 3.3 Receive messages from IoT Hub

-   See [Manage IoT Hub][lnk-manage-iot-hub] to learn how to send cloud-to-device messages to the application.


<a name="tips"></a>
# Tips

-   If you just want to build the serializer samples, run the following commands:

        cd azure-iot-sdk-c/cmake/iotsdk_linux/serializer/samples	
        make -f Makefile all


[lnk-setup-iot-hub]: ../setup_iothub.md
[lnk-manage-iot-hub]: ../manage_iot_hub.md
