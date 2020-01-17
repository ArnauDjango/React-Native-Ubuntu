# React Native on Linux Ubuntu
How to create app with Linux, React native and node

You need:
- dll node lts version ==> nodejs.org (I prefer use the package manager -> search on other downloads)
- dll android studio and create android device

alter ~/.bashrc for create a path
```
/mnt/c/Users/adck/AppData/Local/Android/Sdk/
export ANDROID_HOME=$HOME/Android/Sdk
export PATH=$PATH:$ANDROID_HOME/emulator
export PATH=$PATH:$ANDROID_HOME/tools
export PATH=$PATH:$ANDROID_HOME/tools/bin
export PATH=$PATH:$ANDROID_HOME/platform-tools
```
and write "source ~/.bachrc" for update 
you can test your paths working with command 'echo $PATH'

now you need a **create react native project** 

example:
```
sudo npm i –g react-native-cli 
mkdir dirproject
cd dirproject
react-native init project 
```
in this directory you can run the app for testing on your phone emulator
```
Adb devices 
Emulator –list-avds 
Emulator –avd nameOfYourVirtualDevice
React-native start 
React-native run-android 
```

create a src directory with your App and your components folder
```
src
    -->App.js
    -->components
        \-->Simples.js
    -->Style
        \-->Default.js
```
Default.js example
```
import { StyleSheet } from 'react-native'

export default StyleSheet.create({
    ex:{
        paddingHorizontal: 15,
        marginVertical: 5,
        borderRadius: 10,
        borderWidth: 2,
        borderColor: '#222',
        fontSize: 24,
        fontWeight: 'bold',
    }
})

```

