##### 一、Code给出了一个参考示例
单周期CPU，支持8条指令
-	add/sub/and/or
-	lw,sw
-	beq
-	ori
##### 二、第一个实验需要完成单周期处理器
-	~~add/sub/and/or~~ 
-	~~lw/sw~~
-	~~beq~~
-	~~jalr/jal~~
-	~~ori/xor/xori/andi/addi~~
-	~~sll/sra/srl/slt/sltu/srai/slti/sltiu/slli/srli/lui/auipc~~
-	~~lb/lh/lbu/lhu/sb/sh (数据在内存中以小端形式存储little endian)~~
-	~~bne/blt/bge/bltu/bgeu/~~

**注意：** 可以在示例代码基础上扩展完成，也可以自行设计代码结构。

##### 模块介绍
EXT 立即数生成
NPC 生成PC
PC 程序计数器
Alu 运算器
RF 寄存器
Ctrl 控制器
Ctrl_encode_def 操作码宏定义
Im 指令存储器
Dm 数据存储器
SCPU 不包含存储器的通路

##### git使用指南

给不会用 git 的小萌新们的简单使用指南

1. git clone 把代码下载到本地
2. git add . 添加所有文件
3. git commit -m "修改说明" 提交修改，修改说明的格式见 gitlint
4. git push 推送到远程仓库

_建议单独增加新功能时，新建一个 branch，完成后 merge 到主分支_

2024-07-04 根据 FPGA 封装调整了接口