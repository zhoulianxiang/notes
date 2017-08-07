# 桌面系统

## 连接
通常有两种方式使用桌面系统
- vnc
- hdmi连接显示器，usb键鼠，直连

### vnc

使用比较普遍的tightvnc。vnc会在图形表现上有些限制，一般的使用是足够了

### 直连

hdmi接口，如果需要声音，记得将`/boot/config.txt`中的`hdmi_drive=2`设置一下

## 表现

足够使用。
- 日常事务处理
- 上网
- 音乐/视频
- 一般的游戏

### 亮点

- 一个中规中矩的桌面系统，近乎傻瓜
- minecraft pi，免费的
  - 当然比不上正版的游戏，但是配合python可以有另一种玩法
  - https://www.raspberrypi.org/learning/getting-started-with-minecraft-pi/
- mathematica
  - 一代计算神器，如果需要，就赚到了
- 各种编程ide
  - scratch，可以在这里直接操练了
  - 各种python ide，在python封神的今天，很有价值

### 实用性

- 特种用途，如果说retro游戏模拟器也算桌面系统的一种的话
- 没有计算机的时候的好选择，比如回老家带上键鼠和hdmi线
- “洁癖”的好选择，总是能用到“自己”的私人定制
- 就我目前日常使用的概率很小
  - 找个闲置的hdmi显示设备不容易
  - 我更习惯命令行模式
  - 我不缺计算机
- 我日常还是会关闭所有的桌面系统程序，ssh上去，活在tmux里
