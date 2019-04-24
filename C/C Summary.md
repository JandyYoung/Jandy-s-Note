# 关键字

| 关键字 | 作用                                                         |
| ------ | ------------------------------------------------------------ |
| auto   | 当前变量的作用域为当前函数或代码段的局部变量，当前变量在内存栈中分配。(编译器默认缺省情况下所有变量都是auto) |
| register | 将变量尽可能存在CPU内部寄存器，但不一定能够存在CPU寄存器，访问速度很快。可以将频繁操作的变量放入寄存器中，且不能通过&进行取地址操作，变量长度要小于寄存器长度。|
| static |修饰变量，修饰全局变量，其作用域为该变量定义的文件中；修饰局部变量则该变量不会因为函数的结束而结束；修饰的变量都存储在内存的静态区。修饰函数则表明该函数为静态函数，只能在函数定义所在的文件调用。|
| char | 字符串数据类型，32位机中1字节大小 |
| short | 短整型数据类型，32位机中2字节大小 |
| int | 整型数据类型，32位机中4字节大小 |
| long | 长整型数据类型，32位机中4字节大小 |
| float | 单精度型浮点数，32位机中4字节大小 |
| double | 双精度型浮点数，32位机中4字节大小 |
| sizeof | 获取数据在内存中占用的存储空间(单位：字节)，计算变量时可以省略括号，计算类型时不可以省略 |
| signed | 声明的整型变量为有符号类型，最高位为1表示负数，最高位为0表示正数，但是其本质还是大于0的数 |
| unsigned | 声明的整型变量为无符号类型 |
| if | 条件语句 |
| else | if配套语句 |
|  |  |

## 1. 声明和定义的区别

定义：创建一个对象，向这个对象分配一块内存并取变量名或者对象名。

声明：告诉编译器，该变量已经与内存绑定或者即将绑定。

> 变量名与内存地址绑定，且变量不能重复定义；声明可以使用很多次；定义分配内存，声明不分配内存。
