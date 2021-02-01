# 数据类型

在 *JavaScript* 中有哪些数据类型？

<details>
<summary><b>解答</b></summary>

### 解答

截止到目前（2021年01月27日）为止，*JavaScript* 中的数据类型有： `undefined`, `null`, `number`, `string`, `boolean`, `symbol`, `bigint`, `object`, `function`。

你可能会疑惑数据类型里为什么会有 `null`，因为 `typeof null === 'object'`；`null` 是一个比较特殊的基本类型，它表示一个空值。

你可能曾在MDN的中文版看过[JavaScript 数据类型和数据结构](https://developer.mozilla.org/zh-cn/docs/web/javascript/data_structures)，这里面并没有提到 `function` 类型；可事实是 `function` 确实是单独的一种类型。
你可以试着把上述地址中的语言切换到英文版，或者直接打开[JavaScript data types and data structures](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures)，你就会发现，英文版中其实是有提到 `function` 类型的；另外，想一下，在你想判断一个数据是不是函数时，是怎么判断的？`typeof fn === 'function'`，看 `typeof` 操作符本身就告诉你有这么一个类型了。

</details>
