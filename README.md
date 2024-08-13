# SW-MCU-STM32-W2812-RGB-011

Here is a RGB LED Controller Test Code uses PMW for STM32 microcontrollers.

If you look WS2812 datasheets, you can easly calculate PSC and ARR values.

In datasheet: Data transfer time=(TH+TL=1.25µs). I use Timer in MAX speed(240Mhz).

Here is my settings:

1.25 so it need 800 000 kHZ

240 000 000 / 800 000 = 300

Prescaler(PSC) = 1-1 and AutoReloadRegister(ARR) = 300-1

Here is result:

![STM32-RGB](https://github.com/user-attachments/assets/cf48989f-0160-4d10-a50f-8bc0dab72ecf)

Hope this helps you,

Ceyhun Pempeci STM32 WS2812 RGB
