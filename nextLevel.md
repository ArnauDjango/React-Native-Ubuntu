For first step install nodejs lts version and do this command

`$ sudo npm install -g expo-cli`

After you need to create blank project 
`$ sudo expo init myBlankProject` and `npm start` for running project

Components:

Create a folder Components in root directory and change the declaration app in App.js: 
``` export default class App extends React.Component { } ```
and creat style in all document will you need with **StyleSheet imported from 'react-native'** and the final code declare 
``` 
  const Style = StyleSheet.create({ 
    main:{
      height: 50
    }
  })
```
