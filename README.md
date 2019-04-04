# mem1_electron
Creating a desktop electron app from Rust Webassembly Virtual Dom memory game.
Things are changing very fast. This is the situation as in 2019-04-05.
Learning to use Dodrio virtual DOM on a simple memory game for kids.  
The images are funny cartoon characters from the alphabet.  
The cards grid is only 4x4.  

The source code of the original app is here:  
[https://github.com/LucianoBestia/mem1](https://github.com/LucianoBestia/mem1)

#How to install Electron on Windows
1. install nodejs 11 the latest version. It will install also npm.   
It didn't work for me with the version 10.    
[https://nodejs.org/en/](https://nodejs.org/en/)  

2. Install electron

```
npm i -D electron@latest
```
3. Clone the simplest example. It will create a new folder.
```
git clone https://github.com/electron/electron-quick-start
```
4. move to the new folder
```
cd electron-quick-start
```

5. Install all needed referenced libraries
```
npm install
```
6. build and start the new electron application
```
npm start
```
