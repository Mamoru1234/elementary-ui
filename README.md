
#[Elementary-UI](http://www.elementary-ui.com/)
[![npm package](https://)](https://)
[![Build Status](https://)](https://)
[![Gitter](https://)](https://)

[![PeerDependencies](https://)](https://)
[![Dependencies](https://)](https://)
[![DevDependencies](https://)](https://)

Elementary-UI is a set of [React](http://facebook.github.io/react/) hight performance and fully customizable React
Components that implement  
[Google's Material Design](https://www.google.com/design/spec/material-design/introduction.html)
specification by default.

Check out our [documentation site](http://www.elementary-ui.com/) for live examples.
It's still a work in progress, but hopefully you can see where we're headed.

**Recently Updated?** Please read the [changelog](https://), this README and the documentation before posting an issue.

## Prerequisites

We recommend that you get to know [React](http://facebook.github.io/react/)
before diving into elementary-ui. Elementary-UI is a set of React components,
so understanding how React fits into web development is important.

(If you're not familiar with Node, or with the concept of Single Page Applications (SPAs),
head over to the [documentation website](http://)
for a quick introduction before you read on.)

## Installation

Elementary-UI is available as an [npm package](https://).

**Stable channel**
```sh
npm install elementary-ui
```

Our next version (`0.1.0`) is coming soon!

**Pre-release channel **
```sh
npm install elementary-ui@next
```



### React-Tap-Event-Plugin

Some components use
[react-tap-event-plugin](https://github.com/zilverline/react-tap-event-plugin) to
listen for touch events because onClick is not fast enough
_This dependency is temporary and will eventually go away._ Until then,
be sure to inject this plugin at the start of your app.

```js
import injectTapEventPlugin from 'react-tap-event-plugin';

// Needed for onTouchTap
// http://stackoverflow.com/a/34015469/988941
injectTapEventPlugin();
```

### Roboto Font

Elementary-UI was designed with the [Roboto](http://www.google.com/fonts/specimen/Roboto)
font in mind. So be sure to include it in your project. Here are
[some instructions](http://www.google.com/fonts#UsePlace:use/Collection:Roboto:400,300,500)
on how to do so.

## Usage

Elementary-UI components are easy to use.

Here is a quick example to get you started:

**./App.js**
```jsx
import React from 'react';
import ReactDOM from 'react-dom';
import MyAwesomeReactComponent from './MyAwesomeReactComponent';

const App = () => (
  <MyAwesomeReactComponent />
);

ReactDOM.render(
  <App />,
  document.getElementById('app')
);
```

**./MyAwesomeReactComponent.js**
```jsx
import React from 'react';
import RaisedButton from 'elementary-ui/RaisedButton';

const MyAwesomeReactComponent = () => (
  <RaisedButton label="Default" />
);

export default MyAwesomeReactComponent;
```

Please refer to each component's documentation page to see how they should be imported.

## Customization

We have implemented a default theme to render all Elementary-UI components.
Styling components to your liking is simple and hassle-free. This can be
achieved in the following two ways:

* [Use a custom theme to style components](http://)
* [Override individual component styles via the `style` prop](http://)
* [Override individual component classes via the `className` prop](http://)

## Examples

There are 2 projects that you can look at to get started. They can be found in the
[examples folder](https://).
These projects are basic examples that show how to consume elementary-ui components
in your own project. Projects use [webpack](http://webpack.github.io/) for module bundling and building.

The source code for this documentation site is also included in the repository.
This is a slightly more complex project that also uses webpack, and contains
examples of every elementary-ui component. Check out the
[docs folder](https://)
for build instructions.

## Roadmap

The future plans and high priority features and enhancements can be found
in the [ROADMAP.md](https://) file.

## Contribute

[Elementary-UI](http://) came about from our love of
[React](http://facebook.github.io/react/) and
[Google's Material Design](https://www.google.com/design/spec/material-design/introduction.html).
We'd greatly appreciate any [contribution](https://)
you make. :)

## License
This project is licensed under the terms of the
[MIT license](https://)
