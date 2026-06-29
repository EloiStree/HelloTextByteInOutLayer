# HelloTextByteInOutLayer

> An abstraction layer for building code tournament games, independent of the underlying communication protocol.

Many networking technologies allow applications to exchange both text and binary data. For example, a WebSocket server can send and receive either UTF-8 text messages or raw bytes.

This library exposes four communication channels:

* **Text In** – Receive human-readable commands or configuration messages. Suitable for low-frequency communication.
* **Byte In** – Receive compressed or compact binary data. Optimized for high-frequency updates.
* **Text Out** – Send readable messages, making it easy for beginners to build bots or controllers, at the cost of higher bandwidth usage.
* **Byte Out** – Send compact binary messages for expert users who need the highest update rate with minimal bandwidth.

## Why?

Depending on the project, I may use different networking technologies:

* WebSocket
* UDP
* WebRTC
* Mirror
* ...or any other transport layer.

From the player's perspective, the transport protocol should not matter. A tournament game should expose the same interface regardless of how messages are transmitted.

The goal of **HelloTextByteInOutLayer** is to provide a common abstraction that works across different game engines, frameworks, and microcontrollers.

### Target platforms

* ESP32-S3 (Arduino)
* Raspberry Pi Pico 2 W (CircuitPython)
* Unity [Package](https://github.com/EloiStree/2026_06_29_upm_text_byte_in_out_layer)
* Godot [Package](https://github.com/EloiStree/2026_06_29_gdp_text_byte_in_out_layer)
* Python [Package](https://github.com/EloiStree/2026_06_29_python_text_byte_in_out_layer) 
* Any platform capable of sending and receiving text or binary messages



