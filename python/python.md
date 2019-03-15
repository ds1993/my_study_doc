## 获取文件绝对路径

	os.path.abspath(file)
## 循环遍历

	list = ["fuck1", "fuck2", "fuck3"]

	#方法1
	for value in list:
		print "key: %d, value: %s" % (list.index(value) + 1, value)

	#方法2
	for key in range(len(list)):
		print "key: %d, value: %s" % (key, list[key])

	#方法3
	for key, value in enumerate(list):
		print "key: %d, value: %s" % (key, value)
## 正则匹配替换

	re.sub(pattern, repl, string, count=0, flags=0)
`pattern`: 表示正则表达式中的模式字符串  
`repl`: 被替换的字符串(既可以是字符串，也可以是函数)  
`string`: 要被处理的,要被替换的字符串  
`count`: 匹配的次数,默认是全部替换
## 正则匹配

	re.match(pattern, string, flags=0): 尝试从字符串的起始位置匹配一个模式,如果不是起始位置匹配成功的话,match()就返回none
	re.search(pattern, string, flags=0): 扫描整个字符串并返回第一个成功的匹配