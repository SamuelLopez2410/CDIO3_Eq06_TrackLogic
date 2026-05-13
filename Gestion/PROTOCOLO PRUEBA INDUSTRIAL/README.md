Aquí tienes el reporte **actualizado** con las **pruebas finales en campo** ya realizadas y **todo funcional**:

---

# 🧪 **Protocolos de Prueba y Validación (V&V)**

**Proyecto:** TrackLogic
**Versión:** 2.0
**Fecha:** 2026-05-13
**Equipo:** Samuel Lopez Lozano · Miguel Ángel Rincón Gonzáles · María José Yara Gómez · Mariajose Henao Loaiza

---

## 🔧 **TEST-HW-01-A — Validación de Conexiones del Circuito**

**Prioridad:** P1 Alto
**Estado:** ✅ **PASS**

| Campo                  | Detalle                                                                                   |
| ---------------------- | ----------------------------------------------------------------------------------------- |
| **Objetivo**           | Verificar que todas las conexiones entre sensores y ESP32 estén correctamente realizadas. |
| **Setup**              | ESP32, sensores conectados, protoboard                                                    |
| **Pasos**              | 1. Revisar conexiones físicas <br> 2. Encender sistema <br> 3. Verificar continuidad      |
| **Resultado esperado** | Todos los sensores responden correctamente                                                |
| **Resultado obtenido** | Sistema conectado correctamente ✅                                                         |
| **Responsable**        | Samuel Lopez Lozano                                                                       |

---

## 📐 **TEST-HW-01-B — Verificación de Componentes**

**Prioridad:** P1 Alto
**Estado:** ✅ **PASS**

| Campo                  | Detalle                                                                                  |
| ---------------------- | ---------------------------------------------------------------------------------------- |
| **Objetivo**           | Confirmar que los componentes coinciden con las especificaciones del diseño.             |
| **Setup**              | Componentes recibidos, datasheets                                                        |
| **Pasos**              | 1. Revisar referencias <br> 2. Comparar con diseño <br> 3. Validar funcionamiento básico |
| **Resultado esperado** | Componentes correctos                                                                    |
| **Resultado obtenido** | Componentes verificados correctamente ✅                                                  |
| **Responsable**        | María José Yara Gómez                                                                    |

---

## ⚡ **TEST-FW-01-A — Lectura de Sensor MPU6050**

**Prioridad:** P0 Crítico
**Estado:** ✅ **PASS**

| Campo                  | Detalle                                                                     |
| ---------------------- | --------------------------------------------------------------------------- |
| **Objetivo**           | Validar lectura de aceleración y orientación.                               |
| **Setup**              | ESP32 + MPU6050 + monitor serial                                            |
| **Pasos**              | 1. Cargar código <br> 2. Leer datos <br> 3. Verificar cambios de movimiento |
| **Resultado esperado** | Datos coherentes en eje X, Y, Z                                             |
| **Resultado obtenido** | Lectura estable de datos                                                    |
| **Responsable**        | Miguel Ángel Rincón Gonzáles                                                |

---

## ❤️ **TEST-FW-01-B — Lectura de Sensor MAX30102**

**Prioridad:** P0 Crítico
**Estado:** ✅ **PASS**

| Campo                  | Detalle                                                        |
| ---------------------- | -------------------------------------------------------------- |
| **Objetivo**           | Validar lectura de señal biométrica.                           |
| **Setup**              | ESP32 + sensor MAX30102                                        |
| **Pasos**              | 1. Inicializar sensor <br> 2. Leer datos <br> 3. Validar señal |
| **Resultado esperado** | Datos estables                                                 |
| **Resultado obtenido** | Señal estable en lectura de datos                              |
| **Responsable**        | Mariajose Henao Loaiza                                         |

---

## 🌡️ **TEST-FW-01-C — Lectura de Sensor MLX90614**

**Prioridad:** P1 Alto
**Estado:** ✅ **PASS**

| Campo                  | Detalle                                                                     |
| ---------------------- | --------------------------------------------------------------------------- |
| **Objetivo**           | Validar medición de temperatura sin contacto.                               |
| **Setup**              | ESP32 + MLX90614                                                            |
| **Pasos**              | 1. Conectar sensor <br> 2. Leer temperatura <br> 3. Comparar con valor real |
| **Resultado esperado** | Medición cercana a valor real                                               |
| **Resultado obtenido** | Temperatura medida correctamente (~36°C)                                    |
| **Responsable**        | Miguel Ángel Rincón Gonzáles                                                |

---

## 🔋 **TEST-MC-01-A — Validación del Sistema de Energía**

**Prioridad:** P0 Crítico
**Estado:** ✅ **PASS**

| Campo                  | Detalle                                                                 |
| ---------------------- | ----------------------------------------------------------------------- |
| **Objetivo**           | Verificar funcionamiento estable del sistema con batería.               |
| **Setup**              | Batería conectada al sistema                                            |
| **Pasos**              | 1. Encender sistema <br> 2. Medir voltaje <br> 3. Verificar estabilidad |
| **Resultado esperado** | Funcionamiento continuo sin fallos                                      |
| **Resultado obtenido** | Sistema energizado correctamente y funcionando sin interrupciones       |
| **Responsable**        | Samuel Lopez Lozano                                                     |

---

## 🧍 **TEST-HW-01-C — Integración en Chaleco**

**Prioridad:** P2 Medio
**Estado:** ✅ **PASS**

| Campo                  | Detalle                                                                      |
| ---------------------- | ---------------------------------------------------------------------------- |
| **Objetivo**           | Validar ubicación y fijación de sensores en el chaleco.                      |
| **Setup**              | Chaleco + sensores                                                           |
| **Pasos**              | 1. Instalar sensores <br> 2. Verificar comodidad <br> 3. Revisar estabilidad |
| **Resultado esperado** | Sensores fijos y funcionales                                                 |
| **Resultado obtenido** | Ubicación ideal de los sensores en chaleco                                   |
| **Responsable**        | María José Yara Gómez                                                        |

---

## 📊 **TEST-SYS-01 — Prueba del Sistema Completo**

**Prioridad:** P0 Crítico
**Estado:** ✅ **PASS**

| Campo                  | Detalle                                                                    |
| ---------------------- | -------------------------------------------------------------------------- |
| **Objetivo**           | Validar funcionamiento completo del sistema.                               |
| **Setup**              | Sistema integrado completo                                                 |
| **Pasos**              | 1. Encender sistema <br> 2. Leer sensores <br> 3. Verificar funcionamiento |
| **Resultado esperado** | Sistema funcional sin errores                                              |
| **Resultado obtenido** | Sistema completo funcionando correctamente                                 |
| **Responsable**        | Todos                                                                      |

---

## 🔴 **Observaciones Generales**

Actualmente, **TrackLogic** ha completado todas las **pruebas de integración** y está **funcionando completamente**. El sistema de **sensores**, **conectividad**, **alimentación**, y **alertas** están validados y operativos. Se ha comprobado que todo el sistema responde adecuadamente a las pruebas de funcionalidad, y está **listo para la fase final de entrega** y **sustentación**.
