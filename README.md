# 7815测试时打开usb驱动及装入软件的方法：
## 1、首先连接主板lvds1到电阻屏上，再连接usb口接上主板mio1位置插好鼠标，最后给主板接入12v电源；
### 2、开机进入“设置”然后用鼠标滑动到设置中的“开发者模式”项，进入后滑动到底部系统版本栏点击五次，会看到有提示“已经进入开发者模式”；
#### 3、退到上一步找到“usb debuging”项，打开后可以选择界面常亮；
##### 4、将OTG线连接电脑和主板的OTG接口，会在电脑上显示安装驱动成功，按住键盘“win+R”，在该界面输入“adb devices”可见主板的驱动信息（为一串数字）；
###### 5、输入“adb install 空格键后键入apk的位置”，点击enter向主板系统装入软件，当装成功后会显示“successful”，然后就可以开始在主板上检查软件了。
# 7815安装过程要点：
## 1、有时连接异常可能是数据线问题，要更换；
### 2、无法显示驱动信息可能是上述第二步未正确打开，或者主板异常，可重试和更换好的主板；
#### 3、数据线连接后失败可以尝试按照电脑上提示更新驱动或者重启电脑
##### 4、电脑提前需要安装adb命令，如果想使用其他方式可以选择sd卡装入，方法是从第四步开始将要装的软件存入sd卡后插入主板卡槽在文件管理其中找到并安装；
thanks for reading ！
