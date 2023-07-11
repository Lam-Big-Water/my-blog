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