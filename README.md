﻿# appium
##appium基础学习工程  
1.appium-Java环境配置（新建工程添加java-client依赖)<br>
2.设置机型设置属性<br>
3.设置被测应用包名及启动activity：使用命令`aapt dump badging` <包路径>可以查看  
4.实例化session  
5.可以开始编写UI测试脚本啦  
6.本工程中定位方法类实现了'byXPath','byAndroidUIAutomator','byClassName'三种定位元素方式，详见代码；且用另一个app实现了HybridApp的测试实践；MobileWebApp的测试实践也已添加
tips:  
1.如果不想每执行一个test都重装一次应用这样设置即可
```
capa.setCapability("noReset",true);	
```
2.隐式等待绝对是需要的:
```
driver.manage().timeouts().implicitlyWait(60, TimeUnit.SECONDS);
