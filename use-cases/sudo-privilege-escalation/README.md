# 🛡️ Privilege Escalation Detection (sudo)

## 📌 Descripción

Se simuló el uso de privilegios elevados mediante el comando `sudo` en un endpoint Kali Linux monitoreado por Wazuh.

---

## ⚙️ Configuración

- Endpoint: Kali Linux (agente Wazuh)
- SIEM: Wazuh Manager
- Logs: journald

---

## 💣 Simulación

Se ejecutaron comandos con privilegios elevados:

```bash
sudo ls /root
sudo cat /etc/shadow
```

📊 Resultado en Wazuh

El sistema detectó eventos relacionados con el uso de sudo:

Ejecución de comandos como root
Acceso a recursos críticos

🔍 Ejemplo de evento
```bash
data.command: /usr/bin/cat /etc/shadow
data.srcuser: kali
data.dstuser: root
rule.level: 10
```

🧠 Análisis SOC

El uso de sudo para acceder a archivos sensibles como /etc/shadow puede indicar:

Escalamiento de privilegios
Actividad sospechosa o maliciosa
Movimiento lateral o post-explotación

🚨 Impacto
Exposición de credenciales
Compromiso total del sistema

🛡️ Recomendaciones
Restringir uso de sudo
Monitorear comandos críticos
Implementar alertas personalizadas

---
