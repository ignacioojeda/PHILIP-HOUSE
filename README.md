# 🏠 Philip: domótica de mi casa

Proyecto de domótica para mi cuarto y el jardín. Una Raspberry Pi es el cerebro central y varios ESP32 controlan los dispositivos. Todo se maneja por voz con **Philip**, y la app de Home Assistant queda como respaldo.

## Arquitectura

- **Cerebro:** Raspberry Pi económica (Zero 2 W o Pi 4) con Home Assistant.
- **Nodos:** 3 ESP32 con firmware ESPHome, conectados a corriente (no a pilas, por el consumo del WiFi) y reportando por WiFi.
- **Voz:** Home Assistant Assist, con posible integración de un LLM.
- El Arduino Mega queda libre para la universidad y no se usa en este proyecto.

| Nodo | Controla |
| --- | --- |
| ESP32 cuarto | Televisor (infrarrojo) y ventilador |
| ESP32 cortina | Motor DC de la cortina blackout |
| ESP32 jardín + luz | Riego automático e interruptor de luz normal |

Las luces LED de colores van aparte, en un enchufe inteligente.

## Módulos

- [Luz normal](docs/luz.md)
- [Luces LED de colores](docs/luces-led.md)
- [Televisor](docs/televisor.md)
- [Ventilador](docs/ventilador.md)
- [Cortina blackout](docs/cortina.md)
- [Riego del jardín](docs/riego.md)
- [Asistente de voz Philip](docs/asistente-philip.md)
- [Lista de materiales](docs/materiales.md)

## Estado

Fase de planeación. Ver los pendientes en cada módulo.
