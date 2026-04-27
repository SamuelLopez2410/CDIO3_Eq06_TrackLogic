# 🧪 Protocolos de Prueba y Validación (Test Reports)

Este directorio contiene los reportes oficiales de pruebas ejecutadas para el sistema basado en **ESP32 y sensores biomédicos**, encargado de la adquisición y transmisión de datos fisiológicos.

Todas las validaciones siguen criterios técnicos definidos previamente, asegurando que los resultados se basen en **parámetros medibles y verificables**, eliminando la subjetividad en la evaluación del sistema.

---

# 📊 Documento Oficial: Protocolo de Pruebas

## 📌 Resumen Ejecutivo de Pruebas (Fase Actual)

A continuación, se presenta el estado de los últimos test de integración correspondientes a la etapa de validación funcional del sistema (Conectividad, Sensores y Alertas).

| ID Prueba | Subsistema            | Objetivo Principal                                                      | Resultado Medido                                 | Estado |
| --------- | --------------------- | ----------------------------------------------------------------------- | ------------------------------------------------ | ------ |
| IT-001    | Conectividad WIFI     | Verificar conexión de la ESP32 a la red local para transmisión de datos | Asignación correcta de IP local en monitor serie | ✅ PASS |
| IT-002    | Comunicación Telegram | Validar respuesta del BOT ante comandos enviados desde Telegram         | BOT responde correctamente al comando **/START** | ✅ PASS |
| IT-003    | Sensor MAX30105       | Validar lectura estable de ritmo cardíaco (BPM) en bus I2C principal    | Sistema muestra promedio BPM estable             | ✅ PASS |
| IT-004    | Sensor MAX30102       | Detectar proximidad mediante lectura IR en bus I2C secundario           | Cambio de estado a **"Objeto detectado"**        | ✅ PASS |
| IT-005    | Termómetro MLX90614   | Medir temperatura corporal sin contacto                                 | Lectura mayor a temperatura ambiente (~36°C)     | ✅ PASS |
| IT-006    | Acelerómetro MPU6050  | Detectar movimiento e inclinación del sistema                           | Variación de valores según inclinación           | ✅ PASS |
| IT-007    | Lógicas de Alertas    | Activar buzzer ante parámetros fisiológicos críticos                    | Emisión de sonido intermitente del buzzer        | ✅ PASS |

---

# ⚙️ Metodología de Validación (Definition of Done)

Para que una prueba sea marcada como **✅ PASS** y el componente pase a la etapa final de validación, debe cumplir estrictamente con los siguientes pilares:

---

## 1️⃣ Cero Subjetividad

No se aceptan descripciones ambiguas como:

* "Funcionó bien"
* "Respondió rápido"
* "Se escuchó fuerte"

Cada prueba debe generar:

* Valores medibles
* Respuestas verificables
* Evidencia observable

Ejemplos válidos:

* Dirección IP asignada
* Lectura BPM estable
* Temperatura mayor a 36°C
* Activación sonora del buzzer

---

## 2️⃣ Setup Documentado

Cada prueba fue ejecutada bajo condiciones definidas previamente, incluyendo:

* ESP32 energizado correctamente
* Sensores conectados en buses I2C definidos
* Monitor serie activo a **115200 baudios**
* Red WIFI disponible
* BOT de Telegram configurado
* Buzzer conectado en GPIO 26

Esto garantiza que las pruebas puedan ser:

* Repetidas
* Verificadas
* Auditadas

---

## 3️⃣ Criterios de Aceptación Predefinidos

Antes de ejecutar cada prueba, se definió un **resultado esperado**, basado en:

* Datasheets de sensores
* Configuración del firmware
* Umbrales fisiológicos programados
* Respuestas lógicas del sistema

Ejemplos:

* BPM detectado correctamente
* Temperatura corporal mayor a ambiente
* Respuesta automática del BOT
* Activación del buzzer ante valores críticos

Solo si estos criterios se cumplen, la prueba se clasifica como:

✅ **PASS**

---

# 🧩 Observación Técnica del Sistema

Durante la fase actual de validación, el sistema demostró:

* Integración funcional entre sensores biomédicos
* Comunicación estable vía WIFI
* Interacción correcta con Telegram
* Respuesta automática ante eventos críticos
* Funcionamiento adecuado del sistema de alertas

Esto confirma que el sistema se encuentra en una **fase funcional estable**, apta para continuar hacia pruebas de integración avanzada o pruebas en entorno real.
