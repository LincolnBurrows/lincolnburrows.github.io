## VisionSensorClient Update Log
### 更新0614
1. 新增数据包

```
shotIndex = 100  杆数索引
```
###### 说明:根据shotIndex可以在LPGData_right文件夹下找到此次击球的挥杆图像(保存在以100命名的文件夹内)

```
errCode = 1       can not find sensor

errCode = 4001    sensor authorized failed

errCode = 4002    get sensor ID failed

errCode = 4003    can not find right sensor
```
###### 说明：启动VisionSensorClient.exe自身会进行校验，以上数据在校验失败情况下发送（上位机可根据情况提供UI提示），同时VisionSensorClient.exe会自动关闭

2. VisionSensorClient.exe取消发送重复数据
3. 降低CPU占用率
4. 尽快推送更新，之前版本存在日志过大的问题
