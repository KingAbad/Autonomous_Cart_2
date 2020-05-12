# Project - Autonomous cart

Autonomous cart was one of the 3 main projects of the subject **Project Reasearch** given by several professors of the university-college **PXL**. The main goal of Autonomous cart was to turn a ordinary golf cart into a fully self-driving campus taxi that takes it passengers to their desired locations. The three main technologies that were needed to make this project a succes were: IOT, AI and Automation technology. As of our task to be the brain of this project it was our main responsibility to the IOT side of this project. And that is also what this repository is about.  


## Source Roadmap

```
RFID_Project_Arduino    directory containing RFID system with Arduino files
RFID_Project_PSoC4      directory containing RFID system with PSoC4 files
RFID_Project_STM        directory containing RFID system with STM files
TCP_IP_JETSON_PLC       directory containing Server (twincat) and Client (python) code
PCB_ACTUAL              directory containing all of the Altium designs for the main pcb
PCB_RELAIS7-4           directory containing all of the Altium designs for the relais pcb
Data_Visualisation      directory containing the script to show csv content on webpage
Website                 directory containing all the html code and php scripts for the website
Presentaties            directory containing all of the powerpoint presentations given during this project
```

## All of the projects made by our group
<details> 
 
<summary>Click to see all projects</summary>
  
## RFID project with Arduino

<details>
<summary>Click to expand the RFID project with Arduino</summary> 

**Poject requirements**
* Jumper wires
* RFID-RC522
* RFID tags
* IIC LCD-Display
* Buzzer module
* RGB led
* Breadboard
* Arduino IDE
* Arduino

**Step by step guide**
* Open the Arduino IDE. 
* Plug in your Arduino Nano (used by me) in your laptop.
* Start making your circuit (open my schematic).
* Copy and paste the my .ino code in your IDE.
* Look if you have the right board selected.
* Also select the right serial COM port your Arduino is connected to.
* Upload the code into your Arduino and it should work.

**Note:**
 You have to change the UID of mine tag to the UID of your tag.
To know this UID open one of the simple RFID-RC522 reading examples in the Arduino IDE.
</details>  

## RFID project with PSoC4

<details>
<summary>Click to expand the RFID project with PSoC4</summary> 
 
 **Poject requirements**
* Jumper wires
* RFID-RC522
* RFID tags
* IIC LCD-Display
* Buzzer module
* RGB led
* Breadboard
* PSoC Creator 4.2
* PSoC 4

**Step by step guide**
* Open the PSoC Creator 4.2 download available at the official cypress site. 
* Import my project in the ide.
* If you are using a different PSoC you might have to change the target device and pin settings.
* Plug in your PSoC 4 (used by me) in your laptop.
* Start making your circuit.
* Clean and build the project once.
* Upload the code into your PSoC 4 and it should work.

**Note:**
 This code is made to work with any **RFID-tag** it just detects wheter any tag is detected by the reader or not.
 With some minimal changes to the code you can make it work for a certain specific tag.
</details> 

## RFID project with STM

<details>
<summary>Click to expand the RFID project with STM</summary> 
 
 **Poject requirements**
* Jumper wires
* RFID-RC522
* RFID tags
* IIC LCD-Display
* Breadboard
* STMCubeIDE 1.3.0
* STM32xxxx µController

**Step by step guide**
* Open the  STMCubeIDE 1.3.0 download available at the official st.com site. 
* Import my project in the IDE.
* If you are using a different STM you might have to change device with the board selector.
* Plug in your STMµController into your laptop.
* Start making your circuit.
* Clean and build the project once.
* Upload the code into your STMµContoller and it should work.

**Note:**
 You have to change the UID of mine tag to the UID of your tag.
To know this UID open one of the simple RFID-RC522 reading examples in the Arduino IDE.
And use it afterwards in the code. If you don't have the Arduino IDE then donwload an RFID reader
app on your smartphone it should work if your device supprots NFC.
</details> 

## TCP-IP communication between Jetson and PLC

<details>
<summary>Click to expand the TCP-IP communication between Jetson and PLCs</summary> 

 **Poject requirements**
* Jetson Nano
* Jetson Nano display
* Twincat 3 V4024.7

**Step by step guide**
* Open the Twincat XAE or open it in Visual Studio.
* import the Twincat [server program](KingAbad/Autonomous_Cart_2/TCP_IP_JETSON_PLC/TwinCAT_Program/TCP_Server) in your solution.
* Go on the Jetson Nano terminal and install python3.
* First run the PLC server 
* now run the [client program](Autonomous_Cart_2/TCP_IP_JETSON_PLC/tcp_client.py).
* Now you should be able to see incoming messages in the server that you sent with the client.

**Note:**
 TwinCAT Error and Error ID are stored in the variable 'err' and 'errid' respectively. Some common errors found:
  * 8002 : Variable 'hSocket' is not populated with the correct address. The sequence is for the TwinCAT to call FB_SocketListen, the Python client to connect, and TwinCAT calls the FB_SocketAccept after that. This will populate the variable 'hSocket'. If FB_SocketAccept is called before the Python client trying to connect, it will throw 8002 error.
 * 8003 : The port is already opened. Reset Cold the TwinCAT program and Run again.
 * 6 : I don't know. Seems like there's something wrong with the installation of TF6310. Uninstall, reinstall, make sure that     TcpIpServer.exe is running in your Task Manager processes.

</details> 

## PCB design using Altium

<details>
<summary>Click to read details about the PCB design using Altium</summary> 
  
</details> 

## Data visualisation

<details>
<summary>Click to expand the Data visualisation project</summary> 
  
</details> 

## Website

<details>
<summary>Click to expand the Website details</summary> 
  
</details> 


</details> 
