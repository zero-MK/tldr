# finger

> 用户信息查找程序

- 显示关于当前用户的信息：

`finger`

- 显示指定用户的信息：

`finger {{username}}`

- 显示用户的登录名，真实名，终端名，以及写状态：

`finger -s`

- 产生一个多行显示来描述 信息-s 关于用户家目录，家庭电话，登录脚本，邮件状态以及文件的内容：

`finger -l`

- 防止用户名user的匹配，user通常是登录名，可也会对用户的真实名字进行匹配，添加-m以阻止这样的匹配：

`finger -m`

[#]: contributors: ([霁])