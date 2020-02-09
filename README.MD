# fsr-cli

使用 aardio 编写的命令行程序, 用来调用 `FastStone Capture` 中的 `FSRecorder.exe` 来进行视频录制.


## 使用步骤:
- 设置: 运行命令 `fsr-cli` , 在 UI 界面进行好所需设置, 因为程序只负责开始和结束录制.
- 录制: 运行命令 `fsr-cli action=start` , 将会自动进行以下操作.
  - 点击 `录制屏幕 > 重复上次区域 > 录制 > 开始`
- 停止: 运行命令 `fsr-cli action=stop out=file` , 将会自动进行以下操作.
  - 点击 `停止 > 输入文件名 file > 保存`


``` bat
fsr-cli :: 以UI方式启动视频录制器, 并进行好所需设
fsr-cli action=start :: 开始录制视频
fsr-cli action=stop out=file :: 停止录制视频, 并保存文件名为 file
```
