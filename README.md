# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Installation

We need NPM and Node.js to download and install node library packages

Step 1: Install NPM
```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
```
Step 2: Activate NPM
```bash
source ~/.bashrc 
```
Step 3: Install lastest LTS version of Node.js
```bash
nvm install -lts 
```
Step 4: Check version of Node.js and NPM
```bash
node -v npm -v
```

## Start Project
Step 1: Create a new React app
```bash
npx create-react-app my-app
```
Step 2: Navigate to your project directory
```bash
cd my-app
```
Step 3: Start the development server and open your default web browser with the URL **http://localhost:3000**
```bash
npm start
```
Step 4 (Optional): Create an optimized production build of your app  in the build directory when you're ready to deploy your React app
```bash
npm run build
```

## Folder Structure

After creation, your project should look like this:

> Note: public/index.html and src/index.js must exist with exact filenames.<br>
> You can delete or rename the other files.<br>
> You need to put any JS and CSS file inside src, otherwise Webpack won't see them.<br>

```
my-app/
├── README.md
├── node_modules
├── package.json
├── .gitignore
├── public/
│   ├── favicon.ico
│   ├── index.html
│   └── manifest.json
└── src/
    ├── App.css
    ├── App.js
    ├── App.test.js
    ├── index.css
    ├── index.js
    ├── logo.svg
    └── serviceWorker.js
    └── setupTests.js
```

## How to Structure React Project?
```
my-app/
│
├── node_modules (.gitignore)
├── public/
│   ├── favicon.ico
│   ├── index.html
│   ├── logo192.png
│   ├── logo512.png
│   ├── manifest.json
│   └── robots.txt
├── src/
│   ├── assets/
│   │   ├── fonts/
│   │   │   ├── myFont.ttf
│   │   ├── images/
│   │   │   ├── myImage.png
│   │   ├── styles/
│   │   │   ├── styles.css
│   ├── components/
│   │   ├── Button.jsx
│   │   ├── FormInput.jsx
│   ├── context/
│   │   ├── AuthContext.js
│   ├── data/
│   │   ├── configValues.json
│   │   ├── constants.js
│   ├── features/
│   │   ├── Authentication/
│   │   │   ├── assets/
│   │   │   ├── components/
│   │   │   ├── Authentication.js
│   │   ├── Order/
│   │   │   ├── components/
│   │   │   ├── hooks/
│   │   │   ├── Order.js
│   ├── hooks
│   │   ├── useFetch.js
│   │   ├── useLocalStorage.js
│   ├── services/
│   │   ├── api.js
│   ├── store/
│   │   ├── reducer.js
│   │   ├── saga.js
│   │   ├── store.js
│   ├── utils/
│   │   │   ├── formatDate.js
│   │   │   ├── sessionStorage.js
│   ├── App.css
│   ├── App.js
│   ├── App.test.js
│   ├── index.css
│   ├── index.js
│   ├── logo.svg
│   ├── reportWebVitals.js
│   └── setupTests.js
├── .gitignore
├── package-lock.json
├── package.json
└── README.md
```
* **public/ -** Contains files that will be publicly accessible.
* **src/ -** Contains the source code of your React application.
* **assets/ -** Contains static assets such as fonts, images, or stylesheets that are used within your application.
* **components/ -** Contains reusable React components used throughout your application.
* **context/ -** Contains React context providers used for managing global state within your application.
* **data/ -** Contains any constant data that doesn't change, like JSON files.
* **features/ -** Contains a mini version of the source folder for each of your different features.
* **hooks/ -** Contains custom React hooks used within your application.
* **services/ -** Contains files to handle API interactions, including fetching and sending data to and from your backend.
* **store/ -** Contains files related to state management using libraries like Redux, including reducers, actions, and middleware.
* **utils/ -** Contains pure functions (e.g., functions that return the same output for the same input and don't have side effects) or helper modules used within your application. These utilities can include functions for data manipulation, formatting, or general-purpose tasks.

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).
