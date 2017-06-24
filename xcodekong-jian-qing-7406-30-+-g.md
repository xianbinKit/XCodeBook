# XCode 磁盘清理

##### 移除对旧设备的支持  ---  文件巨大，可恢复，支持删除不需要的

路径：~/Library/Developer/Xcode/iOS DeviceSupport

 第一次将新手机，或者刚升级的手机连接xcode时，都会等待同步信息很长时间，就是在生成支持文件，可删除，每次链接的时候重新生成。



##### 移除旧版本的模拟器支持

路径：~/Library/Application Support/iPhone Simulator

影响：不可恢复；如果需要旧版本的模拟器，就需要重新下载了。我移除了4.3.2, 5.0, 5.1等旧版本的模拟器。



##### 移除模拟器中安装的Apps

路径：~/Library/Application Support/iPhone Simulator/6.1/Applications \(以iOS Simulator 6.1为例\)



##### 移除DerivedData

路径：~/Library/Developer/Xcode/DerivedData

影响：可重新生成；会删除build生成的项目索引、build输出以及日志。重新打开项目时会重新生成，大的项目会耗费一些时间。

  


