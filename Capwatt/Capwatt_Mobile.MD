# Capwatt Mobile Aplication Documentation!

Before proceeding, make sure you have the following:

 - NodeJS installed from [here](https://nodejs.org/en/download/) (for your os)
 - Terminal or command prompt.
 - Any text editor, I recommend [ATOM](https://atom.io/)

# Steps to run

Install Ionic, this step is required only once if Ionic is not installed.
```sh
npm install -g ionic@latest
```
Install Cordova, this help to packge and make the native app
```sh
npm install -g cordova
```
Change directory in terminal to the project folder
```sh
cd <direcrtory of project>
```
Check if you have npm installed. NPM is a package manager which comes with node.
```sh
npm -v
```
Run the following command to install dependencies required for the project.
```sh
npm i
```
Once all the dependencies are installed, run this command to load project on browser.
```sh
ionic serve -l
```
To add android platform(to make the app for android), run following command once.
```sh
ionic cordova platform add android
```
*When you have finished editing, run following command to make android APK*
It is important to note that Android SDK is required to be installed on the system to build for android.
```sh
ionic cordova build android --prod
```
