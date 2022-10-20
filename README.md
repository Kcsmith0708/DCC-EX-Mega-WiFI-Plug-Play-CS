# DCC-EX-Mega-WiFI-Plug-Play-CS
DCC-EX Mega with WiFi 'Plug & Play' Starter Kit 4.1                                           KCSmith 10-13-22

We Recommend you create a DCC-EX Programs folder and Copy this Starter Kit folder into there
Users/Documents/DCC-EX Programs/ 

A DCC-EX Mega + WiFi Command Station with EXRAIL Courses_Macros 
This Assumes you have a Working Mega WiFi Command Station up and Running
and the Arduino IDE Editor loaded on your PC

Unzip the  DCC-EX Mega Plug & Play Starter Kit 4.1 .zip file

Three Folders are included for this 'Plug & Play' Starter Kit 4.1
 DCC-EX Mega 'Plug & Play' Documents     Includes DCC-EX Mega + WiFi 'Plug & Play'.pdf - Engine Driver screenshots & Fig 1 & 2.
 COMMANDSTATION-EX_Courses_4.1.1         Includes All the DCC-EX files needed to setup & run the Station A to Station B examples
 EXRAIL MP3 Samples                      Includes sample sounds the DFPlayer uses in the scripts.
 ReadMe.txt                              These Instruction

Copy them into your Users/Documents/DCC-EX Programs/ folder
 1) Print the DCC-EX Mega 'Plug & Play'.PDF, Follow the Mega wiring & setup instructions.
 2) Open COMMANDSTATION-EX_Courses.4.1.1 folder, Start the .INO file and Edit the config.h file then compile & upload to the CS
 3) Open the EXRAIL MP3 Examples folder, Copy the files to your Micro SD card 'One' file at a time and insert it into the DFPlayer.

1) DCC-EX Mega 'Plug & Play' Documents
   Open DCC-EX Mega 'Plug & Play' Documents Folder
   Open & Print the DCC_EX Mega + WiFI 'Plug & Play' with Engine Driver Controller.PDF
   Follow the Direction to Install The COMMANDSTATION-EX and the Mega pin out wiring instructions & Engine Driver Preferences Setup.

2) DCC-EX Command Station Program
   DCC-EX Mega + WiFi EXRAIL Plug & Play Command Station is a COMPLETE packaged system 'Ready to Run'
   CommandStation-EX folder includes a Complete Master v4.1 release plus these extra files for the Plug & Play example.
   Includes tabs for;
    config.h				  Sets up WiFi Serial 3, OLED display, DFPlayer on Serial 1 turned On.
    myAutomation.h                 Sets up these first 3 #includes my___.h files and is ready to go.
    myEXRAIL_Courses_100_Macros.h  Sets up EXRAIL Sensor, Servo Turnouts, FX Devices, Layout Setup & WiFi Throttles Cmds & Accessory buttons.
    myEXRAIL_Courses_200_Macros.h  Sets up EXRAIL Automation(n) 201 thru 206 for Loco runs.
    myDCCEX_CommandSummary.h       Sets up DCCEX Command Summary displays with </START 411> Commands by Group in the IDE serial monitor.
    myHal.cpp				  Sets up DFPlayer mini micro-SD card & Ultrasonic Sensor configurations
    mySetup.h				  Sets up Sensors 'S' Turnouts'T' & Outputs'Z' and DFPlayer & Ultrasonic Sensor requirements
                                           And I use it to automatically upload & populate JMRI Tools->Table-> Sensors,Turnouts, Outputs
                                           It also seems to be a good example of how a mySetup could be configured and used without EXRAIL.

Open COMMANDSTATION-EX_Courses 4.1.1 Folder
 Open the COMMANDSTATION-EX folder
 click on COMMANDSTATION-EX.ino and the Arduino IDE editor will open automatically.
In the IDE Editor menu bar 
 Click on Tools >
           Board:> choose Arduino Mega or Mega 2560
           Port: > choose your Com#
 Click on Tools >
           Serial Monitor:> to see the Command Station bootup and EXRAIL script interaction & Print statments.

In the IDE Tabs bar, click on the down arrow tab, scroll down and Open the config.h file

In config.h, Find and Edit these WiFi Network lines and Enter Your SSID 'Name'  & 'Password'
#define WIFI_SSID "Your network name"
#define WIFI_PASSWORD "Your network passwd" 

Then scroll down & find your prefered LCD or OLED display then Uncomment one of theses lines,
// #define LCD_DRIVER  0x27,16,2
// #define OLED_DRIVER 128,32
// #define OLED_DRIVER 128,64

Then on the IDE menu bar press the Compile & Upload => button 
The Mega DCC-EX Command Station should Connect to your Network and be able to Connect a Engine Driver(Android) or WiThrottle(IOS) App device
  that is signed onto the Same WiFi network that the command station is signed on to.

3) DFPlayer mini MP3 Sample sounds
   Open the EXRAIL MP3 Examples folder
	You need to copy the MP3 sound files from here onto your micro-SD card and insert it into the DFPlayer.
	It's Important that you copy and past 'One' file at a time in the 'Order' you want them to play onto the micro-SD card.
	 00         1st sound
	 01         2nd sound
	etc., through sound 14

If you delete one you Will have to delete them all and start all over from 00, or else the DFPlayer will be out of sync.

4) Online DCC-EX Support Services on Discord
   If you need additional help, stop by our Discord Server DCC-EX support and ask for help. https://discord.com/invite/y2sB4Fp 


// License

Copyright 2020 DCC-EX

Licensed under the GNU open source licese.

Unless required by applicable law or agreed to in writing, software distributed
under the License is distributed on an “AS IS” BASIS, WITHOUT WARRANTIES OR
CONDITIONS OF ANY KIND, either express or implied. See the License for the
specific language governing permissions and limitations under the License.

[DCC-EX](https://dcc-ex.com)
