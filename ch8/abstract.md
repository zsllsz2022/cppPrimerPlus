1. 使用const引用能使函数能够正确生成并使用临时变量
2. 引用必须在声明的时候初始化 -> 变量的别名 / 类似于const指针
3. C++11新增右值引用 double&& right_ref = 6; 新增rvalue reference的主要目地是，让库设计人员能够提供有些操作更有效的实现。？？？？？
4. 最终的代码不包含任何模板，而只是包含了为程序生成的实际函数。使用模板的好处是，它使生成多个函数定义更简单、更可靠。更常见的情形是。将模板放在头文件里，并在需要使用模板的文件中包含头文件。
5. 内联函数必须放在头文件里！！！
6. 如果在头文件中定义非inline函数，一旦该头文件被多个文件包含，就会造成该非inline函数的“重定义”，因而，不建议将非inline函数的定义放在头文件中，但是非inline函数的声明是可以放在头文件中的。
7. 非函数模板 > 具体化 > 常规模板 
8. 实例化的是对象，而具体化的是模板（类似于声明）。 但我实在没搞动这俩东西。。。。