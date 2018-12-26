---
layout:     post
title:      Learn command line
subtitle:   Note when learning command line
date:       2018-12-24
author:     hanlian
header-img: img/post-bg-2015.jpg
catalog: true
tags:
---

- pwd		= printing working directory
- ls		= lists  
	-a		包含以.开头的（隐藏文件夹+本及目录+上级目录）  
	-A		包含隐藏文件夹  
	-l		长格式  
	-t		修改时间   
	-alt		包含.开头、长格式、修改时间  
- cd		= change directory					cd ../../..    上三级
- mkdir	= make directory  
- touch		创建新文件  
- cp		= copy  
	file to directory  
	files to directory  
	file to file  
	*		wildcard		全部文件  
	m*		全部以m开头的文件  
	m*.txt	全部以m开头的txt文件  
- mv		= move  
	file to directory  
	files to directory  
	rename a file  
- rm		= remove  
	-r		recursive    删除所有子文件（夹）  
	*		当前目录所有文件  

- echo	接受输入的内容  
	echo "Hello"			显示文字  
	echo "Hello">hello.txt	to a file  
- cat		= concatenate			输出内容  
	cat hello.txt > test.txt		用hello.txt的内容覆盖test.txt  
	cat hello.txt >> test.txt	保留hello.txt中的内容  
	cat < hello.txt			从hello.txt中输出  
- wc		= word count		显示新行数、单词数、字节数、文件名  
	行数、字数、字节数或字符数。  
- sort		input  ---alphabetically--->  output  
- uniq		= unique			删除重复项  
- grep		= global regular expression print	(case sensitive)	grep Arctic oceans.txt  
	-i	(case insensitive)	grep -i Arctic oceans.txt  
	-R	= recursive	在目录中查找，显示文件名和符合的行的内容  
	-Rl	只显示文件名  
- sed		= stream editor	input  ---根据表达式修改--->  output  
	's/snow/rain/'  ------  'substitution/search/replacement/'		只替换每一行第一个  
	's/snow/rain/g'      g=global		全部替换  

- 符号
	>	command standard output  ---rewrite--->  file  
	>>	command standard output  ---add--->  file  
	<	program <--- file standard input  
	|	command standard output  ---standard input--->  command  

- 缩写
	stdin		standard input  
	stdou		standard output  
	stderr		standard error  
	txt			textfile  