# CH32V203 を利用した DAPLink

<img src="images/photo1.jpg" width="30%" /><img src="images/photo2.jpg" width="30%" />

<img src="images/photo3.jpg" width="30%" /><img src="images/photo4.jpg" width="30%" />

- Shop: https://booth.pm/ja/items/4916891

## features

- SWD のデバッガとして使える
- USB シリアル変換として使える
- 1.27mm ピッチ 10 ピンの SWD と互換性のあるポートを持っている（ただし SWO はなし）
- Arduino UNO R4 の SWD + UART の 1.27mm ピッチ 10 ピンと互換性のあるポートを持っている
- 10 ピンコネクタの VCC を 5V、3.3V を切り替えることができる（Arduino UNO R4 では 5V が必要）
- USB-C

## SWD 10pin Connector

<img src="images/swd-connector.png" width="50%" />

## Firmware

https://github.com/XIVN1987/DAPLink/tree/master/CH32V203

## v1.1.0

R2、R3 は NC にすること。

- semantics: [pdf](ch32v203-daplink-v1.1.0-semantics.pdf) [kicanvas](https://kicanvas.org/?github=https%3A%2F%2Fgithub.com%2F74th%2Fch32v203-daplink-pcb%2Fblob%2Fmain%2Fch32v203-daplink-pcb.kicad_sch)
- pcb: [pdf](ch32v203-daplink-v1.1.0-pcb.pdf) [kicanvas](https://kicanvas.org/?github=https%3A%2F%2Fgithub.com%2F74th%2Fch32v203-daplink-pcb%2Fblob%2Fmain%2Fch32v203-daplink-pcb.kicad_pcb)

## BOM

| Reference  | Name                                | Quantity |
| ---------- | ----------------------------------- | -------- |
| C1, C2     | Capacitor 0603 22pF                 | 2        |
| C3, C4, C7 | Capacitor 0603 10uF                 | 3        |
| C5         | Capacitor 0603 2.2uF                | 1        |
| C6, C8, C9 | Capacitor 0603 100nF                | 3        |
| D1         | LED 0805 Blue                       | 1        |
| D2         | LED 0805 Red                        | 1        |
| J1         | USB Type-C Receptacle - USB2.0_C_v3 | 1        |
| J2         | Box Pin Header 2x5 Pitch 1.27mm     | 1        |
| J3         | Pin Header 2x5 Pitch 2.54mm         | 1        |
| R1-R3, R5  | Register 0603 10kΩ                  | 4        |
| R4, R6, R7 | Register 0603 5.1kΩ                 | 3        |
| SW1        | Slide Switch                        | 1        |
| U1         | MCU LQFP48 WCH CH32V203C8T6         | 1        |
| U2         | Regulator 3.3V SOT-223 AMS1117-3.3  | 1        |
| Y1         | Crystal 3225 8MHz                   | 1        |

## LICENSE

- Firmware: https://github.com/XIVN1987/DAPLink/blob/master/LICENSE
- PCB: MIT
