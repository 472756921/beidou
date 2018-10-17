# Change Log

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

<a name="1.0.5"></a>
## [1.0.5](https://github.com/alibaba/beidou/compare/v1.0.4...v1.0.5) (2018-06-14)


### Bug Fixes

* wrong bin file excuted in windows [#63](https://github.com/alibaba/beidou/issues/63) ([#65](https://github.com/alibaba/beidou/issues/65)) ([d2f7bac](https://github.com/alibaba/beidou/commit/d2f7bac))




# Change Log

## [1.0.1](https://github.com/alibaba/beidou/compare/v1.0.0...v1.0.1) (2018-03-26)


### Bug Fixes

* prevent `lib/core/agent/index.js` unexpectly loaded by plugin loader ([#35](https://github.com/alibaba/beidou/issues/35)) ([c30f27e](https://github.com/alibaba/beidou/commit/c30f27e))



## 1.0.0 (2018-03-23)

### BREAKING CHANGE

* Node version must >= 8
* React/react-dom versions must >= 16
* Replace `koa-webpack-dev-middleware` with `webpack-dev-server`
* all [webpack configurations](https://webpack.js.org/configuration/) except **entry** are available in `configs#webpack` option, see [default config](https://github.com/alibaba/beidou/blob/master/packages/beidou-webpack/config/config.default.js)
* Move custom webpack config file path to `webpack.custom.configPath`, see [configuration](https://github.com/alibaba/beidou/blob/master/packages/beidou-webpack/README.md#configuration)
* Custom webpack config file api, see [custom webpack configuration](https://github.com/alibaba/beidou/blob/master/packages/beidou-webpack/README.md#custom-webpack-configuration)
* Remove `app.helper.resolveResource`, use `app.helper.asset` instead

### Features

* Upgrade to egg@2, support async/await style middlewares
* All in one manage tool - [beidou-cli](https://github.com/alibaba/beidou/blob/master/packages/beidou-cli/README.md), including init boilerplate, development, debug, test, build assets, start/stop production app, and so on.
* Custom view rendering process by [view middlewares](https://github.com/alibaba/beidou/blob/master/packages/beidou-view-react/README.md#custom-view-middlewares)
* Support [rax](https://github.com/alibaba/rax) isomorphic rendering, see [beidou-view-rax](https://github.com/alibaba/beidou/blob/master/packages/beidou-view-rax/README.md)
* Webpack support many frontend resource loaders, see [code](https://github.com/alibaba/beidou/blob/master/packages/beidou-webpack/config/webpack/webpack.browser.js)
* Webpack support CSS Modules with `.module.{css|scss|less}` files
* Dump webpack config to `[root]/run` directory
* Custom babel client targets by [configuration](https://github.com/alibaba/beidou/blob/master/packages/babel-preset-beidou-client/README.md#configuration)
* Handle many reasonable default configs, you may not need a lot of options in your config files, see [examples](https://github.com/alibaba/beidou/tree/master/examples)


## [0.3.5](https://github.com/alibaba/beidou/compare/v0.3.4...v0.3.5) (2017-12-20)


### Bug Fixes

* [#5](https://github.com/alibaba/beidou/issues/5) path separator on Windows ([10990bf](https://github.com/alibaba/beidou/commit/10990bf))


### Features

* remove config dump override ([a5576e1](https://github.com/alibaba/beidou/commit/a5576e1))
* server side resolve alias ([82257e3](https://github.com/alibaba/beidou/commit/82257e3))
