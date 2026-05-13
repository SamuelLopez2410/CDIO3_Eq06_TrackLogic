# 🚀 **TrackLogic: Sistema de Monitoreo Biométrico y de Movimiento**

**Status:** Completado y Funcional
**Platform:** ESP32
**License:** Académico

**TrackLogic** es un sistema embebido diseñado para la **adquisición, análisis y registro de datos biométricos y de movimiento del usuario**. El sistema permite monitorear variables fisiológicas y cinemáticas en tiempo real, integrando múltiples sensores en una **arquitectura compacta y portable**.

---

## 🎯 **Objetivo del Proyecto**

Desarrollar un **dispositivo de bajo costo**, **portátil** y **adaptable a un chaleco inteligente**, capaz de medir:

* **Frecuencia cardíaca:** mediante sensores ópticos (**MAX30102 / MAX30105**)
* **Movimiento corporal:** usando **IMU (MPU6050)**
* **Temperatura corporal:** mediante sensor infrarrojo (**MLX90614**)
* **Actividad física:** análisis de aceleración y orientación
* **Registro de datos:** almacenamiento para análisis posterior

---

## 🛠️ **Hardware y Arquitectura**

El sistema funciona como una plataforma de **adquisición de datos**, donde el **microcontrolador central** procesa la información de los **sensores** y la transmite o almacena para su análisis.

### 🔹 **Lista de Componentes (BOM)**

* **MCU:** ESP32 Dev Module
* **Sensor IMU:** MPU6050 (acelerómetro + giroscopio)
* **Sensores biométricos:** MAX30102 / MAX30105
* **Sensor de temperatura:** MLX90614
* **Interfaz:** Buzzer (alertas)
* **Energía:** Batería (por definir)
* **Estructura:** Chaleco inteligente

---

## 📊 **Diagrama de Bloques**

```
[MAX30102 / MAX30105] ──┐
[MPU6050] ──────────────┼──> [ESP32] ───> [Procesamiento de datos]
[MLX90614] ─────────────┘

[ESP32] ───> [Almacenamiento / Visualización]
[ESP32] ───> [Salida (Buzzer / Alertas)]
```

---

## ⚙️ **Funcionalidades Clave**

### 1. 📡 **Adquisición de datos en tiempo real**

El sistema permite la **lectura simultánea** de múltiples sensores para obtener información biométrica y de movimiento del usuario.

---

### 2. 🧠 **Análisis de movimiento**

El sensor **MPU6050** permite calcular:

* Aceleración en los ejes **X, Y, Z**
* Inclinación y orientación del cuerpo
* Cambios de movimiento

---

### 3. ❤️ **Monitoreo biométrico**

Los sensores **MAX30102** y **MAX30105** permiten medir señales relacionadas con la **frecuencia cardíaca**, útiles para analizar el estado físico del usuario.

---

### 4. 🌡️ **Medición de temperatura**

El sensor **MLX90614** permite medir **temperatura sin contacto**, lo cual es útil para monitoreo continuo.

---

### 5. 🔔 **Sistema de alertas**

El **buzzer** permite generar alertas sonoras dependiendo del estado del sistema o de los valores medidos.

---

## 🚀 **Instalación y Uso**

### 🔹 **Firmware (ESP32)**

1. Clonar el repositorio
2. Abrir en **Arduino IDE** o **VS Code**
3. Instalar librerías necesarias:

   * **Wire**
   * **Adafruit MPU6050**
   * **Adafruit MAX30102**
   * **Adafruit MLX90614**
4. Cargar el código al **ESP32**

---

### 🔹 **Pruebas del sistema**

1. Conectar sensores al **ESP32**
2. Encender el sistema
3. Verificar lectura de datos en monitor serial
4. Validar comportamiento de sensores

---

## 📌 **Estado Actual**

El proyecto **TrackLogic** se encuentra **totalmente funcional** y en fase de **pruebas completas**. Las siguientes actividades están **completadas**:

* **Integración de sensores**
* **Programación del ESP32**
* **Definición del sistema de energía**
* **Diseño mecánico del chaleco**
* **Pruebas de validación**
* **Documentación final y sustentación preparadas**
