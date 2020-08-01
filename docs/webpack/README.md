# webpack 是什么？

<font  size=4>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;回答这个问题之前，大家可以回想一下自己最开始接触前端时，是如何搭建前端项目的？我相信绝大多数人的前端项目跟下图类似。一个 html 页面，在页面中引入所需要的的样式和 js 资源。</font>

<div align=center>
	<img src="./base/images/1.png" width="">
</div>

<font  size=4>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;随着前端技术的飞速发展，js 有了 es5,es6,es7 等诸多新标准,css 也有了 less，sass 等更简洁的语法标准。运用这些新特性使前端代码更容易书写和阅读，同时随着 nodejs 的诞生，react，vue 等优秀的前端框架也大大加快了前端的开发速度。但是一些老版本的浏览器对这些新技术的支持却没有那么好，甚至根本不认识.vue、.jsx 等文件。这就导致了一个问题要怎样才能让前端开发人员即能使用最新的前端技术，又能让这些通过最新技术开发的项目在绝大多数浏览器上运行呢？</font>

<font  size=4>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;这就需要通过某个工具将开发人员使用新技术写的代码，翻译成市场上绝大多数浏览器都认识的代码，并对翻译后的代码进行压缩，分块，优化等操作，而 webpack 就是这些工具中功能最强且使用最广泛的那个。</font>

[官网资料](https://webpack.docschina.org/concepts/)
