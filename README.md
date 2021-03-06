# PHP7内核剖析

(更新中...)

文中涉及代码版本：php-7.0.12

* 第1章 PHP基本架构
   * 1.1 基本概念(1/base_introduction.md)
   * [1.2 PHP框架执行流程](1/base_process.md)
* 第2章 变量
   * [2.1 变量的内部实现](2/zval.md)
   * 2.2 数组(2/zend_ht.md)
   * 2.3 常量(2/var_common.md)
* 第3章 Zend虚拟机
   * [3.1 PHP代码的编译](3/zend_compile.md)
      * [3.1.1 词法解析、语法解析](3/zend_compile_parse.md)
      * [3.1.2 抽象语法树编译流程](3/zend_compile_opcode.md)
   * [3.2 函数实现](3/function_implement.md)
      * [3.2.1 内部函数](3/function_implement.md)
      * <a href="3/function_implement.md#用户自定义函数的实现">3.2.2 用户函数的实现</a>
   * [3.3 Zend引擎执行流程](3/zend_executor.md)
      * <a href="3/zend_executor.md#331-数据结构">3.3.1 基本结构</a>
      * <a href="3/zend_executor.md#332-执行流程">3.3.2 执行流程</a>
      * <a href="3/zend_executor.md#333-函数的执行流程">3.3.3 函数的执行流程</a>
   * 3.4 面向对象实现
      * [3.4.1 类](3/zend_class.md)
      * 3.4.2 对象(3/zend_object.md)
      * 3.4.3 继承
      * 3.4.4 魔术方法
      * 3.4.5 抽象类和接口
   * 3.5 运行时缓存(3/zend_runtime_cache.md)
* [第4章 PHP语法实现](4/php_language.md)
   * 4.1 变量
   * 4.2 运算符
   * 4.3 选择结构
   * 4.4 循环结构
   * 4.5 跳转语句
   * 4.6 函数
* 第5章 内存管理
   * [5.1 Zend内存池](5/zend_alloc.md)
   * 5.2 垃圾回收(gc.md)
* 第6章 扩展开发
