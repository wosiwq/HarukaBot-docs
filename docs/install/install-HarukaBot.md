#  安装 HarukaBot

::: warning 前提条件
HarukaBot 依赖于 [Python3.7+](https://www.python.org/downloads/release/python-386/)，不会安装的参考[廖雪峰的教程](https://www.liaoxuefeng.com/wiki/1016959663602400/1016959856222624)。  
下面内容将默认你已经安装了 Python 。
:::

##  方法一 脚手架安装（推荐)

打开终端，选择一个文件夹用来存放数据

::: tip Windows 用户可以这么做
打开一个文件夹，对着文件夹内空白处，按住 shift 同时单击鼠标右键 -> 在此处打开 Powershell 窗口。
:::

安装脚手架
```sh
pip install haruka-bot[cli]
```

启动 HarukaBot
```sh
hb run
```

> 以后启动只需在**相同文件夹**内执行最后一步即可

##  方法二 手动安装（包含尚未发布的功能)

克隆 HarukaBot 源码到本地

安装依赖
```sh
pip install -r requirements.txt
```

启动 HarukaBot
```sh
python bot.py
```

##  方法三 插件广场安装（适用于 `NoneBot2` 用户)

使用 `nb-cli` 命令从[插件广场](https://v2.nonebot.dev/plugin-store.html)安装

```sh
nb plugin install haruka_bot
```

（可选）在 bot 根目录的 `.env.*` 文件中，添加 `HARUKA_DIR="./data/"` 设置 HarukaBot 数据文件的存储路径。你也可以将 `./data/` 改成任何其他路径。

  > 如果不添加，HarukaBot 会将配置文件保存于其安装包位置（site-packages/haruka_bot）的 `data` 文件夹中，之后迁移会很麻烦，且不同 bot 之间将共享数据，非常不推荐。

安装完成后重启 `NoneBot2 实例` 即可使用