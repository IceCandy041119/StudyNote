状态：
- Running 
	- ANSI Color: green
- Break
	- ANSI Color: Yellow
- Stop
	- ANSI Color: Red


功能：
- TRACE：
	- MTRACE
	- FTRACE
	- DTRACE
	- ITRACE
- 监视点：
	- Command: w \<express\>  
	- Function: 添加一个监视点
- 打印表达式：
	- Command：p \<express\>
	- Function: 打印表达式的值
- 信息：
	- Command：info \<option>
	- Function: 查看相应选项信息
- 运行：
	- Command: c
	- Function: 运行程序
- 执行多步：
	- Command： si  \<n\>
	- Function: 执行多步信息

日志：
- MTRACE
- DTRACE
- INSTRUCTION


视图

| 状态：     | 当前指令  | 地址    | 访存信息（last) |
| ------- | ----- | ----- | ---------- |
| 寄存器值    | 其他显示区 | 其他显示区 | 其他显示区      |
| CPU信息流  | 其他显示区 | 其他显示区 | 其他显示区      |
| COMMAND | 其他显示区 | 其他显示区 | 其他显示区      |
