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
Make sure to properly setup your remote repositories.

__Careful with this command because this script will assume all changes you made on the source code is final. It will generate a build directory out of the source folder and force push the files inside `build` folder to the master branch of `git@github.com:uxdvo/uxdvo.github.io.git`__

__Before you can deploy make sure to commit and push all changes first on your origin repository__

```
npm run deploy
```

### Features:

* ES6 Support via [babel](https://babeljs.io/) (v7)
* SASS Support via [sass-loader](https://github.com/jtangelder/sass-loader)
* Linting via [eslint-loader](https://github.com/MoOx/eslint-loader)

When you run `npm run build` we use the [mini-css-extract-plugin](https://github.com/webpack-contrib/mini-css-extract-plugin) to move the css to a separate file. The css file gets included in the head of the `index.html`.
