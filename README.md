<h3 align="center">vue开发前期 文本填充 图片占位</h3>

---

## 介绍

`vue-fill` 是一款 基于 `vue 2.X` 的自定义指令，可以实现开发前期 图片 以及文本的填充。

## 安装

### 方式一. 通过 npm 安装 (推荐)

支持使用 npm 安装第三方包，

```bash
# 通过 npm 安装
npm i vue-fill
```

### 方式二. 下载代码

直接通过 git 下载源代码
```bash
git clone https://github.com/HunterXing/vue-fill.git
```

## 使用

`main.js`

```js
import vueFill from 'vue-fill';
Vue.use(vueFill);
```

`template`

```vue
 <p v-fill></p>
 <p v-fill="text"></p>
 <img v-fill="[100,200]" />
```

```js
data() {
    return {
      text: '自定义文本'
    }
}
```

上面第一种方式，将生成随机字符串

第二种方式，将生成自定义的文本

第三种方式，将生成图片占位，大小自定义



