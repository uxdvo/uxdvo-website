# UXDVO Website Source Code

## IMPORTANT

Set your origin as `git@github.com:uxdvo/uxdvo-website.git`

```
git remote add origin git@github.com:uxdvo/uxdvo-website.git
```

Set your upstream as `git@github.com:uxdvo/uxdvo.github.io.git`

```
git remote add origin git@github.com:uxdvo/uxdvo.github.io.git
```

### Start Dev Server

```
npm start
```

### Build Prod Version

```
npm run build
```

### Deploy To Upstream
Make sure to properly setup your remote repositories

```
npm run build
```

### Features:

* ES6 Support via [babel](https://babeljs.io/) (v7)
* SASS Support via [sass-loader](https://github.com/jtangelder/sass-loader)
* Linting via [eslint-loader](https://github.com/MoOx/eslint-loader)

When you run `npm run build` we use the [mini-css-extract-plugin](https://github.com/webpack-contrib/mini-css-extract-plugin) to move the css to a separate file. The css file gets included in the head of the `index.html`.
