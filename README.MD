#vue-backTop
> backTop for vue.

## props:

```
 props: {
         //距离顶部多少距离，出现返回顶部的图标
         visibleOffset: {
            type: [String, Number],
            default: 600
          },
          //自定义，返回图标
          className: {
            type: String
          }
        },
```

## usage:
+ install:
```bash
npm install smalleast/vue-backTop --save


```

+ code:
```javascript
   import VueBackTop from '../components/backTop.vue'
    export default {
      data() {
        return {
          visibleOffset: 400
        };
      },
      components: {VueBackTop}
    };

```

+template
```
<template>
  <aside class="dev">
    <label v-for="i in [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30]">
      测试数据{{i}}
      <br>
    </label>
    <VueBackTop :visibleOffset="visibleOffset" :className="'no-bar'"></VueBackTop>
  </aside>
</template>
```

## resource:
+ http://www.cnblogs.com/Kummy/p/4966937.html
+ https://github.com/steven5538/vue-button
+ https://yarnpkg.com/en/docs/install
