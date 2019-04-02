## 命令行参数

	$0 脚本名
	$1 第一个参数
	$2 第二个参数
	...
	$# 参数个数
	$* 以一个单字符串显示所有参数
	$$ 脚本运行的进程号
	$@ 参数数组
## 数字大小比较

	-gt 大于
	-lt 小于
	-eq 等于
	-ne 不等于
	-ge 大于等于
	-le 小于等于
## 字符串替换

	${parameter//pattern/string}

	例:
	string="hello,shell,split,test"
	array=(${string//,/ })
## 版本管理

	update-alternatives --install <链接> <名称> <路径> <优先级>: 注册
	update-alternatives --config <名称>: 选择
## 软链接创建

	ln -s [源文件或目录] [目标文件或目录]
## 判断文件是否存在

	if [ -f "/data/filename" ];then
	echo "文件存在"
	else
	echo "文件不存在"
	fi