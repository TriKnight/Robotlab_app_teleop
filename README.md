# Robotlab_app
This is the Robotlab app Tutorial We design the GUI for the Robot

-----------------------------------------------------
# STEP1. Install the robotlab app

## 1. Teleop app
```
mkdir web_teleop
cd ~/web_teleop
git clone https://github.com/nvnknightdragon/Robotlab_app/
```
This include basic teleop app

## 2. Setup 
Using bower install all package

```
cd ~/web_teleop
bower install
```
you will get all package automatically install:
```
bower polymer#^2.0.0        not-cached https://github.com/Polymer/polymer.git#^2.0.0
bower polymer#^2.0.0           resolve https://github.com/Polymer/polymer.git#^2.0.0
..............

```

## 3. Confifuring and personalizing
 ### 3.1 Folder Structure of the app
 ```
 my-app
├── images
│   ├── favicon.ico
│   └── manifest
│       ├── icon-48x48.png
│       └── ...
├── src
│   ├── store.js
│   ├── actions
│   │   └── ...
│   ├── reducers
│   │   └── ...
│   ├── components
│   │   └── ...
├── test
│   ├── unit
│   │   └── ...
│   └── integration
│       └── ...
├── index.html
├── README.md
├── package.json
├── polymer.json
├── manifest.json
├── service-worker.js
├── sw-precache-config.js
├── wct.conf.json
├── .travis.yml
 ```
 - ```image/``` Image folder store all the icon and picture
 - ```src/ ``` Where all code lives, this folder include 4 areas:
    - ```components/``` is the directory that contains all the custom elements in the application.
    - ``` action/```, ```reducers/``` and ```store.js``` are Redux specific files and folders. Check out the **Redux and state management** page for details on that setup.
 - ```test/ ``` is the directory with all of your tests. it’s split in unit tests (that are run across different browsers), and integration tests, that just run on headless Chrome to ensure that the end-to-end application runs and is accessible. Check out the application testing page for more information.
 - ```index.html``` is your application’s starting point. It’s where you load your polyfills and the main entry point element.
 - ```package.json```  the npm configuration file, where you specify your dependencies. Make sure you run npm install any time you make any changes to this file.
 - ```polymer.json``` the polymer cli configuration file, that specifies how your project should be bundled, what’s included in the service worker, etc. (docs).
 - ```manifest.json``` is the PWA metadata file. It contains the name, theme color and logos for your app, that are used whenever a user adds your application to the homescreen.
 - ``` service-worker.js```  is a placeholder file for your Service Worker. In each build directory, the polymer cli will populate this file with actual contents, but during development it is disabled.
 - ```sw-precache-config.js ```  is a configuration file that sets up the precaching behaviour of the Service Worker (such as which files to be precached, the navigation fallback, etc.).
 - ```wct.conf.json ```is the web-component-tester configuration file, that specifies the folder to run tests from, etc.
 - ```.travis.yml``` sets up the integration testing we run on every commit on Travis.
