# AndroSpy - Xamarin-C# Android RAT  
<img src="https://user-images.githubusercontent.com/45147475/89324496-096d1580-d690-11ea-86d2-1b8b1d484d35.png" width="25%"></img>   

An Android RAT that written in completely C# by me (qH0sT a.k.a Sagopa K)  

Yes, It is supporting dns connection like no-ip or duckdns or dynu......  

I'm very busy; I can't answer immediately for your issue.  

Connection may will not coming if device is in sleep(doze) mode in currently update but I will fix this.  

+How can I build a Client?  
- https://www.youtube.com/watch?v=3LEegvEp8_E  (thanks to AndroTricks for this video)  

Don't worry, there is no complicated ``Socket`` programming; all thing is simple to understand.  

-A major Socket bug that is only but only because of single word will be released as fixed in the next update.

-You must also UDP port open; select item in comboBox on NAT page of Modem: TCP and UDP (both) , otherwise you can't hear live microphone.  

-Delete all files and folders in the path on SV project (SV\bin\Debug\resources\ProjectFolder\) and re-copy the Client files into the this path.  

For Keylogger your victim must toggle on Accessibility button of your trojan in Settings of Device  

<img src="https://user-images.githubusercontent.com/45147475/101618575-3e64ec80-3a23-11eb-8462-8d36606878d3.jpg" width="25%"></img> 

Minumum Android Version: 4.1    

Tested on some systems:  
Android 4.4.2 - OK  
Android 5.1.1 - OK  
Android 7.1.2 - OK  
Android 6.0.1 - OK  
Android 9.0   - OK  
Android 10    - OK  

AndroSpy Project aims to most powerful-stable-useful open source Android RAT.  

Working with all network types: 2G, 3G, 4G, 4.5G, WI-FI.....; not only working in the local network, but in the WAN.  

Frequently check for update on github repo of AndroSpy for the best user experience.  

For Huawei and other EMUI devices, read this article: https://dontkillmyapp.com/huawei I added the code suggestion for developers to our Client; wakelock tag: "LocationManagerService"  

<img src="https://user-images.githubusercontent.com/45147475/105629498-66ce6c00-5e54-11eb-9ac1-f1930f8007b2.png" width="45%"></img> <img src="https://user-images.githubusercontent.com/45147475/105629500-6930c600-5e54-11eb-932d-392db6be4859.PNG" width="45%"></img> <img src="https://user-images.githubusercontent.com/45147475/105629501-6c2bb680-5e54-11eb-80fe-4051dcae51f6.PNG" width="45%"></img> <img src="https://user-images.githubusercontent.com/45147475/105629503-6c2bb680-5e54-11eb-938d-0a49f8814e5e.PNG" width="45%"></img>  

# Update 2021 Jan. 24  

+ Socket communication has been completely re-coded; quality camera view, fast and light communication. Communicate entirely with byte[] arrays; It got rid of Base64, Fast and light communication.
+ The graphical user interface has been renewed.
+ File download and sending codes, photo capture codes were re-coded by creating a buffer zone.
+ "Night mode" has been added to the live camera form and live screen form.
+ Close, Reconnect and Remove options have been added for the client.
and other improvements-fixes ..  

# Update December 2020 on Version 3  

+CPU Wakelock is now choose of user in Builder.  
+Added "Password" properties for connection security between you and your client.  
+WakeLock power usage optimized; our client uses as little battery as possible.  
+Added "Detailed Infos" tab in the Status of Phone Window, you can see; detailed IMEI, SIM Infos and more..  
+High CPU usage problem fixed that has caused when device didn't have Internet.  
+Focus Mode on Live Camera is now choose of User.  
+Added Live Screen (MediaProjection API has been available since API Level 21, for more: https://developer.android.com/reference/android/media/projection/MediaProjection  
+File Manager has been improvement.  
+Fully English version.  
+Now it is supporting 5 digits Port.  
+Fixed English Flag issue.  
+If device does not have any camera, you will see warning message.  
+Added victim name and ip adress as title of control windows. Ex: Keylogger - Victim@192.168.2.78:7675  
and other changes, fixing, improvents. :)

# Version 3  
+Added live Camera stream (with resolution,zoom,flash,quality controls and scene,focus,white balance mode)  
+Fixed loss data transfer  
+Some excess codes have been removed  
+Performance has been increased

# [+] Update on version V2  
+Added logs.  
+Added preview of clicked image into the filemaneger.  
+Added choose sizes of both front and back camera.  
+Some other fixes and changes.

# [+]Version Update 2 (first update as version)  
+Switching to ``System.Net.Sockets.NetworkStream`` from directly ``System.Net.Sockets.Socket`` Communitation. This change was more stable and fast. And Project has cleaner code.  
+Added Wifi,Bluetooth,Mobil Data etc. into  the Phone Infos form.  
+Added screen brightness option into the settings panel.  
+Some important updates-changes.

# [+]Update 1.3 (First stable Update)  
+Added "Add Shortcut to home screen" option into the Fun Manager.  
+Added Name of Phone Number into the Window that is showed when Incall or Outgoing Call starts in any Victim.  
+a Correction in SMS Manager.
  
# [+]Update 1.2 ( semi-stable Update :) )  
+Connection between Client and Server has been improvement.  
+Added 'Name' column into the Sms and Call Log manager.  
+Some visual changes.  
+Added dropped Pin URL into the Location Manager  
+Fixed terminate problem that caused by Ram Cleaner.  
+Fixed problem that caused when our trojan hides self from launcher.  
+Our trojan can hide it self from launcher.

# [+]Update 1.1  
+Major improvements  
+Added Flash/Torch option to Camera Manager and percentage status with progressbar.  
+Reconstructed Upload/Download file and added percentage status with progressbar.  
+Added Download Manager (you can download any file that you want into the victim's phone but you must put filename into textBox)  
+Added some features into Call Manager (Send sms to selected phone number directly, call selected number...)
+Added source into Microphone Manager (Mic, Call, Default)  
+Some visual improvements.
And more that I have forgot to write :)

# [+]Update 1.0  
+Critical improvements (in both Server and Client)  
+Re-made File Manager (more sightly, stable and useful)

# [+]Update 0.1.2  
+some improvements (in both Server and Client)  
+Notify when Call (incoming or outgoing) in any client starts.  
+Camera was improvement.
  
# User Manual
For Users:
For builder you must install msbuild tools latest version, JDK latest version and Android SDK Tools. Then open the file (in the \Debug\ path) that has .tht extension with Notepad and configure the paths in the this .tht file again to your side. And copy the files in the "Client" folder into the \ProjectFolder\ path in the Server side.

MsBuild Tools: https://download.visualstudio.microsoft.com/download/pr/c10c95d2-4fba-4858-a1aa-c3b4951c244b/54dedc13fbb321033e5d3297ac7c5ad8de484be2871153fe20599211135c9448/vs_BuildTools.exe  

(Check Xamarin checkBox in the installation panel)

For Developers:  
Your Visual Studio must have Xamarin Developing Kit then you can develop the Android side project (Client)
