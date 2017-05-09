# Fast prototyping of IoT with Azure and Beagle Bone Black 
Microsoft's Azure is the powerful cloud computing Platform, which provides different services. One of these services is Internet of Things (IoT). One can define IoT as a kind of network of Devices or  almost everything, which are connected together and communicating via cloud. These things or devices perform some tasks without human-to-human or human-to- devices interaction. In this fast prototyping, we will investigate '''Beaglebone Black Rev C'' capabilities to send message or data to cloud IoT hub.  Before we start our fast prototyping, In what follows, we will  briefly explain the concept behind Microsoft Windows Azure itself and the core concept of internet of things.
### What is Ms Azure ? 


As I mentioned, MS Azure is cloud based cross-platform. There is no mater if you are working on Linux, windows or Mac you are comfortable with C, C#, Java, JavaScript or Python you will always be fine with Azure. If you are  Working with a single or multiple VM environment, Azure is a good choice. If You are Database architect, Database  Administrator, SharePoint Server administrator or SharePoint superuser, MS BI Developer or a kind of Data scientist or machine learning architecture Ms Azure is your Platform. With MS Azure, Developing and hosting a critical rich Web and mobile  applications become a mater of minutes. Ms Azure, with its Internet of Things (IoT), IoTbub and IoT suite, the millions of devices are remotely connecting and communicating  each other by performing certain tasks without requiring  human-to-human or human -to- computer interaction. This simply make our everyday life easier than before. For more info about Microsoft Azure try this link [Azure](https://azure.microsoft.com/en-us/?v=17.14)

# Concept of our IOT setup 

As I mentioned, our Device is A Beaglebone Black, which we will first try to connect with IoT hub and try send messages ''' device -to- iot hub and ioT hub -to- device'''. Then we will use some sensors, which data will be sent to BBB then to cloud via iot suite.

As you can see it is little confusing  at this point because I interchangeably write ''' IoT ''' and  '''IoT Suite'''. But what these two  concepts really mean?.

## IoT Hub 
IoTbub is the core concept of internet of things,it is a kind of bridge between cloud and devices (every thing, any thing, any device). Technically, IoThub is a '''gateway protocol '''  between devices and cloud. Any device that want to communicate via cloud must past by an IoThub instance.

## IoT Suite 
IoT Suite contains IoThub and it is used to gathering all the info from devices for the presentation via web app on azure platform.   

The sketch the  physical architecture of internet of thing can be seeing in following figure:

# Step 01 - Tools needed for our prototyping 
The this fast prototyping, we will need the following Development tools:

## Tools Provided by Azure platform 
Of course, MS Azure licence or account  gives access to all the tools available on the MS Azure Platform, we just need to configure them in our code.
For our IoT, we will use the following list of tools.

* '''Azure SDKs'''
    *''' Azure IoT Device SDK'''
    *''' Azure IoT Service SDK''' 
    *''' Azure Powershell '''

*'''Packages'''

We will also need the target Device and some sensors in the our case, we will need the following elements:

''' Beaglebone Black ''' connected to internet,

''' A microSD card and sensortag ''''


Explain which development tools we will need for this work and why we will need them.

## Needed tools on development Machine 
In order to connect to MS Azure Database or perhaps Develop Web App   and deploy it to azure cloud services , We will need the following Tools:
* A SQL Server management studio 2016 (SSMS).

* Visual studio at least  community 2015.

* Windows 10

* Windows Poweshell (Optional)

* Microsoft azure Powershell

# Step 02 - Configure Azure Account 

Of course one can create one of Microsoft free account and use use Microsoft azure in 30-days but Microsoft azure account setting is more complicated than a simple free account assigning. To take control over all Microsoft Azure Account problem, we will make a parallel between three the following accounts:
## Microsoft Azure Account # = Microsoft Account ## === Microsoft organization Account  Step 03 - Connect Device to Microsoft Azure IoT ==

In order to connect the Device to Microsoft Azure Internet Of Things, the following steps have to be successfully performed:

* Create an azure account by visiting [Microsoft azure](https://azure.microsoft.com/en-us/?v=17.14) if your organisation doen't have an azure account.
* Create and manage IoThub instance. One can  create an IoThub in following methods:[Create Iothub](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-create-through-portal)
* Setup and configure Beaglebone Black  for more info on Beaglebone upsetting go to [ beaglebone.org](http://beagleboard.org/)
* Build SDK on Device go to my github repository [github repos.](https://github.com/souareyo/azure_iot_bbb_setup)
* Create and azure IoT Suite remote monitoring solution [github repos.](https://github.com/souareyo/azure_iot_bbb_setup)

# Step 04 - Use GSM cape 

Install a GSM cape like "http://ciudadoscura.com/beaglebonecape/" on BBB and use this device to make our IOT setup work when "unplugged".
