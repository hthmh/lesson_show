[source](https://juejin.im/post/5b561426518825195f499772)



提前接收部分参数，延迟执行， 不立即输出结果， 而是返回一个接受剩余参数的函数，逐步接受参数的过程。

  - 传入参数， 代码不立即执行， 而是先记忆起来
  - 传入空的参数时， 真正运算

add(1)(2, 3)(4)() = 10
记忆

