# SENZ002 模拟压电陶瓷震动传感器

###### 翻译

> `英文`请参考 [`这里`](https://github.com/FizzyStudio/SENZ002_Analog-Piezo-Disk-Vibration-Sensor/blob/master/README.md).

> `中文`请参考 [`这里`](https://github.com/FizzyStudio/SENZ002_Analog-Piezo-Disk-Vibration-Sensor/blob/master/README_CN.md).

![](https://github.com/FizzyStudio/SENZ002_Analog-Piezo-Disk-Vibration-Sensor/blob/master/pic/SENZ002.jpg "SENZ002") 

### 简介

> 基于压电陶瓷片的模拟震动传感器，是利用压电陶瓷给电信号产生震动的反变换过程，当压电陶瓷片震动时就会产生电信号，与Arduino专用传感器扩展板结合使用，Arduino模拟口能感知微弱的震动电信号，可实现与震动有相关的互动作品，比如电子鼓互动作品。

### 产品参数

* 电压：无需供电
* 接口类型：模拟
* 电流：小于1mA
* 引脚定义：1--地 2--输出 3---空脚
* 重量：10g

### 引脚图

![](https://github.com/FizzyStudio/SENZ002_Analog-Piezo-Disk-Vibration-Sensor/blob/master/pic/SENZ002_2.png "引脚图") 

### 使用教程

#### 连接图

![](https://github.com/FizzyStudio/SENZ002_Analog-Piezo-Disk-Vibration-Sensor/blob/master/pic/SENZ002_3.png "连接图") 

#### 示例代码

    //Arduino Sample code
    void setup()
    {
      Serial.begin(9600); //
    }
    void loop()
    {
          int val;
          val=analogRead(0);//Connect the sensor to analog pin 0
          Serial.println(val,DEC);//
          delay(100);
    }

> 注意:代码编译上传完之后，打开串口监视器，在串口监视器的右下角选择跟您程序中设置一致的波特率。


### 结果

> 不对压电陶瓷片施加压力时，输出的模拟量为0；当对压电陶瓷片施加压力，输出模拟量会发送变化，而且随着压力增大而增大。

![](https://github.com/FizzyStudio/SENZ002_Analog-Piezo-Disk-Vibration-Sensor/blob/master/pic/SENZ002_4.png "结果") 

### 更多




