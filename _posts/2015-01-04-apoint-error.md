---
layout: post
title: set user settings to driver failed (Apoint)
image: /img/hello_world.jpeg
---

Removing Apoint

run cmd.exe with administrator rights

``` cmd
net stop ApHidMonitorService
sc delete ApHidMonitorService

taskkill /f /im ApMsgFwd.exe
taskkill /f /im Apoint.exe
taskkill /f /im HidMonitorSvc.exe
```
Becarefull with the next command be sure to only delete the stated directory
the below command should work but is not tested!!!

```
rd /s /q "C:\Program files\Apoint2K"
```
