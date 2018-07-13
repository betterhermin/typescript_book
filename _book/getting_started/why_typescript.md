## 为什么使用TypeScript
* TypeScript有两个主要目标：
> * 为JavaScript提供可选的类型系统。
> * 提供从未来JavaScript版本到当前JavaScript引擎的计划功能
## TypeScript 类型系统
* 您可能想知道“为什么要向JavaScript添加类型？”
* 已证明类型能够提高代码质量和可理解性。 大型团队（谷歌，微软，Facebook）不断得出这个结论。 特别：
> * 在进行重构时，类型可以提高您的敏捷性。 编译器捕获错误比在运行时失败更好。
> * 类型是您可以拥有的最佳文档形式之一。 函数签名是一个定理，函数体是证明。
* 然而，类型有一种不必要的隆重的方式。 TypeScript非常讲究保持入门门槛尽可能低。
## 你的JavaScript就是TypeScript
* TypeScript为JavaScript代码提供编译时类型安全性。 鉴于它的名字，这并不奇怪。 最棒的是这些类型是完全可选的。 您的JavaScript代码.js文件可以重命名为.ts文件，TypeScript仍然会返回与原始JavaScript文件等效的有效.js文件。
* TypeScript是有意且严格地具有可选的类型检查的一个JavaScript超集
## 类型可以是隐式的
* TypeScript将尝试尽可能地推断出类型信息，以便在代码开发过程中以最小的生产成本为您提供类型安全性。 例如，在下面的示例中，TypeScript将知道foo的类型 number，并将在第二行显示错误，如下所示：
<pre>
var foo = 123;
foo = '456'; // Error: cannot assign `string` to `number`

// Is foo a number or a string?
</pre>
* 他的类型推理是积极的。 如果您执行此示例中显示的内容，则在其余代码中，您无法确定foo是 number 还是 string。 这些问题经常出现在大型多文件代码库中。 我们稍后将深入探讨类型推断规则。
## 类型可以是显式的
* 正如我们之前提到的，TypeScript会尽可能安全地推断，但是您可以使用注释：
帮助编译器，更重要的是为下一个必须阅读代码的开发人员记录内容（可能是未来的你！）。

