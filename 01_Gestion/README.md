# Resultados de Diseño — Planos As-Built y Auditoría de Costos

**Proyecto:** TrackLogic
**Versión:** 2.0
**Fecha:** 2026-04-06

---

## 1. Esquemático Electrónico As-Built

### Mapa de conexiones confirmado

| Componente | Pin | ESP32           | Función                            | Protocolo |
| ---------- | --- | --------------- | ---------------------------------- | --------- |
| MAX30102   | VCC | 3.3V            | Alimentación del sensor biométrico | —         |
| MAX30102   | GND | GND             | Tierra común                       | —         |
| MAX30102   | SDA | GPIO 21         | Datos                              | I²C       |
| MAX30102   | SCL | GPIO 22         | Reloj                              | I²C       |
| MPU6050    | VCC | 3.3V            | Alimentación del sensor IMU        | —         |
| MPU6050    | GND | GND             | Tierra común                       | —         |
| MPU6050    | SDA | GPIO 21         | Datos                              | I²C       |
| MPU6050    | SCL | GPIO 22         | Reloj                              | I²C       |
| MLX90614   | VCC | 3.3V            | Alimentación sensor temperatura    | —         |
| MLX90614   | GND | GND             | Tierra común                       | —         |
| MLX90614   | SDA | GPIO 21         | Datos                              | I²C       |
| MLX90614   | SCL | GPIO 22         | Reloj                              | I²C       |
| Buzzer     | +   | GPIO 25         | Alerta sonora                      | Digital   |
| Buzzer     | -   | GND             | Tierra común                       | —         |
| Batería    | +   | VIN / Regulador | Alimentación principal             | DC        |
| Batería    | -   | GND             | Tierra común                       | —         |

**Archivo de diseño:** Esquemático del circuito / diseño en Proteus
**Ubicación sugerida:** `/5_Resultados_Diseno/`

---

## 2. Dimensiones Mecánicas As-Built

| Parámetro              | Diseño                    | Medido / Estado actual      | Estado         |
| ---------------------- | ------------------------- | --------------------------- | -------------- |
| Ubicación del circuito | Integrado en chaleco      | En definición               | 🚧 Validando   |
| Tipo de montaje        | PCB / baquela             | Diseño en modificación      | 🚧 En proceso  |
| Sensores biométricos   | Integrados al usuario     | MAX30102 / MAX30105         | 🚧 Validando   |
| Sensor de movimiento   | Integrado en zona estable | MPU6050                     | ✅ Seleccionado |
| Sensor de temperatura  | Medición sin contacto     | MLX90614                    | ✅ Seleccionado |
| Material de soporte    | Chaleco                   | Diseño pendiente            | 📋 Planificado |
| Peso del sistema       | Ligero y portable         | Pendiente de medición final | 📋 Planificado |

---

## 3. Auditoría de Costos del Proyecto

Según el documento de economía del proyecto, el presupuesto total de **TrackLogic** incluye personal, equipos, materiales, viajes, servicios técnicos y licencia de software. El total general estimado del proyecto es de **$13.635.000 COP**. 

### Componentes principales

| Ítem | Componente       | Precio estimado | Estado         |
| ---- | ---------------- | --------------: | -------------- |
| 1    | ESP32 Dev Module |         $10.000 | ✅ Seleccionado |
| 2    | MAX30105         |         $30.000 | 🚧 En proceso  |
| 3    | MPU6050 GY-521   |         $20.000 | ✅ Seleccionado |
| 4    | MLX90614         |         $47.000 | 🚧 En proceso  |
| 5    | MAX30102         |         $28.000 | ✅ Seleccionado |
| 6    | Batería          |     Por definir | 📋 Pendiente   |
| 7    | Buzzer           |     Por definir | 📋 Pendiente   |
| 8    | PCB / Baquela    |     Por definir | 🚧 En proceso  |
| 9    | Chaleco          |     Por definir | 📋 Pendiente   |
| 10   | Cables e insumos |     Por definir | 📋 Pendiente   |

---

## 4. Resumen de Costos

| Categoría              |      Valor estimado |
| ---------------------- | ------------------: |
| Personal               |          $1.200.000 |
| Equipos                |          $6.500.000 |
| Materiales e insumos   |            $135.000 |
| Viajes                 |            $600.000 |
| Servicios técnicos     |          $3.600.000 |
| Licencia software      |          $2.000.000 |
| **Total del proyecto** | **$13.635.000 COP** |

El costo variable unitario del sistema se estimó en **$135.000 COP**, y el precio de venta calculado con un margen del 50% fue de **$270.000 COP por unidad**. 

---

## 5. Punto de Equilibrio

El margen de contribución por unidad es de **$135.000 COP**, porque el precio de venta estimado es de $270.000 y el costo variable unitario es de $135.000. Con estos valores, el proyecto necesita vender **101 unidades** para alcanzar el punto de equilibrio. 

---

## 6. Referencias de Archivos

| Archivo                   | Descripción                       | Ubicación sugerida      |
| ------------------------- | --------------------------------- | ----------------------- |
| Esquemático_TrackLogic    | Diseño electrónico del sistema    | `/5_Resultados_Diseno/` |
| BOM_TrackLogic.xlsx       | Lista de materiales               | `/2_Planeacion/`        |
| Economia_del_proyecto.pdf | Presupuesto y punto de equilibrio | `/3_Gestion/`           |
| Actas de reunión          | Seguimiento del equipo            | `/1_Actas/`             |
| Informe final             | Documento técnico del proyecto    | `/6_Documentacion/`     |
