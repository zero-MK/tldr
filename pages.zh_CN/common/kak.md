# kak

> Kakoune 是一个基于模式的代码编辑器，实现了“多重选择”范式
> 数据可以在不同的位置选择和同时编辑，使用多个选择;用户还可以连接到同一个会话进行协作编辑

- 打开一个文件并进入正常模式，执行命令：

`kak {{path/to/file}}`

- 从正常模式进入插入模式，将文本写入文件：

`i`

- 退出插入模式并返回初始状态：

`<Escape>`

- 用 bar 替换当前文件中 foo 的所有实例：

`%s{{foo}}<Enter>c{{bar}}<Escape>`

- 取消选择所有辅助选择，并仅保留主要选择：

`<Space>`

- 搜索数字并选择前两个数字：

`/\d+<Enter>N`

- 插入文件的内容：

`!cat {{path/to/file}}<Enter>`

- 保存当前文件：

`:w<Enter>`

[#]: contributors: ([潘潘]，[千柏]，[Stubborn])