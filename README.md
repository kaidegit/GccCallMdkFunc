本工程旨在测试使用gcc调用keil生成的函数，用于解决某些函数库仅有keil版本的问题

# 纯算法测试

algo文件夹中，MDK工程中主要包含了一个algo函数，使用__USED修饰强制编入HEX中，可以在MAP文件中找到该函数的地址。GCC工程中ld文件中指定这个algo函数的地址，并在程序中添加该函数的声明即可调用。

需要注意的是，MDK工程与GCC工程的Flash和Ram人为设置为了互不重叠，下载前使用`mergehex`（nrf的工具）合并hex。

# 中断测试

TODO

# RTOS测试

TODO