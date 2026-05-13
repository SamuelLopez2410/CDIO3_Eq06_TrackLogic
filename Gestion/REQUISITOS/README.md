# 📋 Requisitos del Sistema

Este directorio contiene la documentación oficial de requisitos funcionales y no funcionales del sistema de monitoreo biomédico orientado al seguimiento fisiológico de atletas durante sesiones de entrenamiento.

Los requisitos definidos establecen el comportamiento esperado del sistema, las capacidades principales de monitoreo y las restricciones técnicas necesarias para garantizar un funcionamiento confiable, seguro y eficiente.

Toda la especificación fue estructurada siguiendo criterios de análisis de sistemas y desarrollo de software, permitiendo que cada funcionalidad pueda ser validada durante las etapas de diseño, implementación y pruebas.

---

# 📊 Documento Oficial: Especificación de Requisitos

## 📌 Resumen Ejecutivo de Requisitos (Fase Actual)

A continuación, se presentan los principales requisitos identificados para el desarrollo del sistema:

| ID     | Tipo         | Descripción General                                        | Estado     |
| ------ | ------------ | ---------------------------------------------------------- | ---------- |
| RF-01  | Funcional    | Medición y registro de variables fisiológicas del atleta   | ✅ DEFINIDO |
| RF-02  | Funcional    | Generación automática de alertas ante sobrecarga física    | ✅ DEFINIDO |
| RF-03  | Funcional    | Personalización de entrenamientos según datos recolectados | ✅ DEFINIDO |
| RNF-01 | No Funcional | Interfaz simple, adaptable y fácil de usar                 | ✅ DEFINIDO |
| RNF-02 | No Funcional | Actualización de variables fisiológicas en tiempo real     | ✅ DEFINIDO |
| RNF-03 | No Funcional | Protección y cifrado de datos de salud                     | ✅ DEFINIDO |

---

# ⚙️ Metodología de Definición de Requisitos (Definition of Done)

Para que un requisito sea considerado válido y aprobado dentro del proyecto, debe cumplir con los siguientes criterios:

---

## 1️⃣ Claridad y Cero Ambigüedad

Cada requisito debe describir de forma precisa:

* Qué debe hacer el sistema
* Cómo debe comportarse
* Qué restricciones debe cumplir

No se aceptan descripciones subjetivas como:

* “El sistema debe ser bueno”
* “La aplicación debe ser rápida”
* “La interfaz debe verse moderna”

Todos los requisitos deben poder:

* Medirse
* Verificarse
* Probarse durante validación

---

## 2️⃣ Requisitos Verificables

Cada funcionalidad definida debe poder comprobarse mediante:

* Pruebas funcionales
* Datos medibles
* Validaciones de software o hardware
* Resultados observables en el sistema

Ejemplos:

* Tiempo de actualización ≤ 2 segundos
* Generación automática de alertas
* Visualización correcta de datos fisiológicos

---

## 3️⃣ Relación con el Objetivo del Proyecto

Todos los requisitos definidos están orientados a:

* Mejorar el monitoreo del atleta
* Detectar condiciones de riesgo físico
* Facilitar el análisis del entrenamiento
* Garantizar seguridad y accesibilidad de la información

Esto asegura coherencia entre:

* Problema planteado
* Diseño del sistema
* Desarrollo tecnológico
* Validación final

---

# 🧩 Observación Técnica del Sistema

La definición de requisitos permitió establecer una base estructurada para el desarrollo del proyecto, facilitando:

* La integración de sensores biomédicos
* El diseño del firmware en ESP32
* La implementación de alertas inteligentes
* El desarrollo futuro de una interfaz web o móvil

Además, los requisitos no funcionales garantizan que el sistema no solo sea técnicamente operativo, sino también accesible, seguro y adaptable a escenarios reales de entrenamiento deportivo.
