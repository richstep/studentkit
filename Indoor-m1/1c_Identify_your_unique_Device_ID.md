Connect the Rasberry Pi to the Internet and Obtain its Unique Device ID
=============================

Before you can register your Microsoft FarmBeats Student Kit with the Microsoft Azure IoT cloud service, you first must identify your
device's unique ID and then follow the registration process on the FarmBeats web
portal.

To gather the device ID you must connect your device to the Internet, identify
its IP address to access Windows IoT Dashboard and then locate the device ID.

The following steps will guide you through this process.

## 1. Preparation
-----------

-   Gather the Raspberry Pi, ethernet cable, micro USB cable, and power adapter
    from the FarmBeats student kit.

-   Verify that a micro SD card is already inserted in the Raspberry Pi. If not,
    please refer to the Assemble your FarmBeats Student Kit Hardware guide
    before continuing with this process.

![](media/c610a04f4848eca9a1f43db8e611cc4a.png)

## 2. [Install the Windows 10 IoT Dashboard](http://go.microsoft.com/fwlink/?LinkID=708576)

- A file named setup.exe should have downloaded. Now install it. After it installs, notice in your Windows start menu a new program named "Windows IoT Core Dashboard".
- Run the Windows IoT Core Dashboard. A window will open showing a list named "My devices". The list will be empty.
 
## 3. Connect the Raspberry Pi to the Internet
--------------------------

There are multiple options to getting your Raspberry Pi online and reachable by
your PC. It’s essential to have your Raspberry Pi and PC connected to the same
network.

*Note: Internet connectivity and device to device communication is the area that
often requires the most troubleshooting. See Known Issues and Frequently Asked
Questions if you are having issues getting your device online.*

-   **OPTION 1: Use an ethernet hub or switch** – Plug one side of the ethernet cable into
    the Raspberry Pi and the other into the same ethernet hub or switch that
    your wired (not WiFi) PC uses. 

![](media/75e575255504adca7f94b162988289f7.png)

-   **OPTION 2: Use the device that your ISP gave you. A DSL or cable modem.** – Plug one side of the ethernet cable into
    the Raspberry Pi and the other into an extra eternet port on the back of your DSL/cable modem. Most likely laptop is using WiFi via the DSL/cable modem. 

-   **OPTION 3: To connect with a Wi-Fi connection** – follow the steps later in this
    document.


## 4. Power on the Rasberry Pi device
--------------------

-   Plug the large end of the micro USB cable into the power adapter and insert
    power adapter into a power source

-   Plug the small end of the micro USB cable into the Raspberry Pi and Power
    Up! A red light should shine on the motherboard.

![](media/d21ffa84ab8122ea6453101970a803a3.png)

## 4. Obtaining the Raspberry Pi's unique device ID
--------------------
- Return to thee Windows IoT Core Dashboard at you installed an ran in step 2. 
- You should now see one device listed.

1. Right-click on the device and select "Open in Device Portal".
2. A web browser will open and will connect to the Raspberry Pi. This website, called the Windows Device
    Portal, lets you configure and manage your device remotely over your local
    network.
3. Login to Windows Device Portal using the username **administrator** and the
    default password
    **p\@ssw0rd**

-   Select **Connectivity** on the menu on the left, then Select **Network**

![](media/ff0b13a743e48640294ac95382bded13.png)

-   On the right-hand side of the screen are listed all the types of network
    connections on the Raspberry Pi. Look for the one that starts Record the
    Physical address of your **LAN** card.

![](media/8ab91e1fd79ce95e31b7d0c8f64f4b1e.png)

-   Look for the one that starts with LAN and record the **Physical address,
    without the dashes in between.** This is your unique device ID that is used
    as the claim code for device registration on the Student Kit Portal. In this
    example the **Device ID** is **b827eb653aba**

4. Write this Device ID down for later use when you need to register in the Azure Cloud.


Next Steps
----------

Next steps are to [install the FarmBeats Sensor Application Software](https://github.com/richstep/studentkit/blob/master/Indoor-m1/1d_Install_the_FarmBeats_Sensor_Application_Software.md) onto the
Raspberry Pi.
