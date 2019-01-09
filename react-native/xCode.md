## Running via XCode Issues

### Issue: Lexical or Preprocessor Issue
**Description**: When we run or build the application in Xcode

|Name|Version|
| ------------ | ------------ |
| react-native | 0.55.4 |
| xcode  |  10.1 |

```
Lexical or Preprocessor Issue
'config.h' file not found
```
**Solution**: Update react-native to 0.56.0

### Issue: main.jsbundle does not exist
**Description**: When we run or build the application in Xcode
**Solution**: run the script below.
```
react-native bundle --entry-file ./index.js --platform ios --bundle-output ios/main.jsbundle
```

### Issue: Cannot read property 'bindings' of null
**Description**: When we run `react-native bundle`

|Name|Version|
| ------------ | ------------ |
| react-native | 0.56.0 |
| xcode  |  10.1 |

**Solution**: Update `babel-preset-react-native` to 5.0.2. See [github
issue](https://github.com/babel/babel/issues/8575#issuecomment-429392213)
