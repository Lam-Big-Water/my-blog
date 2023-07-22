---
title: The Road To React
---
# Hello-React

**In this first part of this learning experience, we'll cover the fundamentals of React, with which we'll create our first React project. Later we'll explore new use cases for React by implementing real features like client and server-side searching, remote data fetching, and advanced state management the same as developing an actual web application. By the end, you will have a fully running React application that interacts with real-world data.**
在学习体验的第一部分中，我们将介绍 React 的基础知识，并用它创建我们的第一个 React 项目。 之后我们将通过实现客户端和服务器端搜索、远程数据获取和高级状态管理等实际功能来探索 React 的新用例，就像开发实际的 Web 应用程序一样。 最后，您将拥有一个完全运行的 React 应用程序，可以与现实世界的数据进行交互。

## Hello React

**Single-page applications ([SPA](https://bit.ly/3BZOL1o)) have become increasingly popular with first-generation SPA frameworks like Angular (by Google), Ember, Knockout, and Backbone. Using these frameworks made it easier to build web applications that advanced beyond vanilla JavaScript and jQuery. React, yet another solution for SPAs, was released by Facebook later in 2013. All of them are used to create modern web applications in JavaScript.**
单页应用程序 ([SPA](https://bit.ly/3BZOL1o)) 在第一代 SPA 框架中变得越来越流行，例如 Angular（由 Google 开发）、Ember、Knockout 和 Backbone。 使用这些框架可以更轻松地构建超越普通 JavaScript 和 jQuery 的 Web 应用程序。 React 是 Facebook 于 2013 年晚些时候发布的另一种 SPA 解决方案。所有这些解决方案都用于用 JavaScript 创建现代 Web 应用程序。

**For a moment, let's go back in time before SPAs existed: In the past, websites and web applications were rendered from the server. A user visits a URL in a browser and requests one HTML file and all its associated HTML, CSS, and JavaScript files from a web server. After some network delay, the user sees the rendered HTML in the browser (client) and starts to interact with it. Every additional page transition (meaning: visiting another URL) would initiate this chain of events again. In this version from the past, essentially everything crucial is done by the server, whereas the client plays a minimal role by just rendering page by page. While barebones HTML and CSS were used to structure and style the application, just a little bit of JavaScript was thrown into the mix to make interactions (e.g. toggling a dropdown) or advanced styling (e.g. positioning a tooltip) possible. A popular JavaScript library for this kind of work was jQuery.**
让我们回到 SPA 存在之前的时间：过去，网站和 Web 应用程序是从服务器呈现的。 用户在浏览器中访问 URL，并向 Web 服务器请求一个 HTML 文件及其所有关联的 HTML、CSS 和 JavaScript 文件。 经过一段网络延迟后，用户在浏览器（客户端）中看到渲染的 HTML 并开始与其交互。 每次额外的页面转换（即：访问另一个 URL）都会再次启动该事件链。 在过去的这个版本中，基本上所有重要的事情都是由服务器完成的，而客户端仅通过逐页渲染来扮演最小的角色。 虽然使用准系统 HTML 和 CSS 来构造和设计应用程序的样式，但只添加了一点 JavaScript 来实现交互（例如切换下拉菜单）或高级样式（例如定位工具提示）。 用于此类工作的流行 JavaScript 库是 jQuery。

**In contrast, modern JavaScript shifted the focus from the server to the client. The most extreme version of it: A user visits a URL and requests _one small HTML file_ and _one larger JavaScript file_. After some network delay, the user sees the _by JavaScript rendered HTML_ in the browser and starts to interact with it. Every additional page transition _wouldn't_ request more files from the web server, but would use the initially requested JavaScript to render the new page. Also, every additional interaction by the user is handled on the client too. In this modern version, the server delivers mainly JavaScript across the wire with one minimal HTML file. The HTML file then executes all the linked JavaScript from the files on the client-side to render the entire application with HTML and uses JavaScript for its interactions.**
相比之下，现代 JavaScript 将焦点从服务器转移到了客户端。 最极端的版本是：用户访问 URL 并请求_一个小 HTML 文件_和_一个较大的 JavaScript 文件_。 经过一段网络延迟后，用户会在浏览器中看到 _by JavaScript 渲染的 HTML_ 并开始与其交互。 每个额外的页面转换不会从 Web 服务器请求更多文件，但会使用最初请求的 JavaScript 来呈现新页面。 此外，用户的每个额外交互也在客户端上处理。 在这一现代版本中，服务器主要通过网络传递 JavaScript 和一个最小的 HTML 文件。 然后，HTML 文件执行客户端文件中所有链接的 JavaScript，以使用 HTML 呈现整个应用程序，并使用 JavaScript 进行交互。

**React, among the other SPA solutions, makes this possible. Essentially a SPA is one bulk of JavaScript, which is neatly organized in folders and files, to create a whole application whereas the SPA framework (e.g. React) gives you all the tools to architect it. This JavaScript-focused application is delivered once over the network to your browser when a user visits the URL for your web application. From there, React, or any other SPA framework, takes over for rendering everything in the browser as HTML and for dealing with user interactions with JavaScript.**
React 以及其他 SPA 解决方案使这成为可能。 本质上，SPA 是 JavaScript 的一部分，它整齐地组织在文件夹和文件中，用于创建整个应用程序，而 SPA 框架（例如 React）为您提供了构建它的所有工具。 当用户访问您的 Web 应用程序的 URL 时，这个以 JavaScript 为中心的应用程序会通过网络一次性传送到您的浏览器。 从那里，React 或任何其他 SPA 框架将接管将浏览器中的所有内容呈现为 HTML 并处理用户与 JavaScript 的交互。

**With the rise of React, the concept of components became popular. Every component defines its look and feel with HTML, CSS, and JavaScript. Once a component is defined, it can be used in a hierarchy of components for creating an entire application. Even though React has a strong focus on components as a library, the surrounding ecosystem makes it a flexible framework. React has a slim API, a stable yet thriving ecosystem, and a welcoming community. We are happy to welcome you :-)**
随着React的兴起，组件的概念开始流行。 每个组件都使用 HTML、CSS 和 JavaScript 定义其外观。 一旦定义了组件，就可以在组件层次结构中使用它来创建整个应用程序。 尽管 React 非常注重组件作为库，但周围的生态系统使其成为一个灵活的框架。 React 拥有简洁的 API、稳定而繁荣的生态系统以及热情的社区。 我们很高兴欢迎您:-)


### Exercises

●Read more about [how we moved from websites to web applications](https://www.robinwieruch.de/web-applications/).  
●Watch [React.js: The Documentary](https://bit.ly/3xrvxkI).  
●Optional: Read more about [how to learn a framework](https://www.robinwieruch.de/how-to-learn-framework/).  
●Optional: Read more about [how to learn React](https://www.robinwieruch.de/learn-react-js/).  
●Read more about [JavaScript fundamentals needed for React](https://www.robinwieruch.de/javascript-fundamentals-react-requirements/) -- without worrying too much about React here -- to challenge yourself with several JavaScript features used in React.  
●Optional: [Leave feedback for this section](https://forms.gle/NTqhvyDaP1RjtanC6).  

---
---

## Requirements

**To follow this book, you'll need to be familiar with the basics of web development, i.e how to use HTML, CSS, and JavaScript. It also helps to understand [APIs](https://www.robinwieruch.de/what-is-an-api-javascript/), as they will be covered in this learning experience. Along with these skills, you'll need the following tools to code with me while reading this book.**
要阅读本书，您需要熟悉 Web 开发的基础知识，即如何使用 HTML、CSS 和 JavaScript。 它还有助于理解 API，因为本次学习体验中将涵盖这些内容。 除了这些技能之外，在阅读本书时，您还需要以下工具来与我一起编码。


### Editor and Terminal

**I have provided [a setup guide](https://www.robinwieruch.de/developer-setup/) to get you started with general web development. For this learning experience, you will need a text editor (e.g. Sublime Text) and a command line tool (e.g. iTerm). As an alternative, I recommend using an IDE, for example Visual Studio Code (also called VSCode), for beginners, as it's an all-in-one solution that provides an advanced editor with an integrated command line tool, and because it's a popular choice among web developers.**
我提供了一个设置指南来帮助您开始一般的 Web 开发。 对于此学习体验，您将需要一个文本编辑器（例如 Sublime Text）和一个命令行工具（例如 iTerm）。 作为替代方案，我建议初学者使用 IDE，例如 Visual Studio Code（也称为 VSCode），因为它是一种一体化解决方案，提供带有集成命令行工具的高级编辑器，并且因为它是一种流行的工具 Web 开发人员之间的选择。

**If you don't want to set up the editor/terminal combination or IDE on your local machine, [CodeSandbox](https://codesandbox.io), an online editor, is also a viable alternative. While CodeSandbox is a great tool for sharing code online, a local machine setup is a better tool for learning the different ways to create a web application. Also, if you want to develop applications professionally, a local setup will be required.**
如果您不想在本地计算机上设置编辑器/终端组合或 IDE，CodeSandbox（在线编辑器）也是一个可行的替代方案。 虽然 CodeSandbox 是在线共享代码的绝佳工具，但本地计算机设置是学习创建 Web 应用程序的不同方法的更好工具。 此外，如果您想专业开发应用程序，则需要本地设置。

**Throughout this learning experience, I will use the term command line, which will be used synonymously for the terms command line tool, terminal, and integrated terminal. The same applies to the terms editor, text editor, and IDE, depending on what you decided to use for your setup.**
在整个学习过程中，我将使用术语“命令行”，它将与术语“命令行工具”、“终端”和“集成终端”同义使用。 这同样适用于术语编辑器、文本编辑器和 IDE，具体取决于您决定在设置中使用什么。

**Optionally, I recommend managing projects on GitHub while we conduct the exercises in this book, and I've provided a short guide on how to use these tools.Github has excellent version control, so you can see what changes were made if you make a mistake or just want a more direct way to follow along.It's also a great way to share your code later with other people.**
可选地，我建议在进行本书中的练习时在 GitHub 上管理项目，并且我提供了有关如何使用这些工具的简短指南。Github 具有出色的版本控制，因此您可以看到所做的更改 犯错误或者只是想要一种更直接的方式来遵循。这也是稍后与其他人共享代码的好方法。


### Node and NPM

**Before we can begin, we'll need to have [Node and NPM](https://nodejs.org/en/) installed. Both are used to manage libraries (node packages) that you will need along the way. These node packages can be libraries or whole frameworks. We'll install external node packages via npm (node package manager).**
在开始之前，我们需要安装 [Node 和 NPM](https://nodejs.org/en/)。 两者都用于管理您在此过程中需要的库（节点包）。 这些节点包可以是库或整个框架。 我们将通过 npm（节点包管理器）安装外部节点包。

**You can verify node and npm versions on the command line using the `node --version` and `npm --version` commands. If you don't receive output in the terminal indicating which version is installed, you need to install node and npm:**
您可以使用“node --version”和“npm --version”命令在命令行上验证节点和 npm 版本。 如果您在终端中没有收到指示已安装哪个版本的输出，则需要安装 Node 和 npm：

```shell
node --version
*vXX.YY.ZZ
npm --version
*vXX.YY.ZZ
```

**If you have already installed Node and npm, make sure that your installation is the most recent version. If you're new to npm or need a refresher, this [npm crash course](https://www.robinwieruch.de/npm-crash-course/) I created will get you up to speed.**
如果您已经安装了 Node 和 npm，请确保您安装的是最新版本。 如果您是 npm 新手或需要复习，我创建的这个 [npm 速成课程](https://www.robinwieruch.de/npm-crash-course/) 将使您快速上手。


### Exercises:

- **Read more about [yarn](https://yarnpkg.com/) and [pnpm](https://pnpm.io/). Both can be used as replacement for npm. However, I do not recommend using them as a beginner. This exercise should only make sure that you know about your options.**
了解有关 [yarn](https://yarnpkg.com/) 和 [pnpm](https://pnpm.io/) 的更多信息。 两者都可以用作 npm 的替代品。 但是，我不建议初学者使用它们。 此练习仅应确保您了解自己的选择。

---
---

## Setup

###  Setting up a React Project

**In the Road to React, we'll use [Vite](https://bit.ly/3BsG1TH) to set up our React application. Vite, a french word which translates to "quick", is a modern build tool for status quo web frameworks (e.g. React) which comes with sensible defaults (read: configuration) while staying highly extensible for specific use cases (e.g. SVG support, Lint support, TypeScript) later on. The essential core of Vite is a development server, which allows you to start your React application on your local machine (read: development environment), and a bundler, which outputs highly optimized files for a production-ready deployment (read: production environment). What matters for a React beginner here: getting started with React by just learning React while not getting distracted by any tooling around it. Therefore Vite is the perfect partner for learning React.**
在 React 之路中，我们将使用 Vite 来设置 React 应用程序。 Vite 是一个法语单词，翻译为“快速”，是一种用于现状 Web 框架（例如 React）的现代构建工具，它具有合理的默认值（读：配置），同时保持稍后针对特定用例（例如 SVG 支持、Lint 支持、TypeScript）的高度可扩展性。 Vite 的基本核心是一个开发服务器，它允许您在本地计算机上启动 React 应用程序（阅读：开发环境），以及一个捆绑器，它输出高度优化的文件以进行生产就绪部署（阅读：生产环境）。 对于 React 初学者来说重要的是：通过学习 React 来开始使用 React，而不是被任何周围的工具分散注意力。 因此Vite是学习React的最佳伙伴。

**There are two ways to create your project with Vite. First, choosing an [online template](https://bit.ly/3RPAZWz), either React (recommended for this book) or React TypeScript (advanced, which means you implement the types for TypeScript yourself) for working on your project online without a local setup. Second, which is the way I would recommend, is creating a React project with Vite on your local machine for working on it in your local IDE/editor (e.g. VSCode).**
使用 Vite 创建项目有两种方法。 首先，选择一个在线模板，React（本书推荐）或 React TypeScript（高级，这意味着您自己实现 TypeScript 的类型），以便在线处理您的项目，而无需本地设置。 其次，我推荐的方法是在本地计算机上使用 Vite 创建一个 React 项目，以便在本地 IDE/编辑器（例如 VSCode）中处理它。

**Since the online template works out of the box, we will focus on the setup for your local machine in this section (recommended). In a previous section, you have installed Node and npm. The latter enables you to install third-party dependencies (read: libraries/frameworks/etc.) from the command line. So open up your command line tool and move to a folder where you want to create your React project. As a crash course for navigating on the command line:**
由于在线模板开箱即用，因此我们将在本节中重点关注本地计算机的设置（推荐）。 在上一节中，您已经安装了 Node 和 npm。 后者使您能够从命令行安装第三方依赖项（阅读：库/框架/等）。 因此，打开命令行工具并移动到要在其中创建 React 项目的文件夹。 作为在命令行上导航的速成课程：

- use `pwd` (Windows: `cd`) to display the current folder
- use `ls` (Windows: `dir`) to display all folders and files in the current folder
- use `mkdir <folder_name>` to create a folder
- use `cd <folder_name>` to move into a folder
- use `cd ..` to move outside of a folder

**After navigating into a folder where you want to create your React project, type the following command. We'll refer to this project as hacker-stories, but you may choose any project name you like:**
导航到要在其中创建 React 项目的文件夹后，键入以下命令。 我们将此项目称为 hacker-stories，但您可以选择您喜欢的任何项目名称：

```shell
npm create vite@latest hacker-stories -- --template react
```

**Optionally you can also go with a React + TypeScript project if you feel confident (check Vite's installation website to follow their instructions for a React + TypeScript project). The book comes with a TypeScript section later on, however, it will not do any hand-holding throughout the sections for transforming JavaScript into TypeScript. Next, follow the instructions given on the command line for navigating into the folder, installing all the third-party dependencies of the project, and running it locally on your machine:**
如果您有信心，您也可以选择使用 React + TypeScript 项目（查看 Vite 的安装网站以按照其关于 React + TypeScript 项目的说明进行操作）。 本书稍后附带了 TypeScript 部分，但是，它不会在整个部分中提供将 JavaScript 转换为 TypeScript 的任何指导。 接下来，按照命令行上给出的说明导航到该文件夹，安装项目的所有第三方依赖项，并在您的计算机上本地运行它：

```shell
cd hacker-stories
npm install
npm run dev
```

**The command line should output a URL where you can find your project running in the browser. Open up the browser with the given URL and verify that you can see the React project running there. We will continue developing this project in the next sections, however, for the rest of this section, we will go through explaining the project structure and the scripts (e.g. `npm run dev`).**
命令行应该输出一个 URL，您可以在其中找到在浏览器中运行的项目。 使用给定的 URL 打开浏览器并验证您是否可以看到正在运行的 React 项目。 我们将在接下来的部分中继续开发该项目，但是，在本节的其余部分中，我们将解释项目结构和脚本（例如 npm run dev）。

### Project Structure

**First, let's open the application in an editor/IDE. For VSCode, you can simply type `code .` on the command line. The following folder structure, or a variation of it depending on the Vite version, should be presented:**
首先，让我们在编辑器/IDE 中打开应用程序。 对于 VSCode，您只需键入 code 即可。 在命令行上。 应显示以下文件夹结构或根据 Vite 版本而变化的文件夹结构：

```shell
hacker-stories/
--node_modules/
--public/
----vite.svg
--src/
----assets/
------react.svg
----App.css
----App.jsx
----index.css
----main.jsx
--.gitignore
--index.html
--package-lock.json
--package.json
--vite.config.js
```

**This is a breakdown of the most important folders and files:**
这是最重要的文件夹和文件的细分：

- package.json: This file shows you a list of all third-party dependencies (read: node packages which are located in the node_modules/ folder) and other essential project configurations related to Node/npm.
- package-lock.json: This file indicates npm how to break down (read: resolve) all node package versions and their internal third-party dependencies. We'll not touch this file.
- node_modules/: This folder contains all node packages that have been installed. Since we used Vite to create our React application, there are various node modules (e.g. React) already installed for us. We'll not touch this folder.
- .gitignore: This file indicates all folders and files that shouldn't be added to your git repository when using git, as such files and folders should be located only on your local machine. The node_modules/ folder is one example. It is enough to share the package.json and package-lock.json files with other developers in the team, so they can install dependencies on their end with `npm install` without having to share the entire node_modules/ folder with everybody.
- vite.config.js: A file to configure Vite. If you open it, you should see Vite's React plugin showing up there. If you would be running Vite with another web framework, the other framework's Vite plugin would show up. In the end, there are many more things that can optionally be set up here.
- public/: This folder holds static assets for the project like a [favicon](https://bit.ly/3QvRupG) which is used for the browser tab's thumbnail when starting the development server or building the project for production.
- index.html: The HTML that is displayed in the browser when starting the project. If you open it, you shouldn't see much content though. However, you should see a script tag which links to your source folder where all the React code is located to output HTML/CSS in the browser.

● package.json：此文件显示所有第三方依赖项的列表（读取：位于node_modules/文件夹中的节点包）以及与Node/npm相关的其他基本项目配置。

● package-lock.json：该文件指示npm 如何分解（读：解析）所有节点包版本及其内部第三方依赖项。 我们不会碰这个文件。

● node_modules/：该文件夹包含所有已安装的节点包。 由于我们使用 Vite 创建 React 应用程序，因此已经为我们安装了各种节点模块（例如 React）。 我们不会碰这个文件夹。

● .gitignore：此文件指示使用git 时不应添加到git 存储库中的所有文件夹和文件，因为此类文件和文件夹应仅位于本地计算机上。 node_modules/ 文件夹就是一个例子。 与团队中的其他开发人员共享 package.json 和 package-lock.json 文件就足够了，因此他们可以使用 npm install 在自己的一端安装依赖项，而不必与每个人共享整个 node_modules/ 文件夹。

● vite.config.js：配置Vite的文件。 如果你打开它，你应该会看到 Vite 的 React 插件出现在那里。 如果您要与另一个 Web 框架一起运行 Vite，则会显示另一个框架的 Vite 插件。 最后，还有很多东西可以选择在这里设置。

● public/：此文件夹保存项目的静态资源，例如启动开发服务器或构建生产项目时用于浏览器选项卡缩略图的图标。

● index.html：启动项目时在浏览器中显示的HTML。 如果你打开它，你不应该看到太多内容。 但是，您应该看到一个脚本标记，它链接到所有 React 代码所在的源文件夹，以便在浏览器中输出 HTML/CSS。

**In the beginning, everything you need is located in the src/ folder. The main focus lies on the src/App.jsx file which is used to implement React components. It will be used to implement your application, but later you might want to split up your React components into multiple files, where each file maintains one or more components on its own. We will arrive at this point eventually.**
一开始，您需要的所有内容都位于 src/ 文件夹中。 主要焦点在于 src/App.jsx 文件，该文件用于实现 React 组件。 它将用于实现您的应用程序，但稍后您可能希望将 React 组件拆分为多个文件，其中每个文件都单独维护一个或多个组件。 我们最终会到达这一点。

**Additionally, you will find a src/main.jsx as an entry point to the React world. You will get to know this file intimately in later sections. There is also a src/index.css and a src/App.css file to style your overall application and components, which comes with the default style when you open them. You will modify them later as well.**
此外，您会发现 src/main.jsx 作为 React 世界的入口点。 您将在后面的部分中深入了解该文件。 还有一个 src/index.css 和 src/App.css 文件用于设置整个应用程序和组件的样式，当您打开它们时，它们带有默认样式。 您稍后也将修改它们。


### npm Scripts

**After you have learned about the folder and file structure of your React project, let's go through the available commands. All your project-specific commands can be found in your package.json file under the `scripts` property. They may look similar to these depending on your Vite version:**
了解 React 项目的文件夹和文件结构后，让我们浏览一下可用的命令。 所有特定于项目的命令都可以在 script 属性下的 package.json 文件中找到。 根据您的 Vite 版本，它们可能看起来与以下类似：

```json
{
  ...
  },
  "scripts": {
    "dev": "vite",
    "build": "vite build",
    "preview": "vite preview"
  },
  ...
}
```

**These scripts are executed with the `npm run <script>` command in an IDE-integrated terminal or your standalone command line tool. The commands are as follows:**
这些脚本是在 IDE 集成终端或独立命令行工具中使用 npm run `<script>` 命令执行的。 命令如下：

```shell
# Runs the application locally for the browser
npm run dev

# Builds the application for production
npm run build
```

**Another command from the previous npm scripts called `preview` can be used to run the production-ready build on your local machine for testing purposes. In order to make it work, you have to execute `npm run build` before running `npm run preview`. Essentially `npm run dev` and `npm run preview` (after `npm run build`) should give the identical output in the browser. However, the former is not optimized by a build for production and should exclusively be used for the local development of the application.**
先前 npm 脚本中的另一个命令（称为预览）可用于在本地计算机上运行生产就绪版本以进行测试。 为了使其工作，您必须在运行 npm run Preview 之前执行 npm run build。 本质上， npm run dev 和 npm run Preview （在 npm run build 之后）应该在浏览器中给出相同的输出。 但是，前者并未通过生产构建进行优化，并且应专门用于应用程序的本地开发。

### Exercises:

- Read more about [Vite](https://bit.ly/3BsG1TH).
- Exercise npm scripts:

- Start your React application with `npm run dev` on the command line and check it out in the browser.

- Exit the command on the command line by pressing `Control + C`.

- Run the `npm run build` script and verify that a dist/ folder was added to your project. Note that the build folder can be used later on to [deploy your application](https://www.robinwieruch.de/deploy-applications-digital-ocean/). Afterward, run `npm run preview` to see the production-ready application in the browser.

- Every time we change something in our source code throughout the coming sections, make sure to check the output in your browser for getting visual feedback. Use `npm run dev` to keep your application running.
- Optional: If you use git and GitHub, add and commit your changes after every section of the book.
- Optional: [Leave feedback for this section](https://forms.gle/bvH2jcppsSA6p9i16).

● 了解更多有关Vite 的信息。

● 练习npm 脚本：

○ 在命令行上使用 npm run dev 启动 React 应用程序，然后在浏览器中查看它。

■ 按 Control + C 退出命令行上的命令。

○ 运行 npm run build 脚本并验证 dist/ 文件夹是否已添加到您的项目中。 请注意，稍后可以使用构建文件夹来部署您的应用程序。 然后，运行 npm run Preview 以在浏览器中查看生产就绪的应用程序。

● 在接下来的部分中，每当我们更改源代码中的某些内容时，请务必检查浏览器中的输出以获得视觉反馈。 使用 npm run dev 来保持应用程序运行。

● 可选：如果您使用git 和GitHub，请在本书的每个部分之后添加并提交更改。

● 可选：留下对此部分的反馈。

---
---

## Meet the React Component

**Every React application is built on the foundation of React components. In this section, you will get to know your first React component which is located in the src/App.jsx file and which should look similar to the example below. Depending on your Vite version, the content of the file might differ slightly:**
每个 React 应用程序都构建在 React 组件的基础上。 在本节中，您将了解您的第一个 React 组件，该组件位于 src/App.jsx 文件中，并且应该类似于下面的示例。 根据您的 Vite 版本，文件内容可能略有不同：

```jsx
import { useState } from 'react';
import reactLogo from './assets/react.svg';
import './App.css';

function App() {
  const [count, setCount] = useState(0);

  return (
    <div className="App">
      <div>
        <a href="https://vitejs.dev" target="_blank">
          <img src="/vite.svg" className="logo" alt="Vite logo" />
        </a>
        <a href="https://reactjs.org" target="_blank">
          <img
            src={reactLogo}
            className="logo react"
            alt="React logo"
          />
        </a>
      </div>
      <h1>Vite + React</h1>
      <div className="card">
        <button onClick={() => setCount((count) => count + 1)}>
          count is {count}
        </button>
        <p>
          Edit <code>src/App.jsx</code> and save to test HMR
        </p>
      </div>
      <p className="read-the-docs">
        Click on the Vite and React logos to learn more
      </p>
    </div>
  );
}

export default App;
```

**This file will be our focus throughout this book, unless otherwise specified. Even though this file will grow in size, because we are not splitting it up from the beginning into multiple files, it will be simpler to understand as a beginner, because everything is at one place. Once you get more comfortable with React, I will show you how to split your React project into multiple files.**
除非另有说明，该文件将是本书的重点。 尽管这个文件的大小会增加，但因为我们没有从一开始就把它分成多个文件，所以作为初学者会更容易理解，因为一切都在一个地方。 一旦您对 React 更加熟悉，我将向您展示如何将 React 项目拆分为多个文件。

**Let's start by reducing the component to a more lightweight version for getting you started without too much distracting [boilerplate code](https://bit.ly/3lZzckS):**
让我们首先将组件减少为更轻量级的版本，以便在没有太多分散注意力的样板代码的情况下开始:

```jsx
# leanpub-start-insert
import * as React from 'react';

function App() {
  return (
    <div>
      <h1>Hello React</h1>
    </div>
  );
}

export default App;
# leanpub-end-insert
```

**Optionally you can also make the src/index.css and src/App.css files blank for starting from a clean slate style-wise.**
或者，您还可以将 src/index.css 和 src/App.css 文件设为空白，以便从干净的样式开始。

**Next, start your application with `npm run dev` on the command line and check what's displayed in the browser. You should see the headline "Hello React" showing up. Before we dive deeper into each topic, here comes a quick overview of what's in your code and what we will cover more in-depth in the following sections:**
接下来，在命令行上使用 npm run dev 启动应用程序并检查浏览器中显示的内容。 您应该会看到标题“Hello React”出现。 在我们深入研究每个主题之前，先快速概述一下您的代码中的内容以及我们将在以下部分中更深入介绍的内容：

- First, this React component, specifically called App component, is just a JavaScript function. In contrast to traditional JavaScript functions, it's defined in [PascalCase](https://www.robinwieruch.de/javascript-naming-conventions/). A component has to start with a capital letter, otherwise it isn't treated as component in React. The kind of the App component is commonly called a function component. Function components are the modern way of using components in React, however, be aware that there are other variations of React components (see component types in a later section) too.
- Second, the App component doesn't have any parameters in its function signature yet. In the upcoming sections, you will learn how to pass information (see props in a later section) from one component to another component. These props will be accessible via the function's signature as parameters then.
- And third, the App component returns code that resembles HTML. You will see how this new syntax (see JSX in a later section), allows you to combine JavaScript and HTML for displaying highly dynamic and interactive content in a browser.

● 首先，这个React 组件，具体称为App 组件，只是一个JavaScript 函数。 与传统的 JavaScript 函数相比，它是用 PascalCase 定义的。 组件必须以大写字母开头，否则在 React 中它不会被视为组件。 App组件的种类通常称为功能组件。 函数组件是在 React 中使用组件的现代方式，但是，请注意 React 组件还有其他变体（请参阅后面部分中的组件类型）。

● 其次，App 组件的函数签名中还没有任何参数。 在接下来的部分中，您将学习如何将信息（请参阅后面部分中的 props）从一个组件传递到另一个组件。 然后可以通过函数的签名作为参数来访问这些道具。

● 第三，App 组件返回类似于HTML 的代码。 您将看到这种新语法（请参阅后面部分中的 JSX）如何允许您组合 JavaScript 和 HTML，以便在浏览器中显示高度动态和交互式的内容。

**Like any other JavaScript function, a function component can have implementation details between the function signature and the return statement. You will see this in practice in action throughout your React journey:**
与任何其他 JavaScript 函数一样，函数组件可以在函数签名和返回语句之间包含实现细节。 在整个 React 之旅中，您将在实践中看到这一点：

```jsx
import * as React from 'react';

function App() {
# leanpub-start-insert
  // you can do something in between
# leanpub-end-insert

  return (
    <div>
      <h1>Hello React</h1>
    </div>
  );
}

export default App;
```

**Variables defined in the function's body will be re-defined each time this function runs, which shouldn't be something new if you are familiar with JavaScript and its functions:**
每次该函数运行时，函数体内定义的变量都会被重新定义，如果您熟悉 JavaScript 及其函数，这应该不是什么新鲜事：

```jsx
import * as React from 'react';

function App() {
# leanpub-start-insert
  const title = 'React';
# leanpub-end-insert

  return (
    <div>
      <h1>Hello React</h1>
    </div>
  );
}

export default App;
```

**The function of a component runs every time a component is displayed in the browser. This happens for the initial rendering (read: displaying) of the component, but also whenever the component updates because it has to display something different due to changes (re-rendering). We will learn more about this later too.**
每次在浏览器中显示组件时，组件的功能都会运行。 这种情况发生在组件的初始渲染（读取：显示）时，而且每当组件更新时也会发生，因为它必须因更改而显示不同的内容（重新渲染）。 稍后我们也会了解更多相关信息。

**Since we do not want to re-define a variable within a function every time this function runs, we could define this variable outside of the component as well. In this case, the `title` does not depend on any information that's within the function component (e.g. parameters coming from the function's signature), hence it's okay to move it outside. Therefore it will be defined only once and not every time the function is called:**
由于我们不想每次运行函数时都在函数内重新定义变量，因此我们也可以在组件外部定义该变量。 在这种情况下，标题不依赖于函数组件内的任何信息（例如来自函数签名的参数），因此可以将其移到外部。 因此它只会被定义一次，而不是每次调用该函数时:

```jsx
import * as React from 'react';

# leanpub-start-insert
const title = 'React';
# leanpub-end-insert

function App() {
  return (
    <div>
      <h1>Hello React</h1>
    </div>
  );
}

export default App;
```

**On your journey as a React developer, and in this learning experience, you will come across both scenarios: variables (and functions) defined outside and within a component. As a rule of thumb: If a variable does not need anything from within the function component's body (e.g. parameters), then define it outside of the component which avoids re-defining it on every function call.**
在作为 React 开发人员的旅程中，以及在这次学习经历中，您将遇到两种场景：在组件外部和内部定义的变量（和函数）。 根据经验：如果变量不需要函数组件体内的任何内容（例如参数），则在组件外部定义它，这样可以避免在每次函数调用时重新定义它。

### Exercises:

- Compare your source code against the author's [source code](https://bit.ly/3UvoTEn).

- Optional: If you are using TypeScript, check out the author's source code [here](https://bit.ly/3RhDTm8).

- Think about ways to display the `title` variable in your App component's returned HTML. In the next section, we'll put this variable to use.
- Optional: [Leave feedback for this section](https://forms.gle/VYiZqqjzXGE11wCv6).

● 将您的源代码与作者的源代码进行比较。

○ 可选：如果您使用 TypeScript，请在此处查看作者的源代码。

● 考虑如何在应用程序组件返回的HTML 中显示标题变量。 在下一节中，我们将使用这个变量。

● 可选：留下对此部分的反馈。