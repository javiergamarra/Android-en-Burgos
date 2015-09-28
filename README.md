
bile Workshop - Building native mobile apps with Liferay

Description in how to set up the **Android environment** for the Mobile Workshop, *Building native mobile apps with Liferay*.

## Requirements

  * PC (Windows 2003 or later), MAC OS 10.8.5 or most of the Linux distros.
  * Java programming experience
  * Having an Android phone is optional. Genymotion or Android emulator are good replacements.

## How to install and configure the environment

We will use the following software:

  * Java JDK 7
  * Android Studio
  * Android SDK
  * Genymotion (optional)
  
### Windows

We will install the following applications:

* [JDK](http://www.oracle.com/technetwork/java/javase/downloads/jdk7-downloads-1880260.html)
* [Android Studio](https://developer.android.com/sdk/index.html)
* Android SDK (usually embedded with Android Studio or available [here](http://dl.google.com/android/installer_r24.3.4-windows.exe))
* [Genymotion](https://www.genymotion.com) (optional, you can use the default Android emulator).

The installation process (for Windows) is briefly detailed here, you can read a more detailed instructions in the official [Android page](https://developer.android.com/sdk/installing/index.html?pkg=studio).
  
1. Install the JDK 7 with the provided file or download it with this [link](http://www.oracle.com/technetwork/java/javase/downloads/jdk7-downloads-1880260.html).

	You will have to set the `JAVA_HOME` environment variable (to the folder you have installed the JDK, usually `C:\Program Files\Java\jdk1.7.0_79\` and the `PATH` variable pointing to the `bin` folder of the JDK, usually `C:\Program Files\Java\jdk1.7.0_79\bin\`.
2. Install the provided Android Studio + SDK tools bundle or download it with this [link](https://developer.android.com/sdk/index.html).

	* The installer will ask to install a JDK it isn't installed or can't find it.
	* Make sure that you install both the Android Studio and the Android SDK.
	* Android Virtual Device y Intel HAXM are recommended but not required.
	* You will need at least 3GB of free space.
	* We recommend using short folder names without spaces.

3. After the installation, when Android Studio starts, the Android SDK will download the latest SDK version (23). You can download more versions from the *configure*, *SDK Manager*. 
	* We recommend downloading the `SDK Platform` and `Google APIs` for **Android 4.1.2 (API 16)**.
4. To run your application you have several options:
	* Launch it in your mobile phone. To be able to do so you need to enable the development mode in your phone (usually by tapping the build number several times) and install the debug drivers of your phone (provided by the manufacturer or using the default drivers).
	* Launch in the Android Emulator with an x86 image (faster than an ARM one). You will need Intel HAXM and won't work in old computers, virtual machines/parallels or computers with VT-x disabled in the BIOS. Intel HAXM can be downloaded from the `SDK Manager` (menu, *tools*, *Android*, *SDK Manager*, *Launch Standalone SDK Manager*, *Extras*, select *Intel x86 Emulator Accelerator*) and opening the installer from the default download folder (usually in `C:\Users\_YOUR_USERNAME\AppData\Local\Android\sdk\extras`).
	* Download an ARM image and create an emulator with that image. You can download an ARM image from the `SDK Manager` (menu, *tools*, *Android*, *SDK Manager*, *Launch Standalone SDK Manager*, *Extras*, select *Intel x86 Emulator Accelerator*) and use the `AVD Manager` (menu, *tools*, *Android*, *AVD Manager*) to create a new emulator using that image.
	* Or use Genymotion. You will have to register in their [website](http://genymotion.com) to be able to use it. And make sure that you install the version with Virtualbox (or install it separately). Once installed, download a Nexus 5 image with Lollipop. The Android Studio plugin is not needed.
5. **To test that everything works**, you can create a new Android Application from the menu, `Start a new Android Studio project`, select *API 16*, *Blank Activity* and launch it with your mobile phone or the Android emulator (from the menu, *Run*, *Run 'app'*).
  
### MAC

We will install the following applications:

* [JDK](http://www.oracle.com/technetwork/java/javase/downloads/jdk7-downloads-1880260.html)
* [Android Studio](https://developer.android.com/sdk/index.html)
* Android SDK (usually embedded with Android Studio or available [here](http://dl.google.com/android/android-sdk_r24.3.4-macosx.zip))
* [Genymotion](https://www.genymotion.com) (optional, you can use the default Android emulator).

The installation process (for MAC computers) is briefly detailed here, you can read a more detailed instructions in the official [Android page](https://developer.android.com/sdk/installing/index.html?pkg=studio).
  
1. Install the JDK 7 with the provided file or download it with this [link](http://download.oracle.com/otn-pub/java/jdk/7u79-b15/jdk-7u79-macosx-x64.dmg).  

2. Install the provided Android Studio + SDK tools bundle or download it with this [link](https://dl.google.com/dl/android/studio/install/1.3.2.0/android-studio-ide-141.2178183-mac.dmg).

	* Make sure that you install both the Android Studio and the Android SDK.
	* Android Virtual Device y Intel HAXM are recommended but not required if you are going to use genymotion.
	* You will need at least 3GB of free space.

3. After the installation, when Android Studio starts, the Android SDK will download the latest SDK version (23). You can download more versions from the *configure*, *SDK Manager*. 
	* We recommend downloading the `SDK Platform` and `Google APIs` for **Android 4.1.2 (API 16)**.

4. To run your application you have several options:
	* Launch it in your mobile phone. To be able to do so you need to enable the development mode in your phone (usually by tapping the build number several times) and install the debug drivers of your phone (provided by the manufacturer or using the default drivers).
	* Launch in the Android Emulator with an x86 image (faster than an ARM one). You will need Intel HAXM and won't work in old computers, virtual machines/parallels or computers with VT-x disabled in the BIOS. Intel HAXM can be downloaded from the `SDK Manager` (menu, *tools*, *Android*, *SDK Manager*, *Launch Standalone SDK Manager*, *Extras*, select *Intel x86 Emulator Accelerator*) and opening the installer from the default download folder (usually in `C:\Users\_YOUR_USERNAME\AppData\Local\Android\sdk\extras`).
	* Download an ARM image and create an emulator with that image. You can download an ARM image from the `SDK Manager` (menu, *tools*, *Android*, *SDK Manager*, *Launch Standalone SDK Manager*, *Extras*, select *Intel x86 Emulator Accelerator*) and use the `AVD Manager` (menu, *tools*, *Android*, *AVD Manager*) to create a new emulator using that image.
	
5. **To test that everything works**, you can create a new Android Application from the menu, `Start a new Android Studio project`, select *API 16*, *Blank Activity* and launch it with your mobile phone or the Android emultator (from the menu, *Run*, *Run 'app'*).
5. We recommend installing Genymotion because is faster than the official Android emulator. You will have to register in their [website](http://genymotion.com) to be able to use it.

	* Make sure that you install the version with Virtualbox (or install it separately). Once installed, download a Nexus 5 image with Lollipop. The Android Studio plugin is not needed.

### Linux

* Please refer to this [guide](https://developer.android.com/sdk/installing/index.html?pkg=studio)

## Common problems

* `emulator: ERROR: x86 emulation currently requires hardware acceleration!` or `Please ensure Intel HAXM is properly installed and usable.`

	Intel acceleration is not working, either because your computer does not have virtualization capabilities (older computers that have >4 years), VT-x is disabled in the BIOS or you are trying to run the emulator inside a virtual machine. We recommend using an ARM image to create a new emulator.

* `INSTALL_FAILED_OLDER_SDK`:

	Your application is targeting a newer SDK version that you have installed in your phone. Tipically a new Android project compiles against a Lollipop or later (21-23)
	
	You can change it in the build.gradle file, under `compileSdkVersion`. A safe number could be 16 (Android 4.1). You would have to download the Android SDK for that version.

* Does the SDK runs in a virtual machine?

	Yes, it is possible to set up the environment in a virtual machine. But it is quite possible that you found the following problems:
	
	* Accessing to your mobile phone is tricky and depends on the port/IP configuration between the virtual machine and the computer.
	* Genymotion usually won't work due to the limited capabilities of the emulated graphic card.
	* HAXM won't work without a lot of configuration, due to the limitations of accelerating a virtual machine (Android emulator) inside another virtual machine.
	
	We recommend using the default Android emulator with an ARM image (x86 usually won't work).
