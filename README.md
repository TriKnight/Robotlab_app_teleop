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

## 2. Confifuring and personalizing
