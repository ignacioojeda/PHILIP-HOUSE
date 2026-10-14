# 🪟 ESP32 5: Cortina blackout motorizada

## Datos
- Cortina pesada, cuesta correrla a mano.
- Recorrido del riel: aproximadamente 1.3 m.

## Solución
- Motor DC con caja reductora de torque alto.
- Driver tipo puente H controlado por el ESP32, reutilizando lo aprendido en el proyecto de los carros RC.
- Mecanismo de tracción: polea o eje con cordón enrollable que convierte el giro del motor en movimiento horizontal.

## Control
- **Voz:** "Philip, abre la cortina", "Philip, cierra la cortina".
- **App:** desde Home Assistant.
- **Manual:** un botón físico que abre y cierra.

## Materiales
- ESP32
- Motor DC con caja reductora
- Driver puente H
- Botón físico

## Pendientes
- [ ] Elegir el motor específico según el torque necesario
- [ ] Definir el mecanismo de polea y cordón
- [ ] Definir dónde va el botón y cómo funciona (uno solo o dos: abrir y cerrar)
