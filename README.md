第一步，先实现让机器人指哪里走哪里

![](C:\Users\james\Desktop\TP\images\2024-04-10-05-04-46-image.png)

主体部分: 高97.5mm

宽 ：350mm

长：520mm

+ 电机驱动 解决
  
  ## 贝塞尔曲线
  
  三层约束  路径  速度 加速度
  
  x 方向 y 方向 都有约束
  
  之后能解出这个，![](C:\Users\james\Desktop\TP\images\2024-04-17-17-24-42-image.png)
  
  S 为步长
  
  H 为步高

+ 运动学解算 

+ 步态

+ 在32上实现机器狗的脉冲产生器 注意，现在用的那个板子上的晶振是8MHZ的

+ 注意把脉冲发生器的起始位置修改成竖直站立状态，便于每次的切换。
  
  大概是改成这样：
  
  ![](C:\Users\james\Desktop\TP\images\2024-04-29-10-30-43-image.png)
  
  在 3/8处，这样的脉冲能确保每次产生的时候接入你站立的姿态

+ 

+ ![](C:\Users\james\Desktop\TP\images\2024-04-29-10-34-38-image.png)

我们实际扔给贝塞尔曲线计算的脉冲是这样

当然，相关的转换处理已经写在了matlab函数中