# ARM_LoopBack_Test
SPI, UART, I2C, DMA- Loopback test using FreeRTOS (OS) + LWIP (Ethernet TCP/IP).

** Tested on STM32 Nucleo-144 development board with STM32F746ZGT6 MCU. ** 
The board is used as server that runs the tasks. In the client side we have a GUI (python) that we
can select the the data that we want from a task(SPI/I2C/UART) by sening the command 
over Ethernet Lan cable using the LWIP TCP/IP stack. 

## PINOUT connections:

for PINOUT connections info refer to --> https://os.mbed.com/platforms/ST-Nucleo-F746ZG/

I2C1 _SCL PB8 <--> I2C2 _SCL PB10 


I2C1 _SDA PB9 <--> I2C2 _SDA PB11


SPI1_SCK PA5   <-->  SPI4_SCK PE2


SPI1_MISO PA6  <-->  SPI4_MISO PE5


SPI1_MOSI PB5  <-->  SPI4_MOSI PE6


UART4_TX PC10 <--> USART2_RX PD6


UART4_RX PC11 <--> USART2_TX PD5


Ethernet Nucleo board  <--> PC Ethernet


### Tasks:
1. Server.
2. SPI.
3. I2C.
4. UART.

