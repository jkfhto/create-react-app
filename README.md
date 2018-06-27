 # Create React App [![Build Status](https://travis-ci.org/facebook/create-react-app.svg?branch=master)](https://travis-ci.org/facebook/create-react-app)

Create React apps with no build configuration.

创建React应用程序，无需编译配置

* [Creating an App](#creating-an-app) – How to create a new app.    如何创建一个新的应用程序
* [User Guide](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md) – How to develop apps bootstrapped with Create React App.  如何使用Create React App开发应用程序



Create React App works on macOS, Windows, and Linux.<br>创建可在macOS，Windows和Linux上运行的React App<br><br>
If something doesn’t work, please [file an issue](https://github.com/facebook/create-react-app/issues/new).<br>如果出现问题，请提交问题

## Quick Overview  快速概览

```sh
npx create-react-app my-app
cd my-app
npm start
```

*([npx](https://medium.com/@maybekatz/introducing-npx-an-npm-package-runner-55f7d4bd282b) comes with npm 5.2+ and higher, see [instructions for older npm versions](https://gist.github.com/gaearon/4064d3c23a77c74a3614c498a8bb1c5f))*

Then open [http://localhost:3000/](http://localhost:3000/) to see your app.<br>Then open http://localhost:3000/ to see your app.<br><br>
When you’re ready to deploy to production, create a minified bundle with `npm run build`.<br>您准备好部署到生产环境时，请使用npm run build创建压缩包

<p align='center'>
<img src='https://cdn.rawgit.com/facebook/create-react-app/27b42ac/screencast.svg' width='600' alt='npm start'>
</p>

### Get Started Immediately  开始

You **don’t** need to install or configure tools like Webpack or Babel.<br>你不需要安装或配置像Webpack或Babel这样的工具<br><br>
They are preconfigured and hidden so that you can focus on the code.<br>它们已预先配置并隐藏，以便您可以专注于代码

Just create a project, and you’re good to go.

## Creating an App  创建应用程序

**You’ll need to have Node >= 6 on your local development machine** (but it’s not required on the server). You can use [nvm](https://github.com/creationix/nvm#installation) (macOS/Linux) or [nvm-windows](https://github.com/coreybutler/nvm-windows#node-version-manager-nvm-for-windows) to easily switch Node versions between different projects.<br>您需要在本地开发机器上安装Node6及以上版本（但服务器上不需要）。 您可以使用[nvm]或[nvm-windows]在不同项目之间轻松切换Node版本。

To create a new app, you may choose one of the following methods:<br>要创建一个新的应用程序，您可以选择以下方法之一：

### npx

```sh
npx create-react-app my-app
```

*([npx](https://medium.com/@maybekatz/introducing-npx-an-npm-package-runner-55f7d4bd282b) comes with npm 5.2+ and higher, see [instructions for older npm versions](https://gist.github.com/gaearon/4064d3c23a77c74a3614c498a8bb1c5f))*

### npm

```sh
npm init react-app my-app
```
*`npm init <initializer>` is available in npm 6+*

### Yarn

```sh
yarn create react-app my-app
```
*`yarn create` is available in Yarn 0.25+*

It will create a directory called `my-app` inside the current folder.<br>
Inside that directory, it will generate the initial project structure and install the transitive dependencies:<br>它会在当前文件夹内创建一个名为my-app的目录。在该目录内，它将生成初始项目结构并安装依赖项：

```
my-app
├── README.md
├── node_modules
├── package.json
├── .gitignore
├── public
│   ├── favicon.ico
│   ├── index.html
│   └── manifest.json
└── src
    ├── App.css
    ├── App.js
    ├── App.test.js
    ├── index.css
    ├── index.js
    ├── logo.svg
    └── registerServiceWorker.js
```

No configuration or complicated folder structures, just the files you need to build your app.<br>
Once the installation is done, you can open your project folder:<br>没有配置或复杂的文件夹结构，只需要构建应用程序所需的文件。
安装完成后，您可以打开项目文件夹：

```sh
cd my-app
```

Inside the newly created project, you can run some built-in commands:<br>在新创建的项目中，您可以运行一些内置命令

### `npm start` or `yarn start`

Runs the app in development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.<br>以开发模式运行应用程序。 在浏览器中打开http：// localhost：3000查看它

The page will automatically reload if you make changes to the code.<br>
You will see the build errors and lint warnings in the console.<br>如果您更改了代码，该页面将自动重新加载。 您将在控制台中看到构建错误和lint警告。

<p align='center'>
<img src='https://cdn.rawgit.com/marionebl/create-react-app/9f62826/screencast-error.svg' width='600' alt='Build errors'>
</p>

### `npm test` or `yarn test`

Runs the test watcher in an interactive mode.<br>
By default, runs tests related to files changed since the last commit.<br>以交互模式运行测试观察器。
默认情况下，运行与上次提交后更改的文件相关的测试。

[Read more about testing.](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#running-tests)

### `npm run build` or `yarn build`

Builds the app for production to the `build` folder.<br>
It correctly bundles React in production mode and optimizes the build for the best performance.<br>将生成的应用程序构建到build文件夹。
它在生产模式下正确捆绑React并优化构建以获得最佳性能。

The build is minified and the filenames include the hashes.<br>
By default, it also [includes a service worker](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#making-a-progressive-web-app) so that your app loads from local cache on future visits.<br>构建被缩小，文件名包含hashes。 默认情况下，它还包含service worker，以便您的应用程序在未来访问时从本地缓存加载

Your app is ready to be deployed.  您的应用已准备好进行部署了。

## User Guide  用户指南

The [User Guide](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md) includes information on different topics, such as:<br>用户指南包含有关不同主题的信息，例如

- [Updating to New Releases](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#updating-to-new-releases)更新到新版本
- [Folder Structure](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#folder-structure)文件夹结构
- [Available Scripts](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#available-scripts)可用的脚本
- [Supported Browsers](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#supported-browsers)支持的浏览器
- [Supported Language Features and Polyfills](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#supported-language-features-and-polyfills)支持的语言功能和Polyfills
- [Syntax Highlighting in the Editor](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#syntax-highlighting-in-the-editor)语法在编辑器中突出显示
- [Displaying Lint Output in the Editor](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#displaying-lint-output-in-the-editor)在编辑器中显示Lint输出
- [Formatting Code Automatically](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#formatting-code-automatically)自动格式化代码
- [Debugging in the Editor](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#debugging-in-the-editor)在编辑器中调试
- [Changing the Page `<title>`](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#changing-the-page-title)改变页面<title>
- [Installing a Dependency](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#installing-a-dependency)安装依赖项
- [Importing a Component](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#importing-a-component)导入组件
- [Code Splitting](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#code-splitting)代码拆分
- [Adding a Stylesheet](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#adding-a-stylesheet)添加样式表
- [Post-Processing CSS](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#post-processing-css)CSS后处理
- [Adding a CSS Preprocessor (Sass, Less etc.)](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#adding-a-css-preprocessor-sass-less-etc)添加一个CSS预处理器（Sass，Less等）
- [Adding Images, Fonts, and Files](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#adding-images-fonts-and-files)添加图像，字体和文件
- [Using the `public` Folder](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#using-the-public-folder)
- [Using Global Variables](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#using-global-variables)
- [Adding Bootstrap](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#adding-bootstrap)
- [Adding Flow](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#adding-flow)
- [Adding a Router](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#adding-a-router)
- [Adding Custom Environment Variables](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#adding-custom-environment-variables)
- [Can I Use Decorators?](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#can-i-use-decorators)
- [Fetching Data with AJAX Requests](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#fetching-data-with-ajax-requests)
- [Integrating with an API Backend](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#integrating-with-an-api-backend)
- [Proxying API Requests in Development](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#proxying-api-requests-in-development)
- [Using HTTPS in Development](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#using-https-in-development)
- [Generating Dynamic `<meta>` Tags on the Server](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#generating-dynamic-meta-tags-on-the-server)
- [Pre-Rendering into Static HTML Files](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#pre-rendering-into-static-html-files)
- [Running Tests](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#running-tests)
- [Debugging Tests](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#debugging-tests)
- [Developing Components in Isolation](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#developing-components-in-isolation)
- [Publishing Components to npm](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#publishing-components-to-npm)
- [Making a Progressive Web App](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#making-a-progressive-web-app)
- [Analyzing the Bundle Size](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#analyzing-the-bundle-size)
- [Deployment](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#deployment)
- [Advanced Configuration](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#advanced-configuration)
- [Troubleshooting](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#troubleshooting)

A copy of the user guide will be created as `README.md` in your project folder.<br>用户指南的副本将在您的项目文件夹中创建为README.md

## How to Update to New Versions?  如何更新到新版本？

Please refer to the [User Guide](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#updating-to-new-releases) for this and other information.有关此信息和其他信息，请参阅用户指南

## Philosophy  原理,理论

* **One Dependency:** There is just one build dependency. It uses Webpack, Babel, ESLint, and other amazing projects, but provides a cohesive curated experience on top of them.<br>一个依赖：只有一个构建依赖。它使用Webpack，Babel，ESLint和其他优秀的项目，但在它们之上提供了有凝聚力的策划体验

* **No Configuration Required:** You don't need to configure anything. Reasonably good configuration of both development and production builds is handled for you so you can focus on writing code.<br>无需配置：您不需要配置任何内容。为您处理开发和生产版本的合理良好配置，以便您可以专注于编写代码

* **No Lock-In:** You can “eject” to a custom setup at any time. Run a single command, and all the configuration and build dependencies will be moved directly into your project, so you can pick up right where you left off.<br>无锁定：您可以随时“eject”到自定义设置。运行一个命令，所有配置和构建依赖关系都会直接移入您的项目中，这样您就可以从停止的地方继续学习

## What’s Included?  包含什么？

Your environment will have everything you need to build a modern single-page React app:<br>您的环境将拥有构建现代单页React应用程序所需的一切

* React, JSX, ES6, and Flow syntax support.
* Language extras beyond ES6 like the object spread operator.
* Autoprefixed CSS, so you don’t need `-webkit-` or other prefixes.
* A fast interactive unit test runner with built-in support for coverage reporting.
* A live development server that warns about common mistakes.
* A build script to bundle JS, CSS, and images for production, with hashes and sourcemaps.
* An offline-first [service worker](https://developers.google.com/web/fundamentals/getting-started/primers/service-workers) and a [web app manifest](https://developers.google.com/web/fundamentals/engage-and-retain/web-app-manifest/), meeting all the [Progressive Web App](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#making-a-progressive-web-app) criteria.
* Hassle-free updates for the above tools with a single dependency.

Check out [this guide](https://github.com/nitishdayal/cra_closer_look) for an overview of how these tools fit together.<br>查看本指南以了解这些工具是如何组合在一起的

The tradeoff is that **these tools are preconfigured to work in a specific way**. If your project needs more customization, you can ["eject"](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#npm-run-eject) and customize it, but then you will need to maintain this configuration.<br>这些工具被预先配置为以特定方式工作。如果您的项目需要更多定制，您可以["eject"]并对其进行自定义，但是您需要维护此配置

## Popular Alternatives  适用场景

Create React App is a great fit for:创建React App非常适合

* **Learning React** in a comfortable and feature-rich development environment.在舒适和功能丰富的开发环境中学习React
* **Starting new single-page React applications.**启动新的单页面React应用程序
* **Creating examples** with React for your libraries and components.使用React为您的库和组件创建示例

Here’s a few common cases where you might want to try something else:<br>以下是一些您可能想做一些其他尝试时面临的常见情况

* If you want to **try React** without hundreds of transitive build tool dependencies, consider [using a single HTML file or an online sandbox instead](https://reactjs.org/docs/try-react.html).<br>如果您想尝试React而没有数百个传递式构建工具依赖项，请考虑[using a single HTML file or an online sandbox instead]

* If you need to **integrate React code with a server-side template framework** like Rails or Django, or if you’re **not building a single-page app**, consider using [nwb](https://github.com/insin/nwb), or [Neutrino](https://neutrino.js.org/) which are more flexible. For Rails specifically, you can use [Rails Webpacker](https://github.com/rails/webpacker).<br>如果您需要将React代码与Rails或Django等服务器端模板框架集成，或者如果您未构建单页应用程序，请考虑使用更灵活的nwb或Neutrino。特别是对于Rails，您可以使用Rails Webpacker

* If you need to **publish a React component**, [nwb](https://github.com/insin/nwb) can [also do this](https://github.com/insin/nwb#react-components-and-libraries), as well as [Neutrino's react-components preset](https://neutrino.js.org/packages/react-components/).<br>如果您需要发布React组件，[nwb]以及[Neutrino's react-components preset]也可以实现

* If you want to do **server rendering** with React and Node.js, check out [Next.js](https://github.com/zeit/next.js/) or [Razzle](https://github.com/jaredpalmer/razzle). Create React App is agnostic of the backend, and just produces static HTML/JS/CSS bundles.<br>如果你想使用React和Node.js进行服务器渲染，请查看Next.js或Razzle。创建React App不受后端的影响，只产生静态的HTML / JS / CSS包

* If your website is **mostly static** (for example, a portfolio or a blog), consider using [Gatsby](https://www.gatsbyjs.org/) instead. Unlike Create React App, it pre-renders the website into HTML at the build time.<br>如果您的网站大多是静态的（例如，投资组合或博客），请考​​虑使用Gatsby。与创建React App不同，它在构建时将网站预渲染为HTML

* If you want to use **TypeScript**, consider using [create-react-app-typescript](https://github.com/wmonk/create-react-app-typescript).<br>如果你想使用TypeScript，可以考虑使用create-react-app-typescript

* If you want to use **Parcel** instead of **Webpack** as your bundler, consider using [create-react-app-parcel](https://github.com/sw-yx/create-react-app-parcel).<br>如果您想使用Parcel而不是Webpack作为构建软件，请考虑使用create-react-app-parcel

* Finally, if you need **more customization**, check out [Neutrino](https://neutrino.js.org/) and its [React preset](https://neutrino.js.org/packages/react/).<br>最后，如果您需要更多定制，请查看Neutrino及其[React preset]

All of the above tools can work with little to no configuration.<br>所有上述工具都可以在很少或没有配置的情况下工作

If you prefer configuring the build yourself, [follow this guide](https://reactjs.org/docs/add-react-to-an-existing-app.html).<br>如果您更愿意自己配置构建，请按照本指南进行操作

## Contributing

We'd love to have your helping hand on `create-react-app`! See [CONTRIBUTING.md](CONTRIBUTING.md) for more information on what we're looking for and how to get started.

## React Native

Looking for something similar, but for React Native?<br>
Check out [Create React Native App](https://github.com/react-community/create-react-native-app/).

## Acknowledgements

We are grateful to the authors of existing related projects for their ideas and collaboration:

* [@eanplatter](https://github.com/eanplatter)
* [@insin](https://github.com/insin)
* [@mxstbr](https://github.com/mxstbr)

## License

Create React App is open source software [licensed as MIT](https://github.com/facebook/create-react-app/blob/master/LICENSE).
