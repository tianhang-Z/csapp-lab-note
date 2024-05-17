共9个实验

- *Data Lab*

- 对应第二章 信息的表示和处理

  涉及整型 浮点数的表示和运算 

  重点是理解补码 补码的范围 补码的加法 用补码加法表示做减法运算   利用~计算相反数 

  理解算数移位和逻辑移位   对整型做逻辑运算！（非） 

  除法正数向下取整   和负数向上取整  （舍弃小数部分）  利用移位及加减运算实现乘除法

  不使用减法 实现整数的大小比较

   浮点数的表示

  > Students implement simple logical, two's complement, and floating point functions, but using a highly restricted subset of C. For example, they might be asked to compute the absolute value of a number using only bit-level operations and straightline code. This lab helps students understand the bit-level representations of C data types and the bit-level behavior of the operations on data.

- *Bomb Lab*

  学习汇编  数据访问（寻址方式 出入栈） 算数和逻辑运算 控制（条件码 跳转 循环 switch[跳转表]） 程序运行时（栈帧 转移控制 参数的传递 局部变量的存储）  数组的分配和访问（指针运算） 数据结构（struct union 数据对齐）  

  GDB调试

  > A "binary bomb" is a program provided to students as an object code file. When run, it prompts the user to type in 6 different strings. If any of these is incorrect, the bomb "explodes," printing an error message and logging the event on a grading server. Students must "defuse" their own unique bomb by disassembling and reverse engineering the program to determine what the 6 strings should be. The lab teaches students to understand assembly language, and also forces them to learn how to use a debugger. It's also great fun. A legendary lab among the CMU undergrads.
  >
  > Here's a [Linux/x86-64 binary bomb](http://csapp.cs.cmu.edu/3e/bomb.tar) that you can try out for yourself. The feature that notifies the grading server has been disabled, so feel free to explode this bomb with impunity. If you're an instructor with a CS:APP account, then you can download the [solution](http://csapp.cs.cmu.edu/im/bomb-solution.txt).

- *Attack Lab*

  缓存区溢出 对抗缓存区溢出（栈随机化 栈破坏检测）

  学习CI和ROP代码攻击

  > Note: This is the 64-bit successor to the 32-bit Buffer Lab.
  >
  > Students are given a pair of unique custom-generated x86-64 binary executables, called targets, that have buffer overflow bugs. One target is vulnerable to code injection attacks. The other is vulnerable to return-oriented programming attacks. Students are asked to modify the behavior of the targets by developing exploits based on either code injection or return-oriented programming. This lab teaches the students about the stack discipline and teaches them about the danger of writing code that is vulnerable to buffer overflow attacks.
  >
  > If you're a self-study student, here are a pair of [Ubuntu 12.4 targets](http://csapp.cs.cmu.edu/3e/target1.tar) that you can try out for yourself. You'll need to run your targets using the **"-q"** option so that they don't try to contact a non-existent grading server. If you're an instructor with a CS:APP acount, you can download the solutions [here](https://csapp.cs.cmu.edu/im/labs/target1-sol.tar).

- *Buffer Lab (IA32)*   被attack lab代替了

  > *Note: This is the legacy 32-bit lab from CS:APP2e. It has been replaced by the Attack Lab.*
  >
  >  In the Buffer Lab, students modify the run-time behavior of a 32-bit x86 binary executable by exploiting a buffer overflow bug. This lab teaches the students about the stack discipline and teaches them about the danger of writing code that is vulnerable to buffer overflow attacks.

- *Architecture Lab*

  > Note: Updated to Y86-64 for CS:APP3e.
  >
  > Students are given a small default Y86-64 array copying function and a working pipelined Y86-64 processor design that runs the copy function in some nominal number of clock cycles per array element (CPE). The students attempt to minimize the CPE by modifying both the function and the processor design. This gives the students a deep appreciation for the interactions between hardware and software.
  >
  > Note: The lab materials include the master source distribution of the Y86-64 processor simulators and the *Y86-64 Guide to Simulators*.

- Architecture Lab (Y86)

- 被代替了

  > Note: Legacy Y86 version for CS:APP2e.
  >
  > Students are given a small default Y86 array copying function and a working pipelined Y86 processor design that runs the copy function in some nominal number of clock cycles per array element (CPE). The students attempt to minimize the CPE by modifying both the function and the processor design. This gives the students a deep appreciation for the interactions between hardware and software.
  >
  > Note: The lab materials include the master source distribution of the Y86 processor simulators and the *Y86 Guide to Simulators*.

- *Cache Lab*

  > At CMU we use this lab in place of the Performance Lab. Students write a general-purpose cache simulator, and then optimize a small matrix transpose kernel to minimize the number of misses on a simulated cache. This lab uses the Valgrind tool to generate address traces.
  >
  > Note: This lab must be run on a 64-bit x86-64 system.

- *Performance Lab*

  > Students optimize the performance of an application kernel function such as convolution or matrix transposition. This lab provides a clear demonstration of the properties of cache memories and gives them experience with low-level program optimization.

- *Shell Lab*

  > Students implement their own simple Unix shell program with job control, including the ctrl-c and ctrl-z keystrokes, fg, bg, and jobs commands. This is the students' first introduction to application level concurrency, and gives them a clear idea of Unix process control, signals, and signal handling.

- *Malloc Lab*

  Students implement their own versions of malloc, free, and realloc. This lab gives students a clear understanding of data layout and organization, and requires them to evaluate different trade-offs between space and time efficiency. One of our favorite labs. When students finish this one, they really understand pointers!

- *Proxy Lab*

  > Students implement a concurrent caching Web proxy that sits between their browser and the rest of the World Wide Web. This lab exposes students to the interesting world of network programming, and ties together many of the concepts from the course, such as byte ordering, caching, process control, signals, signal handling, file I/O, concurrency, and synchronization.