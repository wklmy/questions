# try/catch/finally的运行情况

问题：以下代码会输出什么？返回值是多少？

```js
function tcf() {
  try {
    console.log('尝试做些事情');
    return 1;
  } catch (e) {
    console.log('啊哦，出错了');
    return 2;
  } finally {
    console.log('最终结果总会来的');
    return 3;
  }
}
tcf();
```

<details><summary><b>答案解析</b></summary>
<p>

### 答案解析

> 结果是按顺序输出 `尝试做些事情`, `最终结果总会来的`；并最终返回 `3`。

1. *catch* 块仅在 *try* 出现错误时才会被执行。
2. *finally* 无论 *try* 是否有错误，都会被执行。
3. 为了保证 *finally* 一定会被执行，在 *try* 中的 *return* 语句会被延迟到 *finally* 执行完毕后再执行。
4. 在 *finally* 中也有 *return* 语句，所以 *try* 中被延迟执行的 *return* 语句不会再被触发了。

</p>
</details>
