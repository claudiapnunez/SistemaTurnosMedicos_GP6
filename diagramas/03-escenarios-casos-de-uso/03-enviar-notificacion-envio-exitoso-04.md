# Escenario de Caso de Uso

| Campo | Detalle |
|---|---|
| **Nombre del escenario** | Envío exitoso de notificación por WhatsApp |
| **Nombre del caso de uso** | Enviar notificación por WhatsApp |
| **ID Única** | ESC-004 |
| **Área** | Notificaciones |
| **Actor(es)** | Sistema (automático), Paciente |
| **Descripción** | El sistema genera y envía automáticamente una notificación al paciente por WhatsApp luego de registrar, cancelar o reprogramar un turno. |
| **Activar Evento** | Se registra, cancela o reprograma un turno en el sistema. |
| **Tipo de señal** | Temporal — disparada automáticamente por un evento interno del sistema. |

## Pasos desempeñados (ruta principal)

1. El sistema detecta un cambio de estado en un turno (nuevo, cancelado o reprogramado).
2. El sistema identifica al paciente asociado al turno.
3. El sistema obtiene el número de WhatsApp del paciente.
4. El sistema genera el mensaje correspondiente según el tipo de evento.
5. El sistema envía el mensaje por WhatsApp.
6. El sistema registra el estado del envío (enviado/fallido).

| Campo | Detalle |
|---|---|
| **Precondiciones** | El paciente debe tener un número de WhatsApp válido registrado. El turno debe haber cambiado de estado. |
| **Poscondiciones** | La notificación queda registrada con estado "enviado". El paciente recibe el mensaje en su WhatsApp. |
| **Suposiciones** | El servicio de mensajería de WhatsApp está operativo. El número del paciente es correcto y tiene WhatsApp activo. |
| **Reunir requerimientos** | RF4 — El sistema debe enviar notificaciones automáticas al paciente por WhatsApp. |
| **Aspectos sobresalientes** | ¿Qué sucede si el envío falla? ¿Se reintenta? ¿Existe un canal alternativo (SMS, email)? |
| **Prioridad** | Media |
| **Riesgo** | Alto — Depende de un servicio externo (API de WhatsApp) que puede no estar disponible. |
