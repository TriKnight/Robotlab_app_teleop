# Robotlab_app
This is the Robotlab app Tutorial We design the GUI for the Robot

-----------------------------------------------------
# STEP1. Learning the Polymer with PWA Starter Kit

## 1. Tutorial Polymer with PWA Starter kit
https://pwa-starter-kit.polymer-project.org/overview



This template is very similar to the master template, in the sense that it keeps both Redux for state management, and all of the UI elements. The main difference is that the wide screen layout displays a persistent app-drawer, inline with the content.

## 2. Setup 
This page will take you through the steps you need to do to build and run the sample app locally.

```
git clone --depth 1 https://github.com/Polymer/pwa-starter-kit my-app
cd my-app
```
or we can use the template-responsive-drawer-layout [code](https://github.com/Polymer/pwa-starter-kit/tree/template-responsive-drawer-layout), [demo](https://template-responsive-drawer-layout-dot-pwa-starter-kit.appspot.com/)
```
git clone -b template-responsive-drawer-layout https://github.com/Polymer/pwa-starter-kit.git
cd pwa-starter-kit
```

This will create the inital project **my-app** folder

```
my-app
├── images
│   └── ...
├── src
│   └── ...
├── test
│   └── ...
├── index.html
├── README.md
├── package.json
├── polymer.json
├── manifest.json
├── service-worker.js
├── sw-precache-config.js
├── ... (misc project config files)
```
Intall the dependencies
```
cd my-app
npm install
```
Run the app in the deveopment mode
```
npm start
```
This will start a local server on port 8081. Open [http://localhost:8081](http://localhost:8081) to view your app in the browser. Note that this server can continue running as you’re making changes to your application, which you will see if you refresh the browser tab.

If the port is already taken on your computer, or if you need to change the default hostname (because you’re using a Docker container, for example), you can configure them using command line arguments:
```
npm start -- --hostname 0.0.0.0 --port 4444
```
Run the tests

Check out the Application testing page for more information about the tests. For a quick way to run the tests, run
```
npm run test
```
Available scripts

In the app’s root directory you can run:

- ```npm start``` to run the application in development mode.
- ```npm run test```  to run the application’s unit and integration tests (see the see the Application testing section for more details. To run just the unit or integration tests, both npm run test:unit and npm run test:integration are available.
- ```npm run build``` to build your application for production (see the Building and deploying section for more details).
- ```npm run serve``` to serve the built application (see the Building and deploying section for more details).

The complete list of scripts can be found in the ```package.json``` file.

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
