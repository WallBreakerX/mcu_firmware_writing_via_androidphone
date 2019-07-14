# 单片机固件烧录器

## 注意事项
  
  - 当前暂只支持 **NXP的LPC8xx系单片机**，后续会添加STM32的支持，最终希望实现大部分Cortex-M系的单片机烧录。
  
  - 选择Flash时需与实际Flash大小对应(默认为16KB)，否则有可能造成Flash的擦除和写入失败。
  
  - 连接RTS与DTS引脚是为了让APP控制引脚电平使芯片进入ISP模式，也可自己手动进入ISP。

## 硬件需求与连接

  - 安卓6.0手机及以上
  
  - OTG转接线
  
  - CH340 USB to TTL
  
  - 你想要烧录的单片机
  
  - 将CH340的USB端转接至手机USB口
  
    TTL端的**TX 连接至 PIO0_0， RX 连接至 PIO0_4**
  
    **RTS 连接至 RESET，DTS 连接至 PIO0_12**
    
    (大部分CH340没有引出RTS和DTS针脚，但留有孔位，需要自行焊接)
    
    VCC和GND连接好即可
  
## 使用步骤

  - 选择hex文件
  
  - 选择单片机片内Flash大小
  
  - 开始烧录！
  
  

  
  
  
### 联系方式

    WeChat: xmh849873336
    
    Email: a84987336@outlook.com
    
    
    
### 感谢以下开源库

- https://github.com/felHR85/UsbSerial

- https://github.com/leonHua/LFilePicker

- https://blog.csdn.net/zf_c_cqupt/article/details/52676716 CSDN
