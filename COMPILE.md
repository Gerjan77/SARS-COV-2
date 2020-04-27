# Compile

The principle of compilability reaches further than 'open source'. Any software tester is able to compile the open source software just as efficient as the developer(s).
As a matter of principle, all third-party software meets the following:
No software created after April 26th 2020 Sunday 12:45h UTC will be used, except this repository.
Dependencies will be exactly defined by version and downloadable or included in this repository.
The compiling platform is fully defined by the dependency version list.

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
Xamarin Visual Studio 8.5.3.16 April 14, 2020
.NET Core SDK 3.1.200 March 16, 2020
.NET Core Runtime 2.1.16 February 18th, 2020 
OpenJDK 1.8.0.25
Xamarin Profiler 1.6.13 October 17, 2020
Xamarin.Android 10.2.0.100 March 23, 2020
Xamarin.iOS 13.16.0.13 April 17, 2020
Xamarin.Mac 6.16.0.13 April 17, 2020

https://github.com/Gerjan77/SARS-COV-2/releases/download/v0.0/MonoFramework-MDK-6.6.0.166.macos10.xamarin.universal.pkg download and install
https://github.com/Gerjan77/SARS-COV-2/releases/download/v0.0/visualstudioformac-8.5.3.16.dmg
open and move to applications
https://github.com/Gerjan77/SARS-COV-2/releases/download/v0.0/dotnet-sdk-3.1.200-osx-x64.pkg
download and install
https://github.com/Gerjan77/SARS-COV-2/releases/download/v0.0/dotnet-runtime-2.1.16-osx-x64.pkg
download and install
https://github.com/Gerjan77/SARS-COV-2/releases/download/v0.0/microsoft_dist_openjdk_1.8.0.25.zip
download and install
https://github.com/Gerjan77/SARS-COV-2/releases/download/v0.0/profiler-mac-1.6.13-11.pkg
download and install
https://github.com/Gerjan77/SARS-COV-2/releases/download/v0.0/xamarin.android-10.2.0.100.pkg
download and install
https://github.com/Gerjan77/SARS-COV-2/releases/download/v0.0/xamarin.ios-13.16.0.13.pkg
download and install
https://github.com/Gerjan77/SARS-COV-2/releases/download/v0.0/xamarin.mac-6.16.0.13.pkg
download and install

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




### Scripts used


Tag commits after you’ve moved past them

```zsh
# download all
git clone https://github.com/Gerjan77/SARS-COV-2 ~/SARS-COV-2
cd SARS-COV-2
# tag initial commit
git tag -a v0.0 -m "Initial Commit." 980bc6e
# show commits
git log --pretty=oneline
# upload tag
git push origin v0.0
```

Find a file called xamarin.android-10.2.0.100.pkg

```zsh
# list all files in file-list.txt
sudo find / &> ~/file-list.txt
# file attributes
sudo chown $(whoami) ~/file-list.txt
# search for a substring
cat ~/file-list.txt | grep -E "(10.2.0.100)"
```
