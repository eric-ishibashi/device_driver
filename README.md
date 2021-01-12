## device_driver
デバイスドライバ

## 内容
上田教授が授業で作成したデバイスドライバ(https://github.com/ryuichiueda/robosys_device_drivers/blob/master/myled.c )を少し変え、「マリオカート」のスタート音のタイミングと同時に光らせました。

## 動作環境
OS:Ubuntu 18.04

## 使用器具
・Raspberry Pi4 1個<br>
・ブレットボート（EIC-801）1個<br>
・赤色LED(10mm) 5個<br>
・ジャンパーワイヤ（オスメス）10cm 10本<br>
・炭素被膜抵抗　330Ω　1/4W　5個<br>

## インストール
```
$ git clone https://github.com/eric-ishibashi/device_driver.git]
```

## 動作方法
```
make
```
↓
```
sudo rmmmod myled.ko
```
↓
```
sudo chmod 666/dev/myled0
```
↓
```
echo 0>/dev/myled0
```
## 製作者
19C1007 石橋英陸

## 動画
https://youtu.be/mt3DpGMseac

## ライセンス
[GNU General Public Licence v3.0](https://github.com/kiyoshirou-kawanabe/Robosys_Devicedriver/blob/main/COPYING)

