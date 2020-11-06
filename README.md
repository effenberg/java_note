# java_note
**1.一个".java"源文件中是否可以包括多个类（不是内部类）？有什么限制？**
答：可以。但最多只有一个类名声明为public，与文件名相同。

**2.超纲题目：GC是什么? 为什么要有GC****
答：GC是垃圾收集的意思（Gabage Collection）,内存处理是编程人员容易出现问题的地方，
忘记或者错误的内存回收会导致程序或系统的不稳定甚至崩溃，Java提供的GC功能可以自动监测对象是否超过作用域从而达到自动回收内存的目的，Java语言没有提供释放已分配内存的显示操作方法。

**3.超纲题目：垃圾回收器的基本原理是什么？垃圾回收器可以马上回收内存吗？有什么办法主动通知虚拟机进行垃圾回收**
答：对于GC来说，当程序员创建对象时，GC就开始监控这个对象的地址、大小以及使用情况。通常，GC采用有向图的方式记录和管理堆(heap)中的所有对象。通过这种方式确定哪些对象是"可达的"，哪些对象是"不可达的"。
当GC确定一些对象为"不可达"时，GC就有责任回收这些内存空间。可以。程序员可以手动执行System.gc()，通知GC运行，但是Java语言规范并不保证GC一定会执行。

## Java 中的名称命名规范 ##：
**包名**：多单词组成时所有字母都小写 xxxyyyzzz
**类名、接口名** ：多单词组成时，所有单词的首字母大写 XxxYyyZzz
**变量名、方法名** ：多单词组成时，第一个单词首字母小写，第二个单词开始每个单词首字母大写： xxxYyyZzz
**常量名** ：所有字母都大写。多单词时每个单词用下划线连接 XXX_YYY_ZZZ

d
