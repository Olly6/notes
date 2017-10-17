## java并发机制的底层实现原理
### volatile的应用
在多线程并发编程中synchronized和volatile都扮演着重要的角色，volatile是轻量级的synchronized，它在多处理器开发中保证了共享变量的“可见性”。

可见性的意思是当一个线程修改一个共享变量时，另外一个线程能读到这个修改的值。**如果volatile变量修饰符使用恰当的话，它比synchronized的使用和执行成本更低，因为它不会引起线程上下文的切换和调度**。