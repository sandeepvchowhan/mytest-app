
#Steps for setup

First, install Node.js 4
Then, install the latest Cordova and Ionic command-line tools. 
Follow the Android and iOS platform guides to install required platform dependencies.

#Install Ionic
$ npm install -g cordova ionic

#Start a project
$ ionic start myApp tabs

#Run it
$ cd myApp
$ ionic platform add android
$ ionic build android
$ ionic emulate android

Ensure Android SDK is installed and mapped to the Environment variables path.
Add platforms and platform-tools to path

Example: 
C:\Users\svishwanath\AppData\Local\Android\sdk\platforms
C:\Users\svishwanath\AppData\Local\Android\sdk\platform-tools

Verify target variable in "project.properties" is pointing to the version of android SDK installed.

Example:
D:\ionic_project\myApp\platforms\android\CordovaLib\project.properties
D:\ionic_project\myApp\platforms\android\project.properties

Example:
target=android-23

#android list target from command line should show the version of android target installed on your machine.
