
<img width="4080" height="3072" alt="IMG_20260415_190105" src="https://github.com/user-attachments/assets/0a699f15-d600-4fb1-aa4c-1fab6e5362fc" />

<img width="3072" height="4080" alt="IMG_20260427_205225" src="https://github.com/user-attachments/assets/c93a2d13-76cc-4ce5-8bfe-c4a5724ef392" />

<img width="2080" height="1744" alt="IMG_20260514_201348" src="https://github.com/user-attachments/assets/3b5250b0-c900-48e5-9745-c4095de1a22e" />

# DC-AC
<img width="774" height="723" alt="image" src="https://github.com/user-attachments/assets/ae028e66-c785-4416-8425-fb7d58989df8" />

<img width="729" height="659" alt="image" src="https://github.com/user-attachments/assets/50b0b49d-1530-4a04-8b52-d5ad1df14132" />

<img width="514" height="223" alt="image" src="https://github.com/user-attachments/assets/9b0b93d8-3f79-48e7-95ea-66fa8551f11e" />
12V电源输入，经过电容滤波和MP4560DN-LF-Z芯片开关电压输出降压为5V在经过L1电感储能和滤波电容输出，D4肖特基二极管为防止芯片开启时电感反向输出时破坏电路，反向回复电流，芯片关闭时电感反向经过电流，L1电感能防止电流突变 进行储能 
芯片选型MP4560DN-LF-Z 散热好，成本低，输出电流适中，输出电压稳定

5V电容滤波后经过CJT1117B-3.3再经过高低滤波电容输出3.3V
选型CJT1117B-3.3是成本较低，散热要求不高，精度满足

<img width="490" height="178" alt="image" src="https://github.com/user-attachments/assets/bd213e86-83ef-4b20-9c67-b20bea842383" />

MCU主控
<img width="216" height="277" alt="image" src="https://github.com/user-attachments/assets/10861346-7615-4819-ae6a-66a55a2f0559" />

STM32模块 输出PWM和SD  接受电压和电流数据输出到OLED显示屏

<img width="244" height="327" alt="image" src="https://github.com/user-attachments/assets/6291a273-a2e4-4a26-b983-102bf2923a08" />

STM32输出高低电平到DCOUT，通过DCOUT高低电平控制Q3三极管的导通，导通时5V输入，LED灯亮，线圈带电使2和5连接，输出低BE电压小于发射极开启电压，Q3断开，灯灭，线圈不带电

<img width="711" height="622" alt="image" src="https://github.com/user-attachments/assets/74abdea6-74cc-4403-957b-527161fefee4" />

STM32控制PWM和SD的输出，通过IR204STRPBF和VS的电流和C49自举电容和D5肖特基二极管来控制HO和LO高低电流转换来控制Q1和Q2的通断
输入1K电阻防止电流过大损坏芯片

<img width="774" height="367" alt="image" src="https://github.com/user-attachments/assets/6b9c78fa-1eb5-476a-8cd3-ec0e25e16f5f" />

R82取样电阻
R82分压加R83分压再接运放得电压倍数 34
提供基准电压，单片机不能接收负电压会导致损坏

<img width="211" height="309" alt="image" src="https://github.com/user-attachments/assets/6a1f2d68-6b9e-4e5a-8ecf-b84b84999574" />

1.5V参考电压

<img width="621" height="421" alt="image" src="https://github.com/user-attachments/assets/b68ca82b-4250-4d32-b596-892833a222ee" />

上桥下桥靠2104驱动四个mos管输出交流电压
二极管快速拉低G S电压
电阻消耗寄生电容电压
<img width="3072" height="4080" alt="IMG_20260427_205225" src="https://github.com/user-attachments/assets/160e2387-617e-43ef-9d46-0004612fa81c" />

<img width="824" height="220" alt="image" src="https://github.com/user-attachments/assets/25e41623-90ce-4710-b97a-eccc5596ad5a" />

