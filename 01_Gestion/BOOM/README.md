Aquí tienes la sección lista, ajustada al proyecto **TrackLogic** y basada en el documento de materiales:

---

# 🛒 Lista de Materiales

## Bill of Materials - BOM

Este documento presenta los componentes necesarios para el desarrollo de una unidad funcional del sistema del grupo **TrackLogic**. La lista incluye los elementos principales de control, percepción, conectividad, alimentación y mecánica que permiten el funcionamiento del proyecto.

---

## ⚡ Electrónica Principal

| Ítem | Componente               | Cant. | Referencia / Especificación | Función                                               | Est. Costo |
| ---- | ------------------------ | ----: | --------------------------- | ----------------------------------------------------- | ---------: |
| 1    | Microcontrolador         |     1 | ESP32 Dev Module            | Control principal del sistema y conexión con sensores |    $10.000 |
| 2    | Sensor de ritmo cardiaco |     1 | MAX30105                    | Medición de señales biométricas                       |    $30.000 |
| 3    | Sensor de movimiento     |     1 | MPU6050 GY-521              | Medición de movimiento, inclinación y aceleración     |    $20.000 |
| 4    | Sensor de temperatura    |     1 | MLX90614ESF-BAA             | Medición de temperatura sin contacto                  |    $47.000 |
| 5    | Sensor secundario        |     1 | MAX30102                    | Apoyo en medición biométrica                          |    $28.000 |

---

## 🔋 Sistema de Potencia

En el documento se identifica que el sistema de alimentación aún se encuentra en definición. Por esta razón, este apartado queda como pendiente hasta seleccionar la batería más adecuada para alimentar el ESP32 y los sensores de forma inalámbrica.

| Ítem | Componente                    | Cant. | Referencia / Especificación | Función                         | Estado    |
| ---- | ----------------------------- | ----: | --------------------------- | ------------------------------- | --------- |
| 6    | Batería para alimentación     |     1 | Por definir                 | Fuente de energía principal     | Pendiente |
| 7    | Sistema de carga o regulación |     1 | Por definir                 | Gestión de energía del circuito | Pendiente |

---

## 🛠️ Interfaz y Mecánica

Esta sección reúne los elementos relacionados con la estructura física y la integración del sistema. Según la planeación, el chaleco aún debe diseñarse y adaptarse para integrar los sensores y el circuito.

| Ítem | Componente         | Cant. | Referencia / Especificación            | Función                           | Estado          |
| ---- | ------------------ | ----: | -------------------------------------- | --------------------------------- | --------------- |
| 8    | Chaleco            |     1 | Diseño pendiente                       | Soporte físico del sistema        | Bloqueante      |
| 9    | PCB / Baquela      |     1 | Diseño en Proteus y montaje en baquela | Base del circuito                 | En modificación |
| 10   | Buzzer             |     1 | Buzzer electrónico                     | Señal sonora o alerta del sistema | Listo para PCB  |
| 11   | Cableado e insumos |     1 | Cables, estaño y conectores            | Ensamble del circuito             | Requerido       |

---

## 💰 Resumen de Presupuesto

| Categoría                        | Subtotal Estimado |
| -------------------------------- | ----------------: |
| Electrónica principal y sensores |          $135.000 |
| Potencia y energía               |       Por definir |
| Mecánica e insumos               |       Por definir |
| **TOTAL PARCIAL ESTIMADO**       |  **$135.000 COP** |

Los costos corresponden a valores estimados registrados en la planeación del proyecto, usando proveedores como **AliExpress** y **MercadoLibre**.

---

## 📍 Proveedores Identificados

Los proveedores mencionados para la adquisición de componentes son:

* **AliExpress:** ESP32, MAX30105.
* **MercadoLibre:** MPU6050, MLX90614 y MAX30102.
* **Universidad / laboratorio:** apoyo para diseño, pruebas, PCB, baquela y estructura del chaleco.

---

## 🔍 Observaciones

Algunos componentes ya se encuentran disponibles, como el **ESP32**, el **MPU6050** y el **MAX30102**. Sin embargo, otros elementos siguen pendientes, como el **MAX30105**, el **MLX90614**, la batería de alimentación y el diseño final del chaleco. Por eso, estos elementos deben priorizarse para continuar con la fase de montaje y pruebas del sistema.
