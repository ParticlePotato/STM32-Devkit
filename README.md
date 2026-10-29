# STM32G474RETx DevKit

A compact, 40-pin breadboard-friendly development board based on the high-performance **STM32G474RETx** microcontroller (LQFP64). Designed for advanced analog applications, digital power control, and versatile prototyping.

## 🚀 Key Features
* **MCU:** STM32G474RETx (Arm® Cortex®-M4 with FPU, 170 MHz, 512 KB Flash)
* **Form Factor:** 40-pin dual-row header layout (2x20 pins)
* **Power Supply:** Dual rail design (+5V and +3V3 LDO output) via Micro USB or external pins
* **Hardware Safe:** Integrated input diode protection and power state LED indicator
* **Debug Support:** Standard SWD interface header (SWDIO, SWCLK, SWO, NRST)
* **User Control:** Onboard Reset button (SW1) and Boot selector (SW2)

## 🛠️ Hardware Design Architecture

### 1. Power Distribution & Regulation
* **LDO Regulator:** High-efficiency **AMS1117-3.3** drops the incoming +5V rail down to a stable +3V3 for the MCU logic.
* **Decoupling Network:** Dedicated 100nF ceramic capacitors placed adjacent to every individual VDD pin.
* **Analog Isolation:** **VDDA** and **VREF+** lines are isolated from the main digital power rail using a ferrite bead (FB2) and a 100nF/1uF capacitor array to maintain low-noise ADC/DAC precision.

### 2. Clock & System Controls
* **Main Clock (HSE):** Driven by an external 16 MHz crystal oscillator setup with 18pF load capacitors for stable system timing.
* **Boot Configuration:** BOOT0 pin is tied to GND via a 10kΩ resistor for default Flash booting, accessible via a dedicated switch (SW2).

## 📌 Header Pinout Layout

### Connector J2 (Left Header)
* **Pin 1:** +3V3
* **Pins 2:** GND
* **Pins 3:** VBUS
* **Pin 4:** ADC/TIM
* **Pins 5:** ADC/TIM
* **Pins 6:** ADC/TIM
* **Pin 7:** ADC/TIM
* **Pins 8:** ADC/TIM
* **Pins 9:** ADC/TIM
* **Pin 10:** ADC/TIM
* **Pins 11:** ADC/TIM
* **Pins 12:** ADC/TIM
* **Pin 13:** ADC/TIM
* **Pins 14:** ADC/TIM
* **Pins 15:** ADC/TIM
* **Pins 16:** ADC/TIM
* **Pins 17:** ADC/TIM
* **Pin 18:** TIM
* **Pins 19:** TIM
* **Pins 20:** TIM

### Connector J6 (Right Header)
* **Pin 1:** +3V3
* **Pins 2:** GND
* **Pins 3:** +5V 
* **Pin 4:** UART/ADC/TIM
* **Pins 5:** UART/TIM
* **Pins 6:** I2C/TIM
* **Pin 7:** I2C/ADC/TIM
* **Pins 8:** ADC/TIM
* **Pins 9:** ADC/TIM
* **Pin 10:** ADC/TIM
* **Pins 11:** ADC/TIM
* **Pins 12:** ADC/TIM
* **Pin 13:** ADC/TIM
* **Pins 14:** TIM
* **Pins 15:** TIM
* **Pins 16:** ADC/TIM
* **Pins 17:** TIM
* **Pin 18:** TIM/GPIO
* **Pins 19:** GPIO(0v or 3.3v)
* **Pins 20:** GPIO(0v or 3.3v)

## 📄 License
This project is open-source and released under the [MIT License](LICENSE).
