# 📺 ESP32 2: TV y ventilador

## Televisor
Un enchufe inteligente no sirve: solo corta o restablece la corriente y el TV no se enciende solo al recibirla. Por eso el ESP32 lleva un emisor infrarrojo (LED IR) que replica las señales del control remoto original (encendido, apagado, volumen, etc.).

## Ventilador
- **Botones simples (encendido/apagado):** un relé controlado por el ESP32 es suficiente.
- **Control de velocidad:** depende del modelo específico y requiere más análisis.

## Control
- **Voz:** "Philip, enciende el televisor", "Philip, apaga el ventilador".
- **App:** desde Home Assistant.
- **Manual:** control remoto del TV y botones del ventilador.

## Materiales
- ESP32
- Emisor infrarrojo (LED IR)
- Relé (ventilador)

## Pendientes
- [ ] Capturar las señales del control remoto del TV
- [ ] Ubicar el emisor con línea de vista al televisor
- [ ] Definir si el ventilador tiene solo encendido/apagado o también velocidades
