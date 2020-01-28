# STM32F103 资源与配置

本仓库收集与 STM32F103 开发的相关资源，以备忘的形式供开发者参考。

## [1. 控制电路板配置](environment/boards.md)

## [2. 仿真器配置](environment/emulator.md)

## [3. CAN 总线配置](environment/CAN.md)

## 如何同时将仓库同步到 gitee 和 github

下述操作具有风险, 最好先备份 .git/ 文件夹

1. VS 安装 gitee 及 github 的 extension<br>
如果不通过界面 clone gitee 的远程仓库，可以不安装 gitee extension
2. Team Explorer 中 Setting => Repository Settings 中在 Remote 下
点击 Add, 增加 github 及 gitee 远程仓库, 注意 Fetch 和 Push 可以不同
3. 若要将当前 commit 提交到 github 或 gitee, 则需要将上一步中的相应 Remotes 设置
为 origin。
4. 使用 VS 提交 commit, 也可以直接在 powershell 中 git push
5. backup.bat 是将当前的 .git/备份到 backups 文件夹中, 备份文件夹
名称为当前日期和时间。
注意 .gitignore 中加上了 backups/ , 该文件夹不会被推送到远程。
**随着时间的推移 backups 文件夹中的备份会越来越多，需要手工清除！**

