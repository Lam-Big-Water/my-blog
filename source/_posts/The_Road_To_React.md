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