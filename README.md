# react-redux-sokushu-practice

In this repo, I practice React and Redux, following the hands-on tutorial [React + Reduxを使ったWebアプリケーション開発速習会＠Wantedly](http://wantedly.connpass.com/event/33168/).

- [Article](http://qiita.com/shimpeiws/private/df31e2d70cc67c68115d)
- [Solution repo](https://github.com/shimpeiws/react-redux-sokushu)
- [API docs](https://github.com/shimpeiws/react-redux-sokushu-api/blob/master/api-doc.md)

---

## Get started

#### Install dependencies

```
npm install
```

#### Run two servers

Open a terminal and run the following:

```
npm run serve
```

Open another terminal and run the following:

```
# webpack-dev-server
# Provide the assets bundle via `http://localhost:8080/assets/build/issue.js`.
npm run webpack:serve
```

Visit `localhost:8000`

![スクリーンショット 2016-06-09 14.31.23.png](https://qiita-image-store.s3.amazonaws.com/0/29637/095942c1-0ab9-41d9-4af0-145af9df488f.png "スクリーンショット 2016-06-09 14.31.23.png")

---

## Structure of the project directory

```
root
├── .babelrc
├── finished
├── node_modules
├── package.json
├── public
├── server-finished.babel.js
├── server.babel.js
├── src
├── webpack-dev-server.babel.js
└── webpack.config.babel.js
```

- `.babelrc`
  + Basic configurations for `Babel`.
- `package.json`
  + Dependensies and scripts.
- `public`
  + Mounted as `localhost:8000`.
- `server.babel.js`
  + `Node` (`Express`) server that serves the `public` directory via `localhost:8000`.
- `src`
  + Development code.
-` webpack.config.babel.js`
  + Configuration for serving the compiled assets from `webpack dev server`.

---
