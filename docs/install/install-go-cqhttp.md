# 安装 go-cqhttp

1. 下载 [`go-cqhttp`](https://github.com/Mrs4s/go-cqhttp/releases/latest ) (Windows 用户选择 `windows-amd64.zip` 结尾).
  
2. 解压至一个空文件夹后, 双击启动, 此时文件夹内会生成一个 `config.json` 文件, 打开并编辑. 
以下折叠部分为参考 (中文部分记得替换): 
  
	</br>
  
	<details>
	<summary>config.json 设置参考</summary>
  
	```json
	{
		"uin": 机器人QQ号,
		"password": "QQ密码",
		"encrypt_password": false,
		"password_encrypted": "",
		"enable_db": true,
		"access_token": "",
		"relogin": {
			"enabled": true,
			"relogin_delay": 3,
			"max_relogin_times": 0
		},
		"_rate_limit": {
			"enabled": false,
			"frequency": 1,
			"bucket_size": 1
		},
		"ignore_invalid_cqcode": false,
		"force_fragmented": false,
		"heartbeat_interval": 0,
		"http_config": {
			"enabled": false,
			"host": "0.0.0.0",
			"port": 5700,
			"timeout": 0,
			"post_urls": {}
		},
		"ws_config": {
			"enabled": false,
			"host": "0.0.0.0",
			"port": 6700
		},
		"ws_reverse_servers": [
			{
				"enabled": true,
				"reverse_url": "ws://127.0.0.1:8080/cqhttp/ws",
				"reverse_api_url": "",
				"reverse_event_url": "",
				"reverse_reconnect_interval": 3000
			}
		],
		"post_message_format": "string",
		"debug": false,
		"log_level": "",
		"web_ui": {
			"enabled": false,
			"host": "127.0.0.1",
			"web_ui_port": 9999,
			"web_input": false
		}
	}
	```
	</details>
  
</br>
  
3. 编辑完重启 `go-cqhttp.exe`, 跟着提示完成安全验证即可