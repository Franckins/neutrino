# hot

`@neutrinojs/hot` is Neutrino middleware for enabled Hot Module Replacement with webpack's `HotModuleReplacementPlugin`. This middleware is usually only added during development.

![](https://img.shields.io/npm/v/@neutrinojs/hot.svg) ![](https://img.shields.io/npm/dt/@neutrinojs/hot.svg)

## Requirements

* Node.js v8.3+
* Yarn v1.2.1+, or npm v5.4+
* Neutrino v8

## Installation

`@neutrinojs/hot` can be installed via the Yarn or npm clients.

#### Yarn

```bash
❯ yarn add @neutrinojs/hot
```

#### npm

```bash
❯ npm install --save @neutrinojs/hot
```

## Usage

`@neutrinojs/hot` can be consumed from the Neutrino API, middleware, or presets. Require this package and plug it into Neutrino:

```javascript
// Using function middleware format
const hot = require('@neutrinojs/hot');

neutrino.use(hot);
```

```javascript
// Using object or array middleware format
module.exports = {
  use: ['@neutrinojs/hot']
};
```

## Customization

`@neutrinojs/hot` creates some conventions to make overriding the configuration easier once you are ready to make changes.

### Plugins

The following is a list of plugins and their identifiers which can be overridden:

| Name | Description | Environments and Commands |
| --- | --- | --- |
| `hot` | Enables Hot Module Replacement. | all |

## Contributing

This middleware is part of the [neutrino-dev](https://github.com/mozilla-neutrino/neutrino-dev) repository, a monorepo containing all resources for developing Neutrino and its core presets and middleware. Follow the [contributing guide](https://neutrino.js.org/contributing) for details.
