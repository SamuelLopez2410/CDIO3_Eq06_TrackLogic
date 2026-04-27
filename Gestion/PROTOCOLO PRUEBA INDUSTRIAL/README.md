# 🧪 Protocolos de Prueba — Validación y Verificación (V&V)

**Proyecto:** TrackLogic
**Versión:** 2.0
**Fecha:** 2026-04-06
**Equipo:** Samuel Lopez Lozano · Miguel Ángel Rincón Gonzáles · María José Yara Gómez · Mariajose Henao Loaiza

⚠️ Este protocolo debe ser diligenciado antes de ejecutar cualquier prueba. Los resultados deben registrarse en el repositorio o en la bitácora del proyecto.

---

## 🔧 TEST-HW-01-A — Validación de Conexiones del Circuito

**Prioridad:** P1 Alto
**Estado:** ✅ PASS

| Campo              | Detalle                                                                                  |
| ------------------ | ---------------------------------------------------------------------------------------- |
| Objetivo           | Verificar que todas las conexiones entre sensores y ESP32 estén correctamente realizadas |
| Setup              | ESP32, sensores conectados, protoboard                                                   |
| Pasos              | 1. Revisar conexiones físicas · 2. Encender sistema · 3. Verificar continuidad           |
| Resultado esperado | Todos los sensores responden correctamente                                               |
| Resultado obtenido | Sistema conectado correctamente ✅                                                        |
| Responsable        | Samuel Lopez Lozano                                                                      |

---

## 📐 TEST-HW-01-B — Verificación de Componentes

**Prioridad:** P1 Alto
**Estado:** ✅ PASS

| Campo              | Detalle                                                                            |
| ------------------ | ---------------------------------------------------------------------------------- |
| Objetivo           | Confirmar que los componentes coinciden con las especificaciones del diseño        |
| Setup              | Componentes recibidos, datasheets                                                  |
| Pasos              | 1. Revisar referencias · 2. Comparar con diseño · 3. Validar funcionamiento básico |
| Resultado esperado | Componentes correctos                                                              |
| Resultado obtenido | Componentes verificados correctamente ✅                                            |
| Responsable        | María José Yara Gómez                                                              |

---

## ⚡ TEST-FW-01-A — Lectura de Sensor MPU6050

**Prioridad:** P0 Crítico
**Estado:** 🚧 EN PROCESO

| Campo              | Detalle                                                               |
| ------------------ | --------------------------------------------------------------------- |
| Objetivo           | Validar lectura de aceleración y orientación                          |
| Setup              | ESP32 + MPU6050 + monitor serial                                      |
| Pasos              | 1. Cargar código · 2. Leer datos · 3. Verificar cambios de movimiento |
| Resultado esperado | Datos coherentes en eje X, Y, Z                                       |
| Resultado obtenido | Lectura parcial — requiere ajuste                                     |
| Responsable        | Miguel Ángel Rincón Gonzáles                                          |

---

## ❤️ TEST-FW-01-B — Lectura de Sensor MAX30102

**Prioridad:** P0 Crítico
**Estado:** 🚧 EN PROCESO

| Campo              | Detalle                                                  |
| ------------------ | -------------------------------------------------------- |
| Objetivo           | Validar lectura de señal biométrica                      |
| Setup              | ESP32 + sensor MAX30102                                  |
| Pasos              | 1. Inicializar sensor · 2. Leer datos · 3. Validar señal |
| Resultado esperado | Datos estables                                           |
| Resultado obtenido | Señal inestable                                          |
| Responsable        | Mariajose Henao Loaiza                                   |

---

## 🌡️ TEST-FW-01-C — Lectura de Sensor MLX90614

**Prioridad:** P1 Alto
**Estado:** 📋 PENDIENTE

| Campo              | Detalle                                                               |
| ------------------ | --------------------------------------------------------------------- |
| Objetivo           | Validar medición de temperatura sin contacto                          |
| Setup              | ESP32 + MLX90614                                                      |
| Pasos              | 1. Conectar sensor · 2. Leer temperatura · 3. Comparar con valor real |
| Resultado esperado | Medición cercana a valor real                                         |
| Resultado obtenido | Pendiente                                                             |
| Responsable        | Miguel Ángel Rincón Gonzáles                                          |

---

## 🔋 TEST-MC-01-A — Validación del Sistema de Energía

**Prioridad:** P0 Crítico
**Estado:** 📋 PENDIENTE

| Campo              | Detalle                                                           |
| ------------------ | ----------------------------------------------------------------- |
| Objetivo           | Verificar funcionamiento estable del sistema con batería          |
| Setup              | Batería conectada al sistema                                      |
| Pasos              | 1. Encender sistema · 2. Medir voltaje · 3. Verificar estabilidad |
| Resultado esperado | Funcionamiento continuo sin fallos                                |
| Resultado obtenido | Pendiente                                                         |
| Responsable        | Samuel Lopez Lozano                                               |

---

## 🧍 TEST-HW-01-C — Integración en Chaleco

**Prioridad:** P2 Medio
**Estado:** 📋 PENDIENTE

| Campo              | Detalle                                                                |
| ------------------ | ---------------------------------------------------------------------- |
| Objetivo           | Validar ubicación y fijación de sensores en el chaleco                 |
| Setup              | Chaleco + sensores                                                     |
| Pasos              | 1. Instalar sensores · 2. Verificar comodidad · 3. Revisar estabilidad |
| Resultado esperado | Sensores fijos y funcionales                                           |
| Resultado obtenido | Pendiente                                                              |
| Responsable        | María José Yara Gómez                                                  |

---

## 📊 TEST-SYS-01 — Prueba del Sistema Completo

**Prioridad:** P0 Crítico
**Estado:** 📋 PENDIENTE

| Campo              | Detalle                                                              |
| ------------------ | -------------------------------------------------------------------- |
| Objetivo           | Validar funcionamiento completo del sistema                          |
| Setup              | Sistema integrado completo                                           |
| Pasos              | 1. Encender sistema · 2. Leer sensores · 3. Verificar funcionamiento |
| Resultado esperado | Sistema funcional sin errores                                        |
| Resultado obtenido | Pendiente                                                            |
| Responsable        | Todos                                                                |

---

## 🔴 Observaciones generales

Actualmente el proyecto **TrackLogic** presenta avances en la verificación de componentes y conexiones, pero aún se encuentra en proceso de validación de sensores y pruebas completas del sistema. Las principales dificultades están en la estabilidad de las lecturas y en la integración total del hardware.
