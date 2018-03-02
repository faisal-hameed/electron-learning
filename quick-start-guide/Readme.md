# Electron Framework Learning
Electron is an open-source framework which allows for the development of the desktop GUI applications using front and back end components.
Node.js runtime for the backend and Chromium for the front end.
We can build cross platform desktop app with JavaScript, HTML and CSS.
Electron runtime comes with rich native (operating system) APIs which focused on desktop applications.

## Following functionality is built it with electron apps:
1. Automatic Updates
2. Native Menus and notifications
3. Crash reporting
4. Debugging and profiling
5. Windows installers

## Popular apps built on electron
1. GitHub desktop
2. Postman
3. Slack
4. WordPress.com
5. Atom

## Basic structure of Electron app
A basic Electron application needs just these files:

`package.json` - Points to the app's main file and lists its details and dependencies.  
`main.js` - Starts the app and creates a browser window to render HTML. This is the app's main process.  
`index.html` - A web page to render. This is the app's renderer process.

## Writing your first app
A basic electron app would have the Following folder structure.  
your-app/  
  ├── package.json  
  ├── main.js  
  └── index.html

#### Creating package.json  
Create a new empty folder for your new Electron application. Open up your command line client and run `npm init` from that very folder. Follow the wizard to create following package.json

```
{
    "name": "your-app-name",
    "version": "0.1.0",
    "main": "main.js",
    "scripts": {
      "start": "electron ."
    }
}
```
#### Installing electron

`npm install --save-dev electron`

#### Electron development

Electron apps are developed in JavaScript using the same principals and methods found in Node.js development.

`electron` : Contains all APIs and features of Electron module
`app` : Lifecycle is managed by `electron.app`
`BrowserWindow` : GUI is created by `electron.BrowserWindow`

Create `main.js` file (To start main process).  
Create `index.html` file (To start renderer process)

#### Running electron application
Run `npm start` command from your app directory.


### Useful resources

1. Electron API Demos  
https://github.com/electron/electron-api-demos
2. Awesome-electron    
 https://github.com/sindresorhus/awesome-electron#boilerplates
