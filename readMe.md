# 简介
 * 在Android 开发中，可能需要添加多语言的翻译，添加的翻译文件strings.xml中，可能存在遗漏或错误格式化字符串的问题，某些错误会导致APP Crash，而这种错误是难以人工排查的，固此工具可以帮助开发人员检测String.xml文件中的格式化错误，以避免发布后才发现crash的问题。
## 新任务 
 * 提取出英文中有百分号的所有字符串的key；
 * 然后把其他语言中对应key的字符串执行format操作，看看是否出错。
 * 对比提取出英文中的带百分号的字符串，看看其他语言中对应key的格式化内容和英文中的是否一致。（非常重要，因为其他语言可能漏掉对应的格式化内容，导致在代码里面执行format，找不到格式化内容，而出现崩溃。）
 * 提取出英文中的%1$s有几个，确保其他语言是一致的。
## 打包
 * 导出.Jar包
## 待改进
 * 添加图形界面版本