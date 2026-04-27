# 📂 Gestión del Proyecto TrackLogic

Este directorio centraliza la documentación administrativa, la planificación, las actas, el cronograma, la lista de materiales y el análisis de requisitos del sistema **TrackLogic**.

**Institución:** Universidad del Quindío
**Programa:** Ingeniería Electrónica
**Ubicación:** Armenia, Quindío, Colombia
**Duración:** Semestre académico

---

## 🎯 Alcance del Proyecto

El objetivo del proyecto **TrackLogic** es desarrollar un sistema embebido portátil, integrado a un chaleco, capaz de monitorear variables biométricas y de movimiento del usuario mediante sensores electrónicos conectados a un microcontrolador ESP32.

---

## 🎯 Objetivos Específicos

* Medir señales biométricas mediante sensores **MAX30102 / MAX30105**.
* Registrar movimiento corporal usando el sensor **MPU6050**.
* Medir temperatura sin contacto con el sensor **MLX90614**.
* Integrar los sensores al **ESP32**.
* Diseñar una estructura tipo **chaleco** para ubicar los componentes.
* Realizar pruebas de funcionamiento y validación del sistema.

---

## 📅 Roadmap de Implementación

### Fase 1: Planeación, componentes y diseño base

| Semanas | Hito / Entregable                                                  | Estado        |
| ------- | ------------------------------------------------------------------ | ------------- |
| 1 - 2   | Organización del equipo, creación del repositorio y tablero Kanban | 🟢 Hecho      |
| 3 - 4   | Revisión de hardware, pedidos y selección de sensores              | 🟢 Hecho      |
| 5 - 6   | Recepción y verificación de componentes electrónicos               | 🟡 En proceso |
| 7 - 8   | Integración inicial de sensores con ESP32                          | 🟡 En proceso |
| 9 - 10  | Diseño del chaleco y ubicación de sensores                         | 🔴 Pendiente  |
| 11 - 12 | Montaje del circuito en PCB / baquela                              | 🔴 Pendiente  |
| 13 - 14 | Pruebas funcionales del sistema completo                           | 🔴 Pendiente  |
| 15 - 16 | Documentación final y sustentación                                 | 🔴 Pendiente  |

---

## ⚙️ Matriz de Requisitos

### Requisitos Funcionales

| Código | Requisito                                                                 |
| ------ | ------------------------------------------------------------------------- |
| RF-001 | El sistema debe medir señales biométricas del usuario.                    |
| RF-002 | El sistema debe registrar movimiento mediante acelerómetro y giroscopio.  |
| RF-003 | El sistema debe medir temperatura sin contacto.                           |
| RF-004 | El sistema debe procesar los datos usando un ESP32.                       |
| RF-005 | El sistema debe emitir alertas mediante buzzer.                           |
| RF-006 | El sistema debe permitir la integración física de sensores en un chaleco. |
| RF-007 | El sistema debe permitir pruebas y validación de funcionamiento.          |

---

### Requisitos No Funcionales

| Código  | Requisito                                                         |
| ------- | ----------------------------------------------------------------- |
| RNF-001 | El sistema debe ser portable y cómodo para el usuario.            |
| RNF-002 | Los sensores deben estar ubicados de forma estable en el chaleco. |
| RNF-003 | El circuito debe tener bajo consumo de energía.                   |
| RNF-004 | El sistema debe ser seguro para el usuario.                       |
| RNF-005 | El diseño debe facilitar mantenimiento y revisión de componentes. |
| RNF-006 | El proyecto debe mantenerse dentro del presupuesto definido.      |

---

## 💰 Presupuesto y Recursos

Según la economía del proyecto, el presupuesto general de **TrackLogic** contempla personal, equipos, materiales, viajes, servicios técnicos y licencias de software.

**Costo total estimado del proyecto:** $13.635.000 COP
**Costo variable unitario:** $135.000 COP
**Precio de venta estimado:** $270.000 COP

---

## 🧩 Componentes Principales

* **Microcontrolador:** ESP32 Dev Module
* **Sensor biométrico:** MAX30102 / MAX30105
* **Sensor de movimiento:** MPU6050
* **Sensor de temperatura:** MLX90614
* **Interfaz:** Buzzer
* **Estructura:** Chaleco
* **Base de circuito:** PCB / baquela
* **Alimentación:** Batería por definir

---

## ⚠️ Gestión de Riesgos y Restricciones

| Riesgo                        | Descripción                                          | Mitigación                                                         |
| ----------------------------- | ---------------------------------------------------- | ------------------------------------------------------------------ |
| Retraso en componentes        | Algunos elementos pueden tardar en llegar.           | Verificar proveedores y hacer seguimiento temprano.                |
| Fallas en lectura de sensores | Los datos pueden ser inestables.                     | Realizar pruebas individuales antes de integrar todo.              |
| Diseño del chaleco            | Mala ubicación de sensores puede afectar mediciones. | Probar diferentes posiciones antes del montaje final.              |
| Energía                       | Batería no definida puede limitar la autonomía.      | Seleccionar batería adecuada para el consumo del ESP32 y sensores. |
| Organización del repositorio  | Archivos desordenados pueden afectar la entrega.     | Mantener GitHub actualizado y limpio.                              |
