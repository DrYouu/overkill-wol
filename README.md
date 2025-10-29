# Overkill-WOL

Un proyecto para encender el PC que se me fue de las manos.

---

## Diagrama conceptual

Un ESP con Tasmota conectado al **5 V permanente** de la fuente de alimentación y al **pin del botón de encendido** de la placa base.

---

## Esquema

• Se configura Tasmota para que funcione como **pulsador**, desactivándose automáticamente **20 ms** después de activarse.  
• Se configura también el **servidor MQTT** y la **Wi-Fi**.  
• En Node-RED se activa un nodo de **salida MQTT** que se integra con el resto del flujo.  
• Además, la **pantalla del PC** está conectada a un relé con Tasmota, por lo que también entra dentro del flujo.

---

## Flujo de Node-RED

En el archivo de apagado personalizado de **Waybar**, se envía una señal al servidor MQTT, por lo que la pantalla **se apaga automáticamente al apagar el equipo**.

Del mismo modo, **se enciende antes que el equipo** mediante la señal correspondiente enviada desde **Alexa**.

---

## Caja impresa

Hay una pequeña cajita impresa en 3D (en material **transparente** y con bastante precisión) que aloja el ESP en la zona de los ventiladores.

---

## Fotos

![soporte](https://cdn.thingiverse.com/assets/77/ba/dc/83/a1/large_display_IMG_0872.jpeg)

---

## STL (Thingiverse)

https://www.thingiverse.com/thing:7184951
---
