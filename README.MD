# BEN NOTIFICATION 

### install
```
npm install --save ben-notification
```

```javascript
// nodeJs
const MSG = module.require('ben-notification')
```
```javascript
// ES6
import * as MSG from 'ben-notification'
```
```html
// html
<script src="assets/jQuery.js"></script>
<script src="assets/index.js"></script>
```


### HOW TO USE
```javascript
const MSG = module.require('ben-notification')

// alert
MSG.alert('Alert', 'this is one alert notification')
// success
MSG.success('Success', 'this is one success notification')
// warning
MSG.warning('Alert', 'this is one alert notification')
// error
MSG.error('Alert', 'this is one alert notification')

MSG.msg({
    title: '登鹳雀楼',
    content: '白日依山尽，黄河入海流。<br>欲穷千里目，更上一层楼。',
    icon: 'ion-android-happy',
    iconSmall: 'ion-checkmark-circled bounce animated',
    sound: true,
    sound_file: 'voice_on',
    color: '#d22121',
    timeout: '4000'
})
```


### option of  MSG.msg 

#### title
    type: string
    default :''
#### content
    type: string
    default :''
#### colors
    type: string
    default :''
#### icon
    type: string
    default: false
#### sound
    type: boolean 
    default: true
#### sound_path
    type: string
    default: "assets/sound/"
#### sound_file
    type:string
    default: "smallbox"
#### iconSmall
    type: string
    default: true
#### color
    type:string
    default: '#398bf7'
#### timeout
    type: number
    default: 3000
    
### CALLBACK
callback well be fun if this notification closed
```javascript
MSG.alert('first notification','内容',function() {
  MSG.alert('second notification','内容')
})
```