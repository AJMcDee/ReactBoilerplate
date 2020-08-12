# About this repository

As an early-stage programmer excited about React, I have found the installation process confusing and complex. Although the create-react-app package has been useful, I often encountered errors with random lines in the configuration, and the entire thing felt bloated when all I wanted was to make something small and simple to practice my newfound skills. As a result, I created this boilerplate for myself, and decided to share it with the world in the hopes that other React students will also find it useful.

The following steps have been tested thoroughly in the Ubuntu BASH Shell: 

## 1. Clone this repository and `cd` into it

```
git clone https://github.com/AJMcDee/ReactBoilerplate.git
cd ReactBoilerplate
```

## 2. Install the following npm packages

```
npm init
npm i -S {react,react-dom}
npm i -D babel-{core,loader} babel-preset-react
npm i -D webpack webpack-dev-server html-webpack-plugin
```

## 3. Make changes

Make changes to `index.html` and `script.js` in the `/src` directory. I have already added an `<App />` component and its associated `App.js` file within `/src/components` as a starting point, now populated only with an `<h1>`.

## 4. Build and Run to view the app in development

```
npm run build
npm run start
```
## 5. For GitHub pages

Stage and commit as usual.

Create your own GitHub repository. Remove the cloned remote repository and replace it with your own. Do one commit to remote master and then deploy the `/dist` directory to gh-pages.

```
git remote rm origin
git remote add origin your-repo-url-goes-here
git push -u origin master
git checkout -b gh-pages
git subtree push --prefix dist origin gh-pages
```
