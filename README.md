## React Native Feather Icons

[![npm](https://img.shields.io/npm/v/react-native-feather.svg)](https://www.npmjs.com/package/react-native-feather)

#### Simply beautiful SVG icons as React Native SVG components.
This repository is a copy of the [colebemis](https://github.com/colebemis/) React Feather project.

The only difference between the projects is that this project outputs React Native SVG components that will render on React Native platforms.

### Installation
    npm install react-native-feather --save

### Usage

```javascript
import { Camera } from 'react-feather';

class MyClass extends React.Component {
  render() {
    return <Camera />
  }
}
```
If you are using WebPack, you can import only one icon.
```javascript
import Camera from 'react-native-feather/dist/icons/camera';

class MyClass extends React.Component {
  render() {
    return <Camera />
  }
}
```
If you can't use ES6 imports, it's possible to include icons from the compiled folder ./dist.
```javascript
var Camera = require('react-native-feather/dist/icons/camera').default;

var MyComponent = React.createClass({
  render: function () {
    return (
      <Camera />
    );
  }
});
```
You can also include the whole icon pack:

```javascript
import * as Icon from 'react-native-feather';

class MyClass extends React.Component {
  render() {
    return <Icon.Camera />
  }
}
```
Icons can be configured with inline props:
```javascript
<Icon.AlertCircle color="red" size={48} />
```
