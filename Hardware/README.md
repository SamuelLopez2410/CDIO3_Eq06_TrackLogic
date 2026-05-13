## 🔧 **Diseño de Hardware - TrackLogic**

Este directorio documenta la **arquitectura electrónica**, el **diseño de PCB** y la **integración física** del sistema **TrackLogic**. El hardware está diseñado para ser **portable**, **cómodo** y **adaptable a un chaleco inteligente**, garantizando estabilidad en la medición de **datos biométricos** y **de movimiento**.

---

## 📐 **Vista General del Dispositivo**

El sistema se compone de una **PCB personalizada** donde se integran los **sensores** y el **microcontrolador**, la cual se instala sobre el **chaleco** para su uso en el cuerpo del usuario.

---

## 📏 **Especificaciones Físicas**

* **Tipo de PCB:** Baquela / PCB personalizada
* **Montaje:** Integrado en chaleco
* **Peso:** Ligero y portable
* **Distribución:** Sensores ubicados estratégicamente para mejorar la precisión

---

## ⚡ **Arquitectura del Sistema**

El sistema utiliza una arquitectura basada en **comunicación I2C**, donde todos los sensores se conectan al **ESP32**:

* **ESP32:** Control principal
* **MPU6050:** Movimiento (aceleración y giroscopio)
* **MAX30102:** Señales biométricas (frecuencia cardíaca y oxígeno)
* **MLX90614:** Temperatura sin contacto
* **ADS1115:** Conversión analógica-digital para mejorar precisión
* **Buzzer:** Salida de alertas sonoras

👉 Esta arquitectura permite:

* **Lectura eficiente de múltiples sensores** sin interferencia.
* **Integración sencilla** de componentes y cables.
* **Bajo consumo de energía**, optimizado para funcionamiento continuo.

---

### **Conclusión Final**

El diseño de hardware para **TrackLogic** ya está **completamente funcional**, con todos los sensores integrados y operando de forma estable. El sistema está listo para pruebas finales y su implementación completa.
