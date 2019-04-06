Things are changing very fast. This is the situation as at 2019-04-05.  
# mem1_electron
Learning how to create desktop electron app from Rust Wasm/Webassembly Virtual Dom Dodrio memory game.  
Electron is Cross Platform - compatible with Mac, Windows, and Linux.  

The source code of the original app is here:  
https://github.com/LucianoBestia/mem1  
Learning to use Dodrio virtual DOM on a simple memory game for kids.  
The images are funny cartoon characters from the alphabet.  
The cards grid is only 4x4.  

![snap01](https://user-images.githubusercontent.com/31509965/55587238-181e8200-5755-11e9-88eb-f8fb62be581e.png)

# How to install Electron on Windows
1. install Nodejs 11 - the latest version. It will also install npm - the packet manager.   
It didn't work correctly for me with Nodejs version 10. I don't know why.    
https://nodejs.org/en/  

2. Install electron  
```
npm i -D electron@latest
```

# Clone and run mem1_electron example code
3. Clone mem1_electron code example. It will create a new folder.  
```
git clone https://github.com/LucianoBestia/mem1_electron
```
4. move to the new folder
```
cd mem1_electron
```
5. Install all needed referenced libraries  
```
npm install
```
6. build and start the new electron application  
```
npm start
```
# Create a package for distribution
7. install electron-packager
```
npm install electron-packager -g
```
8. create a folder with all files for distribution.
You can then zip it and publish it. 
```
electron-packager .
```

I published the zip file in GitHub Release:  
https://github.com/LucianoBestia/mem1_electron/releases/tag/ver1  
Download it, unzip it and execute the file mem1_electron.exe.  


I hope it will work for you as it did for me.
# Programming references
https://electronjs.org/  
https://nodejs.org/en/  
https://github.com/electron-userland/electron-packager  


