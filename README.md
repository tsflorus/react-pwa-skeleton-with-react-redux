# React-js PWA Skeleton with React Redux

This project is a template/skeleton for starting a new PWA (Progressive Web App) using [create-react-app](https://reactjs.org/docs/create-a-new-react-app.html) and [React Redux](https://react-redux.js.org/).

## Installation

To work with this skeleton make sure that you have installed Node and npm.
If you haven't, just follow the next lines.

### Install Node and Npm
In order to check if Node is already installed on your computer, enter the following command in a terminal:
```bash
node --version
```
If Node is not installed, then go on the following URL and download the Node.js source code or installer for your platform.
[Download Node.js](https://nodejs.org/en/download/).

### Install and start the project
1. Clone the repo
```bash
git clone https://github.com/tsflorus/react-pwa-with-redux-skeleton.git
```
2. Install all npm packages
```bash
npm install
```
3. Start the project
```bash
npm start
```

## Usage

### PWA customization
By default, the serviceWorker is register in the ```/inidex.js``` file. If you don't want to use your app as a PWA, simply modify the line 17 as below:

From:
```javascript
serviceWorkerRegistration.register();
```
To:
```javascript
serviceWorkerRegistration.unregister();
```

1. index.html
The ```index.html``` file can be found under ```/public/index.html```. This file is simply the base html file for your app. Your react-app content will be loaded in the div with the id ```root```.

In this file you will have to change the ```meta``` of your app (on this project there are only the ```name``` and ```content``` fields but feel free to add more) as well as the ```title``` of your app (in the tags of the same name).

2. manifest.json
The ```manifest.json``` file can be found under ```/public/manifest.json```. It is the file that your browser will use in order to customize your PWA. In this file you will be able to change your app's icons, theme color and background color as well as its name.

All fields are declared in order to meet all manifest's requirements, To customize the file, simple edit values and/or replace icons files.

3. package.json
The ```package.json``` file can be found under ```/package.json```. In this file, you will be able to add custom scripts as well as dependencies (even if it is highly recommended to user your package manager for this purpose). 

In this file  you will have to change the value of the ```name``` field to fit your app's name.

### Redux usage
To learn more about redux, follow [this guide](https://redux.js.org/introduction/getting-started).
With this skeleton, the different parts of redux (actions and reducers) are separated in different folders. You will be able to find the actions folder under ```/src/actions``` and the reducers folder under ```/src/reducers```. 
To match the type of your dispatch in every actions add and export the type in ```/src/actions/type.js``` just as in the example you will find.

When adding a new reducer, make shure to import it in ```/src/reducers/index.js```and add it in ```combineReducer```.

## Contributing
Pull requests are welcome and are what makes open-source projects so initeresting.
To contribute,, just follow theses steps:

1. Fork the Project
2. Create your Feature Branch (git checkout -b feature/AmazingFeature)
3. Commit your Changes (git commit -m 'Add some AmazingFeature')
4. Push to the Branch (git push origin feature/AmazingFeature)
5. Open a Pull Request

## License
[MIT](https://choosealicense.com/licenses/mit/)
