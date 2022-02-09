# SPA on github pages

[Demo](https://sriramrudraraju.github.io/spa-ghpages/)

### Creating react project
```
npx create-react-app <repositoryName> --template typescript
```

### [Deploy to gh-pages](https://create-react-app.dev/docs/deployment/#github-pages)
* When code pushed to main, git actions will build and deploy the code to gh-pages.
* Or manually run `npm run deploy` to deploy the code to gh-pages.

### [Routing for react app](https://v5.reactrouter.com/web/guides/quick-start/installation)
* For base path follow as below.
* From Package.json
```json
"homepage": "https://<userName>.github.io/<repositoryName>"
```
* Use repositoryName from package.json in react-router browserRouter's baseName
```javascript
  <Router basename='/<repositoryName>'>
```

### [spa-github-pages](https://github.com/rafgraph/spa-github-pages)
* Follow the basic instructions provided.
* Add & change 404.html, index.html in public folder.
* This 404.html will not be same for react-router page not found logic. Need to custom develop for react-router.