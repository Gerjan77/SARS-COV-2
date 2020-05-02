# Timestamp

Sunday April 26th 2020 12:45h UTC Worldwide Confirmed Infections 2,9M Recovered 823K Deaths 203K

# Compile

The principle of compilability reaches further than 'open source'. Any software tester is able to compile the open source software just as efficient as the developer(s).
As a matter of principle, all third-party software meets the following:
No software created after April 26th 2020 Sunday 12:45h UTC will be used, except this repository.
Dependencies will be exactly defined by version and downloadable or included in this repository.
The *compiling platform* is fully defined by the dependency version list.

## Upgrade or downgrade to the following software versions

MacOS 10.15.4 Supplemental Update 19E287 April 8, 2020 (clean install)

Xcode 11.4.1 11E503a April 15, 2020
  - go to https://developer.apple.com/download/more/ and login as developer
  - download Xcode_11.4.1.xip, move to applications and install

Command Line Tools for Xcode 11.4.1 April 15, 2020

- go to https://developer.apple.com/download/more/ and login as developer
- download Command_Line_Tools_for_Xcode_11.4.1.dmg, open and install
- Versioncheck in the Terminal
```zsh
if pkgutil --pkgs=com.apple.pkg.CLTools_Executables >/dev/null; then
    echo CommandLineTools: $(pkgutil --pkg-info=com.apple.pkg.CLTools_Executables | awk '/version:/ {print $2}')
else
    echo CommandLineTools: not installed
fi
```

## install dependencies

Mono Framework MDK 6.6.0.166 December 10, 2019

https://github.com/Gerjan77/SARS-COV-2/releases/download/v0.0/MonoFramework-MDK-6.6.0.166.macos10.xamarin.universal.pkg 

download and install

Xamarin Visual Studio 8.5.3.16 April 14, 2020

https://github.com/Gerjan77/SARS-COV-2/releases/download/v0.0/visualstudioformac-8.5.3.16.dmg

open and move to applications

.NET Core SDK 3.1.200 March 16, 2020

https://github.com/Gerjan77/SARS-COV-2/releases/download/v0.0/dotnet-sdk-3.1.200-osx-x64.pkg

download and install

.NET Core Runtime 2.1.16 February 18th, 2020 

https://github.com/Gerjan77/SARS-COV-2/releases/download/v0.0/dotnet-runtime-2.1.16-osx-x64.pkg

download and install

OpenJDK 1.8.0.25

https://github.com/Gerjan77/SARS-COV-2/releases/download/v0.0/microsoft_dist_openjdk_1.8.0.25.zip

extract and copy to ~/Library/Developer/Xamarin/jdk/microsoft_dist_openjdk_1.8.0.25
```zsh
mkdir ~/Library/Developer/Xamarin/jdk
mkdir ~/Library/Developer/Xamarin/jdk/microsoft_dist_openjdk_1.8.0.25
sudo cp -R ~/Downloads/microsoft_dist_openjdk_1.8.0.25 ~/Library/Developer/Xamarin/jdk/
ls ~/Library/Developer/Xamarin/jdk/microsoft_dist_openjdk_1.8.0.25
```

Point the IDE to the new JDK:
Click Tools > SDK Manager > Locations and change the Java SDK (JDK) Location to the full path of the OpenJDK installation. In the following example, this path is set to ~/Library/Developer/Xamarin/jdk/microsoft_dist_openjdk_1.8.0.25
https://docs.microsoft.com/en-us/xamarin/android/get-started/installation/openjdk-images/vsm.png

Xamarin Profiler 1.6.13 October 17, 2020

https://github.com/Gerjan77/SARS-COV-2/releases/download/v0.0/profiler-mac-1.6.13-11.pkg

download and install

Xamarin.Android 10.2.0.100 March 23, 2020

https://github.com/Gerjan77/SARS-COV-2/releases/download/v0.0/xamarin.android-10.2.0.100.pkg

download and install

Xamarin.iOS 13.16.0.13 April 17, 2020

https://github.com/Gerjan77/SARS-COV-2/releases/download/v0.0/xamarin.ios-13.16.0.13.pkg

download and install

Xamarin.Mac 6.16.0.13 April 17, 2020

https://github.com/Gerjan77/SARS-COV-2/releases/download/v0.0/xamarin.mac-6.16.0.13.pkg

download and install

Open Visual Studio, go to Tools -> SDK Manager

Select Platforms:

    Android 9.0 - Pie     API 28 >
        Android SDK Platform 28                Version 6  72 MB
    Android 8.0 - Oreo    API 26 >
        Android SDK Platform 26                Version 2  60 MB
    Android 7.1 - Nougat  API 25 >
        Android SDK Platform 25                Version 3  81 MB
    Android 7.0 - Nougat  API 24 >
        Android SDK Platform 25                Version 2  78 MB
    Android 5.0 - Nougat  API 21 >
        Android SDK Platform 21                Version 2  62 MB
        
Choose Emulators 
    
    Android 7.1 - Nougat  API 25 >
        Google APIs Intel x86 Atom_64 System Image        1 GB
        Google APIs ARM EABI v7a System Image             879 MB
Select Tools:

    Android SDK Tools >
        Android SDK Tools 26.1.1                          98 MB
        Android SDK Tools 25.2.5                          191 MB

    Android SDK Platform-Tools 29.0.5                     7 MB     

    Android SDK Build Tools >
        Android SDK Build-Tools 29.0.2                    38 MB
        Android SDK Build-Tools 25.0.3                    48 MB

    Android Emulator 29.3.0                               317 MB
    SDK Patch Applier v4                                  1 MB
    
The Empty projectfile (SARS-COV-2 v0.0.2.0 Empty Project) is created in Visual Studio, File -> New Solution.
The 'New Project' window lefthand pane: Multiplatform -> App. The 'New Project' window righthand pane: Xamarin.Forms -> Shell Forms App, select C#. [Next]. App name: sarscov2 Organisation: com.goodjobunit [Next] [Next] Now change App in Xamarin.Forms.Application.

Nuget Packages used in the projectfile:

    Xamarin.Essentials 1.3.1
    Xamarin.Forms 4.4.0.991265

## Become a Software tester now: Save a restorable image of your harddrive on an external USB drive using CloneZilla Live

You need an external USB drive and a USB pendrive. Install CloneZilla Live on a USB pendrive. Boot your pendrive as UEFI and start CloneZilla Live. Save a restorable image of your harddrive on an external USB drive. 

After a software crash, you can restore this image.

## Project files

Press [Clone or download] in the code section of this repository

Press [Download ZIP]

Open the project file

## Compile

Set the startup project to match your smartphone or tablet. You can connect your iPhone 3GS, iPhone 4, iPhone 4s, iPhone 5, iPhone 5c, select "Build Configuration ARMv7|iPhone5c" and press the [arrow forward] button.

Build and Deploy

# Licensing iOS App

## Free provisioning for Xamarin.iOS apps

Free provisioning allows Xamarin.iOS developers to deploy and test their apps on iOS devices without being part of the Apple Developer Program. While simulator testing is valuable and convenient, it is also essential to test apps on physical iOS devices to verify that they function properly under real-world memory, storage, and network connectivity constraints.

To use free provisioning to deploy an app to a device:

    Use Xcode to create the necessary signing identity (developer certificate and private key) and provisioning profile (containing an explicit App ID and the UDID of a connected iOS device).
    Use the signing identity and provisioning profile created by Xcode in Visual Studio for Mac or Visual Studio 2019 to deploy your Xamarin.iOS application.

### Important

Automatic provisioning allows Visual Studio for Mac or Visual Studio 2019 to automatically set up a device for developer testing. However, automatic provisioning is not compatible with free provisioning. In order to use automatic provisioning, you must have a paid Apple Developer Program account.

## Requirements

To deploy your Xamarin.iOS applications to a device with free provisioning:

    The Apple ID being used must not be connected to the Apple Developer Program.
    Your Xamarin.iOS app must use an explicit App ID, not a wildcard App ID.
    The bundle identifier used in your Xamarin.iOS app must be unique and cannot have been used in another app previously. Any bundle identifier used with free provisioning cannot be re-used.
    If you have already distributed an app, you cannot deploy that app with free provisioning.
    If your app uses App Services, you will need to create a provisioning profile as detailed in the device provisioning guide.

Take a look at the Limitations section of this document for more information about limitations associated with free provisioning, and refer to the App distribution guides for more information about distributing iOS applications.

## Testing on device with free provisioning

Follow these steps below to test your Xamarin.iOS app with free provisioning.
Use Xcode to create a signing identity and provisioning profile

    If you do not have an Apple ID, create one.

    Open Xcode and navigate to Xcode > Preferences.

    Under Accounts, use the + button to add your existing Apple ID. It should look similar to the screenshot below:

    Xcode Preferences – Accounts

    Close Xcode preferences.

    Plug in the iOS device to which you'd like to deploy your app.

    In Xcode, create a new project. Choose File > New > Project and select Single View App.

    In the new project dialog, set Team to the Apple ID that you just added. In the drop-down list, it should look similar to Your Name (Personal Team):

### Create a new app

    Once the new project has been created, choose an Xcode build scheme that targets your iOS device (rather than a simulator).

    Select an Xcode build scheme

    Open your app's project settings by selecting its top-level node in Xcode's Project Navigator.

    Under General > Identity, make sure that the Bundle Identifier exactly matches your Xamarin.iOS app's bundle identifier.

    Set a bundle identifier

### Important

    Xcode will only create a provisioning profile for an explicit App ID, and it must be identical to the App ID of your Xamarin.iOS app. If they differ, you will not be able to use free provisioning to deploy your Xamarin.iOS app.

    Under Deployment Info, ensure that the deployment target matches or is lower than the version of iOS installed on your connected iOS device.

    Under Signing, select Automatically manage signing and select your team from the drop-down list:

    Automatically manage signing

    Xcode will automatically generate a provisioning profile and signing identity for you. You can view this by clicking on the information icon next to provisioning profile:

    View the provisioning profile

### Tip

    If there is a failure when Xcode attempts to generate a provisioning profile, make sure that Xcode's currently-selected build scheme targets the connected iOS device rather than a simulator.

    To test in Xcode, deploy the blank application to your device by clicking the run button.

Deploy your Xamarin.iOS app

    Visual Studio for Mac
    Visual Studio

    Connect your iOS device to the Mac build host via USB or wirelessly.

    In the Visual Studio for Mac Solution Pad, double-click on Info.plist.

    In Signing, select Manual Provisioning.

    Click the iOS Bundle Signing… button.

    For Configuration, select Debug.

    For Platform, select iPhone.

    Select the Signing Identity created by Xcode.

    Select the Provisioning Profile created by Xcode.

    Set the signing identity and provisioning profile

    Tip

    If you cannot see your signing identity or the correct provisioning profile, you may need to restart Visual Studio for Mac.

    Click OK to save and close the Project Options.

    Select your iOS device and run the app.

## Limitations

Apple has imposed a number of limitations on when and how you can use free provisioning to run your application on an iOS device, ensuring that you can only deploy to your device:

    Access to iTunes Connect is limited and therefore services such as publishing to the App Store and TestFlight are unavailable to developers provisioning their applications freely. An Apple Developer Account (Enterprise or Personal) is required to distribute via Ad Hoc and In-House means.
    Provisioning profiles created with free provisioning will expire after one week, and signing identities will expire after one year.
    Since Xcode will only create provisioning profiles for explicit App IDs, you will need to follow the instructions above for every app that you wish to install.
    Provisioning for most application services is not possible with free provisioning. This includes Apple Pay, Game Center, iCloud, In-App Purchasing, Push Notifications, and Wallet. Apple provides a full list of capabilities in the Supported capabilities (iOS) guide. To provision your app for use with application services, visit the Working with capabilities guides.

## Summary

This guide explored the advantages and limitations of using free provisioning to install applications on an iOS device. It provided a step-by-step walkthrough that demonstrated how to use free provisioning to install a Xamarin.iOS app.
