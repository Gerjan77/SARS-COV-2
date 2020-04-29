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

Set the startup project to match your smartphone or tablet

Build and Deploy
