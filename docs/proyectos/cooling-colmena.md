# 🐝 Sistema de Control Térmico para Colmena

**Estado:** ✅ Funcional en terreno  
**Fecha:** [06/2026]  
**Tecnologías:** ESP8266, DHT22, Relé, Python

---

## 📋 Descripción

Sistema automatizado de control de temperatura y humedad para colmenas, implementando un **lazo de control cerrado** que activa/desactiva ventilación según parámetros predefinidos.

---

## 🎯 Objetivo

Mantener condiciones óptimas (28-32°C, <70% HR) dentro de la colmena para proteger la colonia y maximizar la producción.

---

## ⚙️ Especificaciones Técnicas

### Hardware
| Componente | Modelo | Especificación |
|------------|--------|----------------|
| Controlador | NodeMCU ESP8266 | 3.3V, WiFi 802.11 b/g/n |
| Sensor | DHT22 | -40 a 80°C, ±0.5°C |
| Actuador | Relé 5V 1 canal | 10A @ 250VAC |
| Ventilador | Cooler 5V 80mm | 0.15A |
| Alimentación | Batería 5V 2000mAh | Autonomía ~40h |

### Diagrama de Bloques





---

## 📊 Resultados

| Métrica | Valor |
|---------|-------|
| Temp. máxima ambiente | 35°C |
| Temp. máxima en colmena | 31°C |
| **Reducción lograda** | **4°C** ✅ |
| Humedad promedio | 65% |
| Ciclos/día | 8-12 activaciones |

---

## 🔧 Desafíos y Soluciones

1. **Ruido eléctrico del ventilador**  
   → Separación de fuentes + capacitor 100µF

2. **Condensación en sensor**  
   → Ubicación fuera del flujo directo de aire

3. **Autonomía de batería**  
   → Implementación de deep sleep (pendiente)

---

## 📎 Recursos

- [Código fuente en GitHub](https://github.com/Bl4ckj4ck84/colmena-cooling)
- [Diagrama esquemático](https://github.com/Bl4ckj4ck/colmena-cooling/blob/main/schematic.png)
- [Video de funcionamiento](https://youtu.be/tu-video)
