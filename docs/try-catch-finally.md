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
