# SPA on github pages

[Demo](https://sriramrudraraju.github.io/spa-ghpages/)

### Deploy to gh-pages
* When code pushed to main, git actions will build and deploy the code to gh-pages.
* Or manually run `npm run deploy` to deploy the code to gh-pages.

### Routing for react app
* React router [setup](https://v5.reactrouter.com/web/guides/quick-start/installation)

### Base path
* For base path follow as below
* From Package.json
```json
homepage: `https://<userName>.github.io/<repositoryName>`
```
* Use repositoryName from in react-router browserRouter's baseName
```javasccript
  <Router basename='/<repositoryName>'>
```