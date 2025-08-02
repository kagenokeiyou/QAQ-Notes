# Vue

Vue 是一个开源的 MVVM (Model-View-ViewModel) 前端 JavaScript 框架，用于构建用户界面和单页应用程序

## 创建项目

```bash
npm create vue@latest
cd your-project-name
npm install
npm run dev
```

## 创建应用

```html
<!-- index.html -->
<!-- ... -->
    <div id="app"></div>
<!-- ... -->
```

```js
// main.js
import { createApp } from 'vue'
import App from './App.vue'

createApp(App).mount('#app')
```

使用 `createApp()` 创建应用，然后使用 `mount()` 方法将应用挂载到 DOM 元素中

传入 `createApp()` 的参数是一个组件，每个应用都需要有一个根组件，其他组件都是子组件

## 单文件组件

一般将 Vue 组件定义在一个单独的 `.vue` 文件中，这被称为单文件组件（SFC, Single File Component）

## 模板语法

## Typescript

### `lang="ts"`

在 `<script>` 或 `<script setup>` 标签上加上 `lang="ts"` 属性启用 Typescript

```html
<script setup lang="ts">
    // ...
</script>
```

### `ref()`

`ref()` 会根据初始化值推导类型，也可显式声明类型。若未给出初始值，则会得到一个包含 `undefined` 的联合类型

```ts
const ciallo = ref('0721'); // Ref<string>
const aaa: Ref<string | number> = ref(114514);
const homo = ref<string | number>(1919810);
const x = ref<number>(); // Ref<number | undefined>
```
