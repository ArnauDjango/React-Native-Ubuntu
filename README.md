# React-Native
How to create app with Linux, React native, node

You need:
- dll node lts version ==> nodejs.org
- dll android studio and create android device

alter ~/.bashrc for create a path
```
export ANDROID_HOME=$HOME/Android/Sdk
export PATH=$PATH:$ANDROID_HOME/emulator
export PATH=$PATH:$ANDROID_HOME/tools
export PATH=$PATH:$ANDROID_HOME/tools/bin
export PATH=$PATH:$ANDROID_HOME/platform-tools
```
and write "source ~/.bachrc" for update this
you can test so you path work with this command 'echo $PATH'

now you need a **create react project** 

example:
```
sudo npm i –g react-native-cli 
mkdir dirproject
cd dirproject
react-native init project 
```
in this directory you can run the app for testin on your phone emulator
```
Adb devices 
Emulator –list-avds 
Emulator –avd blablabla 
React-native start 
React-native run-android 
```
