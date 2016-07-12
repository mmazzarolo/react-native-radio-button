# React-Native Radio Button
Just a simple radio button for React-Native.  

![](https://raw.githubusercontent.com/mmazzarolo/react-native-tips/master/imgs/radio-button.gif)

### Install it with NPM...
- Run `npm install --save react-native-radio-button` 
- Require it with `import RadioButton from 'react-native-radio-button'`
<br />

### ...or just copy it in your project
You can just copy `RadioButton.js` in your project and use it directly (`react-native-animatable` is required to make it work this way).    
<br />

### Usage
Not much to say here, the component itself is just presentational: you must handle the logic outside of it:
```javascript
<RadioButton
  animation={'bounceIn'}
  isSelected={true}
  onPress={() => doSomething('hello')}
/>
```
<br />

### Available props
| Prop | Description | Default |
|---|---|---|
|**`size`**|Size of the Radio Button. |`16`|
|**`innerColor`**|Color of the inner circle. |`dodgerblue`|
|**`outerColor`**|Color of the outer circle. |`dodgerblue`|
|**`isSelected`**|Is this Radio Button selected? |`false`|
|**`onPress`**|Function invoked on button press. |*None*|

The Radio Button is animated by the awesome [`react-native-animatable`](https://github.com/oblador/react-native-animatable).  
To enable the animation you can just pass it any `react-native-animatable` props (e.g. `animation`, `duration`, etc...).  
Hint: `animation={'bounceIn'}` is the animation that you can see in the preview gif above.
<br />

### Stateless component info
As you can see by taking a look at `RadioButton.js` the component is plain simple and you can modify it easily.  
If you're interested there's also a version of it written in a more function style [here](https://gist.github.com/mmazzarolo/3ed3883d5c838c7010c353c6f3ac2be8).  
