# PET Bot Controller PCB

A compact **6x6 cm**, DIY-friendly, **single-layer PCB** for controlling up to **8 servo motors** with an **ESP32**.  
This board is specifically designed for easy at-home manufacturing via the **chemical etching process**, using robust **40-mil traces** and common **through-hole components**.

---

## 🔑 Key Features

| Feature         | Description                                                      |
|-----------------|------------------------------------------------------------------|
| **MCU**         | ESP32 DevKitC (Wi-Fi & Bluetooth)                                |
| **Motor Control** | 8 Servo motor channels                                          |
| **Power**       | On-board footprint for a buck converter module (e.g., MP1584EN)  |
| **DIY-Friendly** | Single-sided layout with wide 40-mil traces, easy THT soldering |
| **Grounding**   | Full GND polygon pour for electrical stability                   |

---

## 📋 Component List

| Qty | Part Description                | Type       | Notes                        |
|-----|---------------------------------|------------|------------------------------|
| 1   | ESP32 DevKitC (30/38-pin)       | Module     |                              |
| 1   | Buck Converter Module           | Module     | MP1584EN, LM2596, etc.       |
| 8   | 3-Pin Male Headers              | Connector  | For servo connections        |
| 2   | 2-Pin Screw Terminal (5.08mm)   | Connector  | For power input/output       |
| 2   | Electrolytic Capacitor (100–470uF) | THT     | 16V or 25V for power smoothing |
| 1   | 6x6 cm Copper Clad Board        | Material   | Single-sided                 |

---

## 🛠️ Manufacturing Steps (Toner Transfer Method)

1. **Print**: Print the 1:1 scale PDF layout onto glossy paper using a **laser printer**.
2. **Transfer**: Iron the print (toner side down) onto a cleaned copper-clad board.
3. **Soak & Peel**: Submerge in water to soften and remove the paper backing.
4. **Etch**: Place the board in an etchant (e.g., Ferric Chloride) to remove exposed copper.
5. **Clean**: Remove the toner resist with acetone to reveal copper traces.
6. **Drill**: Drill all holes for components.
7. **Solder**: Solder all components onto the board.

---

## 🔌 Firmware & Pinout

Program the **ESP32** using the **Arduino IDE** or **PlatformIO** with the [`ESP32Servo`](https://github.com/jkb-git/ESP32Servo) library.

**Servo Pin Mapping** *(update with your actual GPIO connections)*:

| Servo  | GPIO Pin |
|--------|----------|
| SERVO_1 | GPIO_XX |
| SERVO_2 | GPIO_XX |
| SERVO_3 | GPIO_XX |
| SERVO_4 | GPIO_XX |
| SERVO_5 | GPIO_XX |
| SERVO_6 | GPIO_XX |
| SERVO_7 | GPIO_XX |
| SERVO_8 | GPIO_XX |

---
