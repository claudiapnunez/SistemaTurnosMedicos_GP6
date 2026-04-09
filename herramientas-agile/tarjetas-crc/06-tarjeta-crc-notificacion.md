# Tarjeta CRC — Notificacion

| Campo | Detalle |
|---|---|
| **Nombre de la clase** | Notificacion |
| **Superclase** | — |
| **Subclase** | — |
| **Pensamiento del objeto** | "Soy una notificación que informa al paciente sobre el estado de su turno. Puedo enviarse por WhatsApp." |

## Responsabilidades

| Responsabilidad | Colaboraciones |
|---|---|
| Conocer el destinatario de la notificación | Paciente |
| Conocer el mensaje a enviar | — |
| Conocer el canal de envío (WhatsApp) | — |
| Enviar notificación de confirmación de turno | Turno, Paciente |
| Enviar notificación de cancelación de turno | Turno, Paciente |
| Enviar recordatorio de turno próximo | Turno, Paciente |

## Propiedades

| Propiedad | Tipo |
|---|---|
| destinatario | Paciente |
| mensaje | String |
| canal | String |
| fechaEnvio | Date |
| estado | String |
