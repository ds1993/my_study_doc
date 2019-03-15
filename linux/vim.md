## 查找:

	#查找str
	:/str
## 撤销操作

	:u
## 替换
(`/`转义为`\/`)

	:s/vivian/sky/ 替换当前行第一个 vivian 为 sky
	:%s/vivian/sky/(等同于: g/vivian/s//sky/) 替换每一行的第一个vivian为sky
	:%s/vivian/sky/g(等同于: g/vivian/s//sky/g) 替换每一行中所有vivian为sky
## 插入

	%s/^/str 在每行行首插入字符串str
	%s/$/str 在每行行尾插入字符串str