# comm

> 对比两个有序文件来获取或删除共有内容（通过选项控制，进行交、并、差等运算达成目的）

- 形成三个用 TAB 划分的列：第一列的每一行仅在第一个文件中出现，第二列的每一行仅在第二个文件中出现，第三个列的每一行是两个文件共有的：

`comm {{file1}} {{file2}}`

- 只输出两个文件共有的行：

`comm -12 {{file1}} {{file2}}`

- 只输出两个文件共有的行，其中一个文件从标准输入 (stdin) 读入：

`cat {{file1}} | comm -12 - {{file2}}`

- 取得仅出现于第一个文件的行，并将它保存到第三个文件中：

`comm -23 {{file1}} {{file2}} > {{file1_only}}`

- 对于没有排序的两个文件，输出仅存在于第二个文件的行：

`comm -13 <(sort {{file1}}) <(sort {{file2}})`

[#]: contributors: ([󠀀]，[毕玮])