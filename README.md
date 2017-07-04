## address-picker

本插件基于mint-ui的picker和popup组件进行封装的三级地址联动，
使用效果类似于mint-ui的datetime-picker组件效果，如若需要自
定义地址数据，可根据address.js数据结果对数据进行替换
### Install

``` bash
npm i address-picker --save
```

Code Example (ES6)
``` html
<template>
    <div>
        <h5 @click="show=true;">地址选择</h5>
        <address-picker  
            @confirm="handle" 
            v-model="show"
        ></address-picker>
    </div>
</template>
```
``` js
import addressPicker from 'address-picker';
    let components = {};
    components[addressPicker.name] = addressPicker;
    export default {
      components : components,
      data () {
        return {
          show : false
        }
      },
      methods : {
        handle (value) {
          console.log(value);
        }
      },
    }
```

### Props
- v-model: 绑定一个本地变量控制组件显示与隐藏.
- confirm: 选择地址之后的回掉，返回地址信息的对象.


### Contributions

Your contributions and suggestions are welcome 😄😄😄💐💐💐.


# address-picker
