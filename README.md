---
platform: debian
device: beaglebone Black Rev C
language: C
---

Microsoft Azure Internet of things: Connecting Beaglebone Black to azure iothub
===
---

# Table of contents

-   [Introduction](#Introduction)
-   [Device Setting up](#DeviceSettingup)
-   [Beaglebone setup][lnk-beaglebone_azureiot_connect]
-   [Create and manage Iothub][lnk-Setup_and_manage_iothub]
-   [IoT Suite monitoring solution][lnk-iot_suite_remote_monitoring_solution]
-   [IoT Suite Preconfigured monitoring solution][lnk-remote_monitoring_preconfig_solution]
-   [ IoT Suite monotoring solution with physical devices][lnk-remote_monitoring_with_physical_devices]

<a name="Introduction"></a>
# Introduction
This document presents an introduction of Microsoft azure internet of things and how to connect and remotly control data from device such as beaglebone Black Rev C. The document that highlith the outlines of the document can be found [iot presntation][lnk-iotslides] 

<a name="DeviceSettingup"></a>
 # Device Setting up

In  order to connect your device to  azure Internet of Things (IoT), we must create and manage an azure iot hub instance. Therefore in the this documentation, I will explain a Step-by-Step description of  a creation of an  azure Iot hub instance, how to manage it and how to connect a specific device on iothub such as Beaglebone Black (BBB).
There are several ways to create an azure iothub depending on the working environment or platform (Linux, Windows, Mac ),the developers preferences and the type of device (Windows or Linux). The following list  Will show the difference methods used to create an iothub.
Azure portal
Azure CLI  for Python Command line
Azure powershell
Visual Studio C# using NuGet Package manager.

The step-by-step description to create an iothub can be found  here (link will comme here).

Manage an Iot hub

Having created an iothub, we can perform the folling operations:

Device ( Creation, deleting)
Rettrive the device crediential
Device registry credential 
send Device-to-Cloud messages 

Create Device:

One can use either iothub-explorer or a Device-explorer. The first one is cross-platform and second one is designed for windows only. Both of these methods, one can use the following languages:

C#

Java

Python

NodeJs

JavaScript.


Device setting
In order to connect the device iothub, the following tools are required:
Real Device in our case Beaglebone Black Rv C
A  16 GB of a microSD Card
Ethernet cabel
USB cabel to power the Beaglebone

A sensor tag (Temperature, pressure sensor and so on.. ).

In order to connect to the device, we will need its IP address to get it I used CLOUD IDE, which is an integrated IDE in Beablebone. IP address is used to remotely connect to Beaglebone via Putty, which can be download here.








[lnk-beaglebone_azureiot_connect]: ./beaglebone_azureiot_connect.md 
[lnk-Setup_and_manage_iothub]: ./Setup_and_manage_iothub.md
[lnk-iot_suite_remote_monitoring_solution]: ./iot_suite_remote_monitoring_solution.md
[lnk-remote_monitoring_preconfig_solution]: ./remote_monitoring_preconfig_solution.md
[lnk-remote_monitoring_with_physical_devices]: ./remote_monitoring_with_physical_devices.md
[lnk-iot-present]: ./azure_iot_demo_1.pdfd



