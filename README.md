# 1. Clone this repository

# 2. Install the following npm packages

```
npm init
npm i -S {react,react-dom}
npm i -D babel-{core,loader} babel-preset-react
npm i -D webpack webpack-dev-server html-webpack-plugin
```

# 3. Make changes

Make changes to `index.html` and `script.js` in the `/src` directory. I have already added an `<App />` component and its associated `App.js` file within `/src/components` as a starting point, now populated only with an `<h1>`.

# 4. Build and Run

```
npm run build
npm run start
```
# 5. For GitHub pages

Create your own GitHub repository. Remove the cloned remote repository and replace it with your own. 

```
git remote rm origin
git remote add origin your-repo-url-goes-here
git checkout -b gh-pages
git subtree push --prefix dist origin gh-pages
```
