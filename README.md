# Amazon-Echo-Dot-and-Raspberry-Pi.
By connecting Amazon Echo Dot and Raspberry Pi, we can exercise voice control over devices connected to the microcontroller.


# Installing Raspberry Pi and Interfacing Amazon Echo Dot.
The Raspberry Pi is a series of small single-board computers, developed by Raspberry Pi Foundation, that plug into a computer monitor or TV, and use a standard keyboard and mouse. It is a dynamic microcontroller with a wide variety of applications. Amazon Echo is a category of devices designed to enable customers to interact with Alexa, Amazon’s voice service, and ask for news, music, weather etc. By interfacing Amazon Echo Dot to Raspberry Pi, we can exercise voice control over devices connected to the microcontroller.

## Steps to Set up Raspberry Pi:
1	Download "RASPBIAN STRETCH WITH DESKTOP" and unzip "2018-04-18-raspbian-stretch.zip" Ref:https://www.raspberrypi.org/downloads/raspbian/.  
2	Download "win32diskimager-1.0.0-install.exe" program from following URL Ref:https://sourceforge.net/projects/win32diskimager/files/latest/download.  
3	Install "win32diskimager-1.0.0-install.exe".  
4	Connect micro-sd card to computer. Write raspbian-stretch image file onto micro-sd card using “Win32DiskImager”.  
![writing](https://user-images.githubusercontent.com/39903083/41076797-f7d8c800-6a30-11e8-96b1-37e3a949abf1.jpg).  
5	Once image writing is completed, create "ssh" (ssh file is empty) files to the root of the sd card.  
6	Insert the sd card into Raspberry Pi 3 and boot it.  
7	Connect Ethernet cable to the Raspberry Pi3.  
8	Search for the IP address of Raspberry Pi3 using advanced ip scanner                                                     Ref: https://www.advanced-ip-scanner.com.  
9	Download PuTTY  Ref: https://www.putty.org/.  
10	Insert IP address of Raspberry Pi3 into host name.  
11	In command window login with id as “pi” and password as “raspberry”.  
 
        






12	Type "sudo raspi-config" and go to "Interfacing Options" and enable SSH and VNC.  
13	Type “vncserver” into command line.  
14	Download VNC client  Ref: https://www.realvnc.com/en/connect/download/vnc/windows/.  
15	Open VNC client and insert IP address of Raspberry Pi.  
16	Login with user name "pi" and password "raspberry". Now Pi3 desktop can be viewed.  
17  Type the following two commands in Pi command prompt to update it. "sudo apt-get update"    and "sudo apt-get upgrade".  
## Steps to interface Amazon echo dot to Raspberry Pi  
1.	Download this github project as zip file with following command "wget https://github.com/nassiramalik/IOT-Pi3-Alexa-Automation/archive/master.zip".  
2.	Unzip downloaded zip file with "unzip master.zip" command and type "cd IOT-Pi3-Alexa-Automation-master" command after unzip completes.  
3.	Enter "sudo python3 RPi_name_port_gpio.py" command to run Pi IOT program.  
4.	Give voice command to Alex to discover devices "Alexa discover devices" it will search your network and discover your Raspberry Pi 3 as an IOT device.  
5.	 Connect GPIO pins to devices (here LED’s).  
 
 
6.	Give a voice command to Alexa "Turn on Kitchen" and led will turn on.  
7.	Give a voice command to Alexa "Turn off Kitchen" and led will turn off.  
 
8.	Similarly we can choose to command other devices listed in the code.  
Therefore, we see that connecting Amazon echo dot and raspberry pi gives a whole new dimension to the use of microcontrollers in home automation. Having familiarized with the basics, we proceed to the project using raspberry pi.  
