### 🧠 Resumen del Proyecto HoneyPot Avanzado
### 🎯 Objetivo:
Capturar y analizar intentos de intrusión en un honeypot, impedir que el atacante borre logs, bloquear automáticamente la IP atacante, analizar el ataque y notificar por correo electrónico con nivel de riesgo.

### 🧱 Arquitectura del Proyecto
- **Honeypot (Suricata o Cowrie)** 

*Simula servicios vulnerables*

 *Captura tráfico de red sospechoso*

 *Guarda logs de forma segura*

- **Protección de logs**

*Logs almacenados con permisos estrictos*

*Posiblemente logs en tiempo real a servidor externo o sistema SIEM*

- **Sistema de detección (IDS)**

Suricata con reglas personalizadas

Detección de patrones y alertas

- **Firewall (UFW/IPTables)**

Script automático para bloquear IPs que atacan

- **Consulta de base externa**

(Simulado o real) API que clasifique la herramienta del atacante y devuelva un riesgo

- **Sistema de notificación**

Envío de correo con ssmtp o mailx

Incluye: herramienta usada, IP, nivel de riesgo

### 🔧 Tecnologías usadas
- **Docker**	-->        Aislamiento de servicios del honeypot
- **Suricata**	  -->     Detección de intrusos (IDS)
- **IPTables**	 -->      Bloqueo automático de IPs
- **Python/Bash**  -->   Scripts de automatización
- **Cron**	   -->        Automatización periódica si es necesario
- **Mailx/ssmtp**	 -->    Notificaciones por correo
- **Ubuntu**	   -->      Sistema base
- **Git**	    -->        Control de versiones y entrega


### 📦 Fases del Proyecto
 1. Montar el honeypot con Suricata o Cowrie.
 2. Asegurar los logs (root-only, logs externos o chattr +i).
 3. Crear un script que lea logs y detecte IPs maliciosas.
 4. Bloquear automáticamente esas IPs.
 5. Simular o consultar base de datos de amenazas.
 6. Enviar un correo con la info del ataque.








 Documentar absolutamente todo.

