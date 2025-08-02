# TypeScript

TypeScript（简称 TS）是一种高级编程语言，它为 JavaScript 添加了可选的类型注解，从而提供了静态类型系统。它被设计用于开发大型应用程序，并可以编译成 JavaScript。TypeScript 由微软开发，作为免费和开源软件，在 Apache License 2.0 下发布。

## 安装

```bash
npm install -g typescript
```

## 使用

初始化

```bash
tsc --init
```

监控文件变化自动编译

```bash
tsc -w
```

## 类型

热血沸腾的类型体操，令人又爱又恨😇

### 类型注解

当声明变量时，可以给添加类型注解，在大多数情况下并不是必要的。TypeScript 会尽可能自动推断代码中的类型

```ts
let jm: number = 350234;
```

### 任意类型

`any`：任意类型，什么都可以  
`unknown`：未知类型，不知道是什么

使用 `any` 会失去类型检查，过多使用 `any` 的话 TypeScript 就变成 AnyScript 了，一座新的屎山诞生了🤓

`unknown` 比 `any` 更安全，它不能赋给其他变量，也不能调用方法，不能访问属性

### 值类型

`number`： 数字类型，例如 `114514`

`bigint`： 大数字类型，例如 `9007199254740991n`

`string`：字符串类型，例如 `"hello world"`

`boolean`：布尔类型，`true` 和 `false`

`null`：空值 `null`

`undefined`：未定义的值 `undefined`

### object

`object`：所有非值类型的类型，例如对象、数组、函数等

```ts
let user: object = { name: "John Smith", age: 18 };
let arr: object = [22, 33, 2233];
let func: object = () => 666;
```

`Object`（`interface Object`）：内置类型，接收一切非 `null` 或 `undefined` 的值，无法访问属性

`{}`：字面量，接收一切非 `null` 或 `undefined` 的值，无法访问属性，常用于表示非空值

### 内置类型

例如 `Object`、`Number`、`String`、`Boolean`、`Error`、`Promise<T>` 等，是内置类型

### 数组

### 元组

### 联合类型

我们联合！！！

```ts
let id: number | null = null;
id = 114514;
let more:
    | number
    | string
    | boolean
    | null = null;
```

### 类型别名

### 接口

### 交叉类型

### 无返回与不返回

`void`：无返回值  
`never`：从不返回

```ts
function returnVoid(): void {}
function neverReturn(): never { throw new Error('error'); }
```

### 枚举
