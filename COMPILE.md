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

Mono Framework MDK 6.6.0.166 December 10, 2019

- download from https://www.mono-project.com/download/vs/ and install MonoFramework-MDK-6.6.0.166.macos10.xamarin.universal.pkg

Xamarin Visual Studio 8.5.3.16 April 14, 2020 (= Visual Studio for Mac 8.5 Service Release 3)
- download from https://visualstudio.microsoft.com/vs/mac/ April 14, 2020 - April 21, 2020
- download from https://mac.softpedia.com/get/Developer-Tools/Visual-Studio.shtml April 21, 2020 - April 28, 2020
- open and move to applications

Run Xamarin Visual Studio 8.5.3.16 Visual Studio -> Check for Updates... 
Xamarin Visual Studio 8.5.3.16 uses these dependencies:

.NET Core SDK 3.1.200 March 16, 2020 https://github.com/dotnet/core/blob/master/release-notes/3.1/3.1.2/3.1.200-sdk.md

.NET Core Runtime 2.1.16 February 18th, 2020 https://github.com/dotnet/core/blob/master/release-notes/2.1/2.1.16/2.1.16.md

(Mono Framework MDK 6.8.0.123 Unchecked - Don't install.)

OpenJDK 1.8.0.25 https://docs.microsoft.com/en-us/xamarin/android/get-started/installation/openjdk

(Visual Studio for Mac 8.5.4.12 Unchecked - Don't install.)

Xamarin Profiler 1.6.13 October 17, 2020

Xamarin.Android 10.2.0.100 March 23, 2020 

Xamarin.iOS 13.16.0.13 April 17, 2020

Xamarin.Mac 6.16.0.13 April 17, 2020

Download them and uncheck all Downloaded updates.
These are stored by Visual Studio Update in ~/Library/Caches/VisualStudio/8.0/TempDownload/ and should be backed up.

## Become a Software tester now: Save a restorable image of your harddrive on an external USB drive using CloneZilla Live

You need an external USB drive and a USB pendrive. Install CloneZilla Live on a USB pendrive. Boot your pendrive as UEFI and start CloneZilla Live. Save a restorable image of your harddrive on an external USB drive. 

After a software crash, you can restore this image.

## Project files

Press [Clone or download] in the code section of this repository

Press [Download ZIP]

## Tag commits after you’ve moved past them

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


Open the project file

## Compile

Set the startup project to match your smartphone or tablet

Build and Deploy
