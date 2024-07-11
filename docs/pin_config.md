# APM2 GPIO configuration

## Mapping of GPIO for APM2

It is done by the function **digitalPinToBitMask(pin)** and **digitalPinToPort(pin)**, it receives as argument the pin number of APM board.
These functions will assign pins according the file *pins_arduino_mega.cpp*.

`PE0 ** 0 ** USART0_RX
PE1 ** 1 ** USART0_TX
PE4 ** 2 ** PWM2
PE5 ** 3 ** PWM3
PG5 ** 4 ** PWM4
PE3 ** 5 ** PWM5
PH3 ** 6 ** PWM6
PH4 ** 7 ** PWM7
PH5 ** 8 ** PWM8
PH6 ** 9 ** PWM9
PB4 ** 10 ** PWM10
PB5 ** 11 ** PWM11
PB6 ** 12 ** PWM12
PB7 ** 13 ** PWM13
PJ1 ** 14 ** USART3_TX
PJ0 ** 15 ** USART3_RX
PH1 ** 16 ** USART2_TX
PH0 ** 17 ** USART2_RX
PD3 ** 18 ** USART1_TX
PD2 ** 19 ** USART1_RX
PD1 ** 20 ** I2C_SDA
PD0 ** 21 ** I2C_SCL
PA0 ** 22 ** D22
PA1 ** 23 ** D23
PA2 ** 24 ** D24
PA3 ** 25 ** D25
PA4 ** 26 ** D26
PA5 ** 27 ** D27
PA6 ** 28 ** D28
PA7 ** 29 ** D29
PC7 ** 30 ** D30
PC6 ** 31 ** D31
PC5 ** 32 ** D32
PC4 ** 33 ** D33
PC3 ** 34 ** D34
PC2 ** 35 ** D35
PC1 ** 36 ** D36
PC0 ** 37 ** D37
PD7 ** 38 ** D38
PG2 ** 39 ** D39
PG1 ** 40 ** D40
PG0 ** 41 ** D41
PL7 ** 42 ** D42
PL6 ** 43 ** D43
PL5 ** 44 ** D44
PL4 ** 45 ** D45
PL3 ** 46 ** D46
PL2 ** 47 ** D47
PL1 ** 48 ** D48
PL0 ** 49 ** D49
PB3 ** 50 ** SPI_MISO
PB2 ** 51 ** SPI_MOSI
PB1 ** 52 ** SPI_SCK
PB0 ** 53 ** SPI_SS
PF0 ** 54 ** A0
PF1 ** 55 ** A1
PF2 ** 56 ** A2
PF3 ** 57 ** A3
PF4 ** 58 ** A4
PF5 ** 59 ** A5
PF6 ** 60 ** A6
PF7 ** 61 ** A7
PK0 ** 62 ** A8
PK1 ** 63 ** A9
PK2 ** 64 ** A10
PK3 ** 65 ** A11
PK4 ** 66 ** A12
PK5 ** 67 ** A13
PK6 ** 68 ** A14
PK7 ** 69 ** A15
PE6 ** 70 ** APM only`
