#  安装 HarukaBot
  
  
##  方法一 脚手架安装 (推荐)
  
  
1. 安装 [Python3.7+](https://www.python.org/downloads/release/python-386/ ) (推荐 `3.8.6` 安装的时候一定要[**勾选 "Add Python 3.x to PATH"**](https://www.liaoxuefeng.com/wiki/1016959663602400/1016959856222624 ) )
  
2. 打开一个文件夹 (建议新建), 对着空白处按住 Shift 单击鼠标右键, 选择 "在此处打开 Powershell 窗口"
  
3. 输入 `pip install haruka-bot[cli]` 安装脚手架
  
4. 输入 `hb run` 启动 bot
  
> 以后只需在**相同文件夹**内执行最后一步即可启动
  
  
##  方法二 手动安装 (可获取实验性功能)
  
  
1. 安装 [Python3.7+](https://www.python.org/downloads/release/python-386/ ) (推荐 `3.8.6` 安装的时候一定要[**勾选 "Add Python 3.x to PATH"**](https://www.liaoxuefeng.com/wiki/1016959663602400/1016959856222624 ) )
  
2. 克隆 or [下载](https://github.com/SK-415/HarukaBot/releases/latest ) HarukaBot 源码到本地
  
3. 在源码根目录打开命令提示符 (对着文件夹内, 按住 shift 同时鼠标右键 -> 在此处打开 Powershell 窗口)
  
3. 输入 `pip install -r requirements.txt` 安装依赖
  
4. 输入 `python bot.py` 启动 HarukaBot
  
> 以后每次启动只需重复 3, 5 两步
  
##  方法三 插件广场安装 (适用于 `NoneBot2` 用户)
  
  
- 使用[插件广场](https://v2.nonebot.dev/plugin-store.html )或者 `pip install haruka-bot`, 安装 `HarukaBot`
  
- 如果使用 pip 下载的还需要手动在 `bot.py` 中添加 `nonebot.load_plugin("haruka_bot")`
  
- (可选) 在 `.env.prod` 或 `.env.dev` 中添加 `HARUKA_DIR="./data/"`, 你也可以将 `./data/` 改成任何其他路径. 
  > 如果不添加, HarukaBot 会将配置文件保存于其安装包位置 (site-packages/haruka_bot) 的 `data` 文件夹中, 之后迁移会很麻烦, 并不推荐.
  
- 完成后重启 `NoneBot2` 实例即可使用