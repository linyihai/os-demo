# 进度
## 进度 10
1. 完成rustlings项目的clippy，collections，conversions，enums
2. 在本地机器搭建了基于wsl2的开发环境，目前完成了文档的第一章的阅读并将其完成放在os目录下了。

## 进度 20
1. 完成rustlings: https://github.com/linyihai/os_rustlings
2. 完成test3: https://github.com/LearningOS/lab1-os3-linyihai


## 进度 100
终于把lab1-5 全部完成了.

rustling:  https://github.com/linyihai/os_rustlings (原来的仓库删掉了，自己fork了一个)
lab1: https://github.com/LearningOS/lab1-os3-linyihai
lab2: https://github.com/LearningOS/lab2-os4-linyihai
lab3: https://github.com/LearningOS/lab3-os5-linyihai
lab4: https://github.com/LearningOS/lab4-os6-linyihai
lab5: https://github.com/LearningOS/lab5-os8-linyihai


# 笔记

## 第一章

可以通过rustc --target指定编译平台，也可以通过`rustup target add riscv64gc-unknown-none-elf` 下载安装编辑

`rust-objdump -S target/riscv64gc-unknown-none-elf/debug/os` 反向导出汇编程序

用到了core::arch::asm!这个汇编宏的话，需要安装nightly的rust版本

`rustup default nightly`
`rustup update`
`rustup target add riscv64gc-unknown-none-elf`

# 寄存器
`RISC-V 寄存器编号从 0~31 ，表示为 x0~x31 。 其中： - x10~x17 : 对应 a0~a7 - x1 ：对应 ra`

# 问题

os4: PhysPageNum.get_pte_arrray, 不太明白物理页码怎么得到页表项

# TODO
1. lab4 
第六章: 文件系统与I/O重定向; 这章内容挺多，而且把文件系统从磁盘到操作系统内部抽象了好多层，后面有时间再仔细捋一捋各个模块之间的关系

