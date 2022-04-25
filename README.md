# STM32 Control DYNAMIXEL Motor

Control ROBOTIS DYNAMIXEL motor with MAX485(RS-485 module), STM32 NUCLEO-F446RE and [LibOpenCM3](https://libopencm3.org/).

Tested on [H42-20-S300-R](https://emanual.robotis.com/docs/en/dxl/pro/h42-20-s300-r/) and [H54-200-S500-R](https://emanual.robotis.com/docs/en/dxl/pro/h54-200-s500-r/).

- Example code: [/src/main.c](/src/main.c)  
- [DYNAMIXEL Protocol 2.0](https://emanual.robotis.com/docs/en/dxl/protocol2/) library files: [/lib/DYNAMIXEL/](/lib/DYNAMIXEL/)

## Pin map

| NUCLEO-F446RE Board  | MAX485    |
| -------------------- | --------- |
| D3 (PB3)             | DE and RE |
| D2 (PA10, USART1_RX) | RO        |
| D8 (PA9, USART1_TX)  | DI        |

| DYNAMIXEL Connector | MAX485 |
| ------------------- | ------ |
| 1, GND              | --     |
| 2, VDD              | --     |
| 3, DATA+            | A      |
| 4, DATA-            | B      |

> Ref: [Communication Circuit](https://emanual.robotis.com/docs/en/dxl/pro/h42-20-s300-r/#communication-circuit)