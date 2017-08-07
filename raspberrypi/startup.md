## 买树莓派

- 买最新最贵的就好了
- 散热片、盒子也要
- 屏幕、键鼠一般不需要
- 没有其他的了

## 买卡

- 大小
  - 专用8GB即可，比如安装游戏模拟器retropi，主要是更小的现在不好买了
  - 通用16GB即可，
  - 如有特殊用途，可考虑更大
- 品牌，大牌子都可以
- 类型，class10

## 发行版

- https://www.raspberrypi.org/downloads/raspbian/
  - 按照我目前的习惯，对desktop的需求很小，更喜欢“RASPBIAN JESSIE LITE”
  - 出于通用性考虑，及初级阶段，我选择了“RASPBIAN JESSIE WITH DESKTOP”
- https://retropie.org.uk/
  - 考虑到T卡的价格，追求方便、稳定的使用，单独弄张卡做个模拟器系统是个不错的选择
- 目前我还没有其他感兴趣的版本

## img写入

- windows：Win32DiskImager
- linux/unix/mac：dd
- backup
  - `dd if=/dev/sdX | gzip > img.gz`
  - `gzip -dc img.gz | dd of=/dev/sdX`

## 启动之前

- 通过uart终端登录
  - 修改config.txt，在末尾添加`enable_uart=1`
  - 通过usb to ttl工具，连接gpio口
    - 将gpio脚放在左下方位，竖着放
    - 左下，由下向上，345脚分别是GND/TXD/RXD
- 通过显示器登录
  - 连接上hdmi接口的显示器、usb键盘、鼠标即可

## 登录

- pi/raspberry

## 网络

- wifi
  - /etc/wpa_supplicant/wpa_supplicant.conf
  - https://wiki.archlinux.org/index.php/WPA_supplicant
```
network={
        ssid="..."
        psk="..."
}
````

## 打开ssh

- sudo raspi-config
  - 5 Interfacing Options -> P2 SSH -> YES
- 如果总是在ssh下工作，可以考虑修改默认登录方式到`B1 Console`

## 默认登录方式

- sudo raspi-config
  - 3 Boot Options -> B1 Desktop / CLI -> ...

## 习惯设定

- adduser
- `.bashrc`
- 更新vim，`.vimrc`
- tmux，`.tmux.conf`
- others...

## 进入专项设定

就看这个树莓派是买回来干啥的了
