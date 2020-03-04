# Robotlab_app
This is the Robotlab app Tutorial We design the GUI for the Robot

-----------------------------------------------------
# STEP1. Learning the Polymer with PWA Starter Kit

## 1. Tutorial Polymer with PWA Starter kit
https://pwa-starter-kit.polymer-project.org/overview

template-responsive-drawer-layout [code](https://github.com/Polymer/pwa-starter-kit/tree/template-responsive-drawer-layout), [demo](https://template-responsive-drawer-layout-dot-pwa-starter-kit.appspot.com/)

This template is very similar to the master template, in the sense that it keeps both Redux for state management, and all of the UI elements. The main difference is that the wide screen layout displays a persistent app-drawer, inline with the content.

## 2. Setup 
This page will take you through the steps you need to do to build and run the sample app locally.

```
git clone --depth 1 https://github.com/Polymer/pwa-starter-kit my-app
cd my-app
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
