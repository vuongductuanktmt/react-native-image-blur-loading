# React Native Image Blur Loading

React Native component for progressive image loading.

![](image-blur-loading.gif)

## Installation

Run in your root project directory

```bash
$ npm install react-native-image-blur-loading --save
```

## Usage

```jsx
import React, { Component } from 'react';
import { View } from 'react-native';
import ImageBlurLoading from 'react-native-image-blur-loading'

// ...
class MyComponent extends Component {
  render() {
    return (
      <View style={{ flex: 1 }}>
        <ImageBlurLoading
          thumbnailSource={{ uri: 'https://picsum.photos/id/1/16/16' }}
          source={{ uri: 'https://picsum.photos/id/1/600/600' }}
          style={{ flex: 1, width: null, height: null, resizeMode: 'contain' }}
          resizeMode='cover'
        />
      </View>
  }
}
```

## Properties
| Props | Description | Type | Required |
| --- | --- | --- | --- |
| [Image props ...](https://facebook.github.io/react-native/docs/image#props) | It accepts all the [Image props](https://facebook.github.io/react-native/docs/image#props) | - | - |
| `thumbnailSource` | The source of the thumbnail image. Should be a low resolution version of the image used in `imageSource`. | ImageSourcePropType | No |

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.


## License
[MIT](https://choosealicense.com/licenses/mit/)