# Escenario de Caso de Uso

| Campo | Detalle |
|---|---|
| **Nombre del escenario** | Bloqueo exitoso de agenda por vacaciones |
| **Nombre del caso de uso** | Bloquear agenda por vacaciones |
| **ID Única** | ESC-005 |
| **Área** | Gestión de Agenda |
| **Actor(es)** | Médico, Secretaria |
| **Descripción** | El médico solicita bloquear su agenda para un período de vacaciones. La secretaria registra el bloqueo en el sistema, lo que impide agendar turnos en esas fechas y notifica a los pacientes afectados. |
| **Activar Evento** | El médico informa que tomará vacaciones en un período determinado. |
| **Tipo de señal** | Externa — iniciada por el médico. |

## Pasos desempeñados (ruta principal)

1. El médico comunica a la secretaria las fechas de sus vacaciones.
2. La secretaria ingresa al módulo de gestión de agenda.
3. La secretaria selecciona al médico correspondiente.
4. La secretaria ingresa la fecha de inicio y fin del bloqueo.
5. El sistema verifica si existen turnos ya registrados en ese período.
6. El sistema muestra los turnos afectados (si los hay).
7. La secretaria confirma el bloqueo.
8. El sistema bloquea la agenda para el rango de fechas indicado.
9. El sistema notifica a los pacientes con turnos afectados por WhatsApp.

| Campo | Detalle |
|---|---|
| **Precondiciones** | El médico debe tener una agenda configurada en el sistema. Las fechas de bloqueo deben ser futuras. |
| **Poscondiciones** | La agenda del médico queda bloqueada para el período indicado. No se pueden registrar nuevos turnos en esas fechas. Los pacientes afectados fueron notificados. |
| **Suposiciones** | Los turnos afectados se cancelan o reprograman antes del bloqueo. El médico informa con anticipación suficiente. |
| **Reunir requerimientos** | RF5, RF4 — El sistema debe bloquear agenda por vacaciones y notificar a los pacientes afectados. |
| **Aspectos sobresalientes** | ¿Se reprograman automáticamente los turnos afectados o solo se cancelan? ¿Con cuánta anticipación mínima se puede bloquear la agenda? |
| **Prioridad** | Media |
| **Riesgo** | Medio — Requiere gestionar turnos existentes en el período bloqueado. |
