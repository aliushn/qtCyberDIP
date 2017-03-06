# qtCyberDIP
![CyberDIP](/pic/CyberDIP.JPG)

CyberDIP driver for windows in C++ 11.

CyberDIP is a USB device clicking touchscreens of smartphones or pads under PC's control. 
With the help of [grbl](https://github.com/grbl/grbl) running on an Arduino Nano, CyberDIP will translate serial port signals from your PC into 2D-motion and clicks.

本工程是由C++ 11编写的CyberDIP在Windows环境下的配套驱动。

CyberDIP是通过计算机USB控制的触摸屏点击设备，通过搭载[grbl 0.8c/0.9j](https://github.com/grbl/grbl)驱动的Arduino Nano(ATmega328)控制器，CyberDIP可以将USB串口发来的指令翻译成相应的二维运动与点击操作，模拟单指对屏幕的操作。

***
###TODO
* Find solution to replace Airplayer.exe+PrintScreen


###Depends
* Qt 5.7
* FFmpeg 2.2.2	(included in [/3rdparty](/3rdparty))
* Android Debug Bridge  (included in [/qtCyberDip/prebuilts](/qtCyberDip/prebuilts))
* OpenCV 2.4.9+ (optional)
	
###Framework 
qtCyberDIP contains 3 parts
* COM		:Serial port and g-code module to communicate with Arduino.
* [BBQScreen](https://github.com/xplodwild/bbqscreen_client) :BBQScreen client module to decode frames from Android devices.
* Capture   :System API module to grab screen or windows, working with AirPlayer to read frames from iOS devices.

###Usage
* Install Qt 5.7 and the Qt VS Add-In
* Install Driver for CH340 Chipset after connected to CyberDIP.
* Install Git for windows
* Git Bash Here: git clone https://github.com/LostXine/qtCyberDIP
* Add '3rdparty/x64' (or '3rdparty/x86', depending on your project platform) into Environment Variable 'Path'
* Open qtCyberDIP.sln in Visual Studio 2013+ and follow the instructions in stdafx.h

###使用方法
* 安装Qt 5.7与相应版本Qt的VS插件
* 连接CyberDIP后，安装CH340 芯片组驱动
* 安装git for windows
* 在目标文件夹中右键选择Git Bash Here,在打开的命令行中输入：git clone https://github.com/LostXine/qtCyberDIP
* 根据编译平台将3rdparty/x64(或3rdprty/x86,取决于你的编译平台)加入系统环境变量Path中
* 使用VS2013及以上版本打开工程文件qtCyberDIP.sln, 并按照stdafx.h中的说明操作

***

###Developer
* Yue ZHOU, A.P. Department of Automation, Shanghai Jiao Tong University.
* Xiang LI, MEng Department of Automation, Shanghai Jiao Tong University. 

###Contact me
* Email:lostxine@gmail.com
* Address:Room 2#302B, SEIEE Building, 800 DongchuanRd., Shanghai, PR China (200240) 


