## TypeScript 入门
* TypeScript会编译成JavaScript，JavaScript是你要实际执行（在浏览器或服务器上）的代码，所以你需要这些：
* TypeScript编译器（OSS在源代码和NPM上可用）
* 一个TypeScript编辑器（推荐vscode）
## TypeScript 版本
* 我们将在本书中介绍许多可能与版本号无关的新内容，而不是使用稳定的TypeScript编译器。 我通常建议人们使用最新版本（每日更新），不然编译器测试套件可能随着时间的推移捕获很多的错误。
您可以在命令行上安装它
<pre>
npm install -g typescript@next
</pre>
* 现在命令行tsc是最新的和最好的。各种IDE也支持它，例如
* 您可以通过使用以下内容创建.vscode / settings.json来要求vscode使用此版本：
<pre>
{
  "typescript.tsdk": "./node_modules/typescript/lib"
}
</pre>
## 获取源码
* 本书的源代码可以在书籍github存储库https://github.com/basarat/typescript-book/tree/master/code中找到，大多数代码示例都可以复制到vscode中，你可以按原样使用它们。 对于需要额外设置的代码示例（例如npm模块），我们会在呈现代码之前将您链接到代码示例。 例如:
<pre>
this/will/be/the/link/to/the/code.ts
// This will be the code under discussion
</pre>
* 通过开发设置，让我们跳转到TypeScript语法。