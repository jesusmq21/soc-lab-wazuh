![SOC Lab](screenshots/cover.png)

# 🛡️ Laboratorio SOC – Wazuh SIEM

## 🚀 Descripción

Laboratorio práctico de un Centro de Operaciones de Seguridad (SOC) utilizando Wazuh como SIEM, enfocado en la simulación de ataques reales, detección de amenazas y análisis de logs.

Este proyecto demuestra habilidades de nivel SOC 1 mediante la simulación de ataques, detección de eventos y creación de reglas personalizadas.

---

## ⚙️ Arquitectura

- 🖥️ Wazuh Manager (Ubuntu Server)
- 💻 Endpoint monitoreado: Kali Linux
- 🔗 Recolección de logs mediante agente Wazuh
- 📊 Análisis desde Wazuh Dashboard

---

## 🧪 Casos de uso implementados

### 🔓 Fuerza bruta SSH
Simulación de múltiples intentos fallidos de autenticación para detectar ataques de fuerza bruta.

### 🛡️ Escalamiento de privilegios (sudo)
Detección del uso de privilegios elevados y acceso a recursos críticos del sistema.

### 🚨 Reglas personalizadas
Creación de reglas en Wazuh para mejorar la detección de eventos críticos:

- 🔴 Acceso a `/etc/shadow` → Nivel 12 (Crítico)
- 🟠 Acceso a `/root` → Nivel 10 (Alto)

---

## 📊 Flujo de detección

1. Simulación de ataque desde Kali Linux  
2. Recolección de logs mediante el agente  
3. Procesamiento en Wazuh Manager  
4. Generación de alertas  
5. Análisis en el dashboard  

---

## 🧠 Habilidades demostradas

- Operación de SIEM (Wazuh)
- Análisis de logs
- Detección de amenazas
- Investigación de incidentes (SOC Nivel 1)
- Creación y ajuste de reglas (Rule Tuning)
- Monitoreo de seguridad en Linux
- Resolución de problemas (Troubleshooting)

---

## 📸 Evidencia

Las capturas de los ataques y detecciones están disponibles en:

/screenshots.


---

## 🎯 Logros

- Simulación de escenarios reales de ataque
- Detección de fuerza bruta y escalamiento de privilegios
- Implementación de reglas personalizadas
- Aumento de severidad en eventos críticos
- Construcción de un laboratorio SOC funcional

---

## 🚀 Conclusión

Este laboratorio refleja el flujo de trabajo real de un analista SOC, incluyendo monitoreo, detección, análisis y mejora continua de reglas.

---

## 👨‍💻 Autor

**Jesús Eduardo Machuca**  
Aspirante a Analista SOC | Entusiasta de la Ciberseguridad

![SIEM](https://img.shields.io/badge/SIEM-Wazuh-blue)
![Nivel](https://img.shields.io/badge/Nivel-SOC%20L1-green)
![Estado](https://img.shields.io/badge/Estado-Completado-brightgreen)
