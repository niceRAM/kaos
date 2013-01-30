kaos - 谷歌拼音输入法颜文字扩展
==============================

在输入一些特定的拼音字母时，候选会显示表情文字
比如 'ai', 会显示 '╮(╯_╰)╭' 在最后一个候选项中
  
文件:
-----
*   dict.txt 
    固有格式存储的颜文字词库

*   generator.py
    python3 写的从词库文件转为谷歌输入法扩展的转换器

*   kaos.lua
    输入法扩展

更新:
-----
*	2013-01-30	2.1.1 
	词库微小修正

*	2013-01-30	2.1.0 beta 测试版
	修改词库词定义方式，去掉了可选的释义项，分隔符现在可以是TAB也
	可以是4个以上的空格。融合了旧版词库。

*	2013-01-27	2.0.0 beta 测试版
	新的字库, 新的框架, 支持字符缩写映射, 采用 python3 重写转换器
	目前词库是新组的词库, 旧词库暂时未整合, 下一版本将整合词库

安装方法:
--------
在谷歌拼音输入法 属性设置 > 扩展 > 安装扩展包 > 选择 kaos.lua
然后重启输入法即可 (即关闭输入法再打开，两次按 Ctrl+Space)

已知问题:
---------
1.	候选的表情总是在候选列表最后，这是谷歌输入法本身的设置所致
2.	某些拼音字母对应多个表情，但是目前谷歌输入法只能显示一个,
    这里采用随机方法来显示多个表情中的一个
  

