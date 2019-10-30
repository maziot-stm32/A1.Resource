## 文件列表

- schematic.pdf
  最新系统板原理图
- STM32CubeIDEv1.0.xml
  STM32CubeIDE配置文件备份

## STM32CubeIDE配置习惯

待补充

## 工程建立标准流程

设计到的开发工具有：

- STM32CubeIDE
- GitHub Desktop
- Git

建议的创建工程流程：

1. STM32CubeIDE创建工程，可视化界面配置好后不修改任何代码
2. GitHub Desktop 创建同名仓库，默认会将自动生成的代码做第一笔提交记录提交
3. 删除工程中的 .setting 配置文件，添加 .gitignore 忽略规则，进行第二笔提交
4. 在 GitHub 上创建同名仓库，使用 Git 客户端绑定本地仓库和远程仓库
5. 修改代码，并通过 GitHub Desktop 进行管理以及和 GitHub 网站通信

备注：第4步为什么要 Git 客户端介入呢，是因为我的远程仓库不是在我的个人账户下的，是在组织账户下的。直接使用 GitHub Desktop 没有权限创建组织账户下的仓库，因此只能手动创建组织下的仓库，并手动进行绑定。

## 工程建立顺序

1. f103rc.msb.gpio.led
2. f103rc.msb.gpio.key
3. f103rc.msb.exti.key
4. f103rc.msb.uart.log