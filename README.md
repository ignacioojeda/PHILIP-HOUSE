# 🏠 Philip

Philip es el sistema de domótica de mi casa (cuarto y jardín). Una Raspberry Pi con Home Assistant es el cerebro, y desde ahí Philip controla todo de tres maneras:

- **Por voz**, con Home Assistant Assist (posible integración con un LLM para conversar de forma más natural).
- **Por app**, con la app de Home Assistant.
- **De forma manual**, con los interruptores y botones físicos de cada dispositivo.

## Arquitectura

- **Cerebro:** Raspberry Pi económica (Zero 2 W o Pi 4) con Home Assistant.
- **Nodos:** 5 ESP32 con firmware ESPHome, conectados a corriente (no a pilas, por el consumo del WiFi), reportando por WiFi.
- El Arduino Mega queda libre para la universidad y no se usa en este proyecto.

| # | ESP32 | Controla | Documentación |
| --- | --- | --- | --- |
| 1 | Jardín | Riego automático | [docs/01-jardin.md](docs/01-jardin.md) |
| 2 | TV y ventilador | Televisor (infrarrojo) y ventilador | [docs/02-tv-ventilador.md](docs/02-tv-ventilador.md) |
| 3 | Luz normal | Luz de techo del cuarto | [docs/03-luz-normal.md](docs/03-luz-normal.md) |
| 4 | Luces LED y lámpara | Luces LED de colores y lámpara de trabajo | [docs/04-luces-led-lampara.md](docs/04-luces-led-lampara.md) |
| 5 | Cortina | Cortina blackout motorizada | [docs/05-cortina.md](docs/05-cortina.md) |

## 🧰 Lista de materiales

| Elemento | Cantidad | Para |
| --- | --- | --- |
| Raspberry Pi (modelo económico) | 1 | Cerebro central |
| ESP32 | 5 | Jardín, TV y ventilador, luz normal, luces LED y lámpara, cortina |
| Módulo relé empotrable | 1 | Luz normal |
| Relé | 2+ | Ventilador y bomba de riego |
| Emisor infrarrojo (LED IR) | 1 | Televisor |
| Motor DC con caja reductora | 1 | Cortina |
| Driver puente H | 1 | Cortina |
| Botón físico | 1 | Cortina |
| Sensor de humedad de suelo | 1 | Riego |
| Bomba de 12 V | 1 | Riego |

## Por definir
- Conexión de las luces LED y la lámpara de trabajo (relé o enchufe inteligente)
- Micrófono y parlante para Philip

## Por comprar
- [ ] Raspberry Pi
- [ ] 5 ESP32
- [ ] Motor de la cortina (lo busca Andres)

## Estado

Fase de planeación. Los pendientes están al final de cada documento.
