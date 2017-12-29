# amlogic<br>
## 本周任务<br>
`修复以下bug`<br>

* 1在DVB中，按MENU，Exit退出DVB后，再次进入DVB出现黑屏。按OK（或上下键）进入节目才正常播放 <br>
* 2进入timeshift后，停止键为播放暂停作用 <br>
* 3进入二级菜单后，如果要返回一次菜单，只能按UP键，如果按EXIT就直接退出菜单了，建议参考普通的DVB-T2机器，菜单操作一定要人性化 <br>
* 4Recall list建议默认值为5 <br>
* 5Information Show Time建议默认值为3秒 <br>

## 20171225

* 1、按menu键正常播放节目（OK）:smile:

* 2、info键（OK）:mask:

* 3、recall list 默认为1符合用户习惯 :sunglasses:

* 4、释放Mstar俄罗斯&迪拜参展样机软件T10A、T10B、T10F、T10G（OK）:innocent:


## 20171226<br>

* 1、DTV遥控器完善优化 <br>
* 2、DTV UI 优化 <br>
* 3、timeshift下，stop（OK） <br>
* 4、information show time 默认为3s （OK） <br>

## 20171227<br>

* 1、Mstar 7T01 IPTV支持.m3u8格式播放<br>
* 2、Option 中增加Antenna Power（ON/OFF），默认OFF(OK) <br>
* 3、主菜单中back键二级菜单返回一级菜单再返回主菜单（由Sky完成）（OK） <br>

## 20171228 <br>

* 1、释放新版本软件给测试部测试，送样给客户升级（IR更新，需要提醒业务）

* 2、Mstar Divisat添加遥控器新的遥控器  

* 3、更新安卓UI（dialog） 

## 20171229任务 <br>
1、 修复测试部反馈的bug  
`我的调试机器tuner有问题，poweroff显示0.18v，实际是5v；poweron显示0.31v，实际是0v`  
2、 了解git<br>
3、 DTVRecordDevice.java和DTVDeviceBrowser.java经常恢复到R23之前的版本，只能rm然后update，但是第二天或者某一天又恢复到了R23之前的版本  
