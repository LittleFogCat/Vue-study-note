完全按照官方教程来进行：https://cn.vuejs.org/guide/quick-start.html

# 快速上手

## 线上尝试 

*   想要快速体验 Vue，你可以直接试试我们的[演练场](https://play.vuejs.org/#eNo9jcEKwjAMhl/lt5fpQYfXUQfefAMvvRQbddC1pUuHUPrudg4HIcmXjyRZXEM4zYlEJ+T0iEPgXjn6BB8Zhp46WUZWDjCa9f6w9kAkTtH9CRinV4fmRtZ63H20Ztesqiylphqy3R5UYBqD1UyVAPk+9zkvV1CKbCv9poMLiTEfR2/IXpSoXomqZLtti/IFwVtA9A==)。

*   如果你更喜欢不用任何构建的原始 HTML，可以使用 [JSFiddle](https://jsfiddle.net/yyx990803/2ke1ab0z/) 入门。

*   如果你已经比较熟悉 Node.js 和构建工具等概念，还可以直接在浏览器中打开 [StackBlitz](https://vite.new/vue) 来尝试完整的构建设置。

## 创建一个 Vue 应用[](https://cn.vuejs.org/guide/quick-start.html#creating-a-vue-application)

前提条件

*   熟悉命令行
*   已安装 18.3 或更高版本的 [Node.js](https://nodejs.org/)

在本节中，我们将介绍如何在本地搭建 Vue [单页应用](https://cn.vuejs.org/guide/extras/ways-of-using-vue.html#single-page-application-spa)。创建的项目将使用基于 [Vite](https://vitejs.dev/) 的构建设置，并允许我们使用 Vue 的[单文件组件](https://cn.vuejs.org/guide/scaling-up/sfc.html) (SFC)。

确保你安装了最新版本的 [Node.js](https://nodejs.org/)，并且你的当前工作目录正是打算创建项目的目录。在命令行中运行以下命令 (不要带上 `$` 符号)：

```
$ npm create vue@latest
```

这一指令将会安装并执行 [create-vue](https://github.com/vuejs/create-vue)，它是 Vue 官方的项目脚手架工具。你将会看到一些诸如 TypeScript 和测试支持之类的可选功能提示：

```
✔ Project name: … <your-project-name>
✔ Add TypeScript? … No / Yes
✔ Add JSX Support? … No / Yes
✔ Add Vue Router for Single Page Application development? … No / Yes
✔ Add Pinia for state management? … No / Yes
✔ Add Vitest for Unit testing? … No / Yes
✔ Add an End-to-End Testing Solution? … No / Cypress / Nightwatch / Playwright
✔ Add ESLint for code quality? … No / Yes
✔ Add Prettier for code formatting? … No / Yes
✔ Add Vue DevTools 7 extension for debugging? (experimental) … No / Yes

Scaffolding project in ./<your-project-name>...
Done.
```

如果不确定是否要开启某个功能，你可以直接按下回车键选择 `No`。在项目被创建后，通过以下步骤安装依赖并启动开发服务器：
```
$ cd <your-project-name>
$ npm install
$ npm run dev
```

你现在应该已经运行起来了你的第一个 Vue 项目！请注意，生成的项目中的示例组件使用的是[组合式 API](https://cn.vuejs.org/guide/introduction.html#composition-api) 和 `<script setup>`，而非[选项式 API](https://cn.vuejs.org/guide/introduction.html#options-api)。下面是一些补充提示：

*   推荐的 IDE 配置是 [Visual Studio Code](https://code.visualstudio.com/) + [Vue - Official 扩展](https://marketplace.visualstudio.com/items?itemName=Vue.volar)。如果使用其他编辑器，参考 [IDE 支持章节](https://cn.vuejs.org/guide/scaling-up/tooling.html#ide-support)。
*   更多工具细节，包括与后端框架的整合，我们会在[工具链指南](https://cn.vuejs.org/guide/scaling-up/tooling.html)进行讨论。
*   要了解构建工具 Vite 更多背后的细节，请查看 [Vite 文档](https://cn.vitejs.dev/)。
*   如果你选择使用 TypeScript，请阅读 [TypeScript 使用指南](https://cn.vuejs.org/guide/typescript/overview.html)。

当你准备将应用发布到生产环境时，请运行：
```
$ npm run build
```

此命令会在 `./dist` 文件夹中为你的应用创建一个生产环境的构建版本。关于将应用上线生产环境的更多内容，请阅读[生产环境部署指南](https://cn.vuejs.org/guide/best-practices/production-deployment.html)。

# 总结和补充

按照以下步骤创建并运行一个 Vue 项目：
1. 安装`node.js`；
2. 在父文件夹中，执行命令：`npm create vue@latest`；这一步的目的是创建一个基于最新版本的`vue`项目；
3. 进入项目文件夹，执行命令：`npm install`；这一步的目的是安装需要的依赖项；
4. 执行命令：`npm run dev`；这一步的目的是启动一个本地服务器，可以进行项目预览；

执行完以上步骤后，会有以下提示：
> VITE v6.0.5  ready in 636 ms
> 
>   ➜  Local:   http://localhost:5173/
>   ➜  Network: use --host to expose
>   ➜  Vue DevTools: Open http://localhost:5173/__devtools__/ as a separate window
>   ➜  Vue DevTools: Press Alt(⌥)+Shift(⇧)+D in App to toggle the Vue DevTools
> 
>   ➜  press h + enter to show help

如上所述，在浏览器访问`http://localhost:5173/` 即可预览刚才创建的项目了。

