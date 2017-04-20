---
platform: debian
device: beaglebone-black
language: C
---

# azure_iot_bbb_setup
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









