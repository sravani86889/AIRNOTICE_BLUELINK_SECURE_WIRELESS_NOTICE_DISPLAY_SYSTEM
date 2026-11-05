# AIRNOTICE_BLUELINK_SECURE_WIRELESS_NOTICE_DISPLAY_SYSTEM
AirNotice BlueLink – Secure Wireless Display System is a modern alternative to traditional notice boards. An Android app sends messages via Bluetooth to a microcontroller, which verifies a security code and displays the approved text on a scrolling dot-matrix LED. It enables secure, flexible communication for schools, offices, and public spaces.

Features

📲 Android-based wireless message transmission (Bluetooth – HC-05)

🔐 Passkey-protected message authentication

💾 EEPROM-based message storage (AT25LC512)

🔄 Continuous scrolling display on 4 × 8x8 dot-matrix LEDs

⚡ UART interrupt-based communication

🛑 Auto-update display when new authorized message is received

🕒 Default message display: “Waiting for message”

🛠 Hardware Requirements

LPC2148 Microcontroller

4 × 8x8 Dot Matrix LED Displays

74HC573 (Latch)

74HC164 (Shift Register)

AT25LC512 EEPROM

HC-05 Bluetooth Module

DB-9 Cable / USB-UART Converter

💻 Software Requirements

KEIL C Compiler

Embedded C Programming

Flash Magic (for programming LPC2148)

HC-05 Terminal App (Android)

🔌 System Architecture

Android app sends message via Bluetooth.

LPC2148 receives message using UART interrupt.

System verifies passkey (e.g., 786VectorIndia).

Valid message is stored in EEPROM.

Stored message scrolls continuously on dot-matrix display.

If no message exists → displays “Waiting for message”.

🔐 Security Format

Message must follow this syntax:

$\$$$

Example:

786VectorIndia

Displayed Output:

Vector India

Only messages with the correct passkey are accepted.

