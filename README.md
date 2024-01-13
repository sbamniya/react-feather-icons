## Note

This is extension of (`react-feather`)[https://www.npmjs.com/package/react-feather], to allow configuring with React context, to define color and size of icons, instead of passing to each component individually. You can still pass both of these props to override the default configuration.

## React Feather Icons

[![npm version](https://img.shields.io/npm/v/react-feather-icon.svg?style=flat-square)](https://www.npmjs.com/package/react-feather-icon)
[![npm downloads](https://img.shields.io/npm/dm/react-feather-icon.svg?style=flat-square)](https://www.npmjs.com/package/react-feather-icon)

#### What is react-feather-icon?

`react-feather-icon` is forked from `react-feather` which is a collection of simply beautiful open source icons for React.js. Each icon is designed on a 24x24 grid with an emphasis on simplicity, consistency and readability.

#### Based on Feather Icons `v4.29.0`

https://feathericons.com/

### Installation

    yarn add react-feather-icon

or
  
 npm i react-feather-icon

### Usage

```javascript
import React from 'react';
import { Camera } from 'react-feather-icon';

const App = () => {
  return <Camera />;
};

export default App;
```

Icons can be configured with Provider:

```javascript
import React from 'react';
import { FeatherIconProvider, Camera } from 'react-feather-icon';

const App = () => {
  return (
    <FeatherIconProvider color="red" size={48}>
      <Camera />
    </FeatherIconProvider>
  );
};

export default App;
```

Icons can be configured with inline props:

```javascript
<Camera color="red" size={48} />
```

If you can't use ES6 imports, it's possible to include icons from the compiled folder ./dist.

```javascript
var Camera = require('react-feather/dist/icons/camera').default;

var MyComponent = React.createClass({
  render: function() {
    return <Camera />;
  },
});
```

You can also include the whole icon pack:

```javascript
import React from 'react';
import * as Icon from 'react-feather-icon';

const App = () => {
  return <Icon.Camera />;
};

export default App;
```
