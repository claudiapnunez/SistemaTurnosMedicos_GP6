# Escenario de Caso de Uso

| Campo | Detalle |
|---|---|
| **Nombre del escenario** | Cancelación exitosa de turno médico |
| **Nombre del caso de uso** | Cancelar turno |
| **ID Única** | ESC-003 |
| **Área** | Gestión de Turnos |
| **Actor(es)** | Secretaria, Paciente |
| **Descripción** | El paciente solicita cancelar un turno previamente registrado. La secretaria lo busca en el sistema, lo cancela y el sistema envía una notificación al paciente. |
| **Activar Evento** | El paciente se comunica para cancelar su turno. |
| **Tipo de señal** | Externa — iniciada por el paciente. |

## Pasos desempeñados (ruta principal)

1. El paciente se comunica con el consultorio solicitando cancelar su turno.
2. La secretaria ingresa al módulo de gestión de turnos.
3. La secretaria busca el turno por nombre del paciente o fecha.
4. El sistema muestra los datos del turno encontrado.
5. La secretaria confirma la cancelación del turno.
6. El sistema cambia el estado del turno a "cancelado".
7. El sistema libera el horario en la agenda del médico.
8. El sistema envía una notificación de cancelación al paciente por WhatsApp.

| Campo | Detalle |
|---|---|
| **Precondiciones** | El turno debe existir en el sistema con estado "confirmado". |
| **Poscondiciones** | El turno queda con estado "cancelado". El horario se libera en la agenda. El paciente recibe notificación de cancelación. |
| **Suposiciones** | La cancelación se realiza con al menos 24 horas de anticipación. El paciente tiene WhatsApp activo. |
| **Reunir requerimientos** | RF3, RF4 — El sistema debe permitir cancelar turnos y notificar al paciente. |
| **Aspectos sobresalientes** | ¿Existe una política de cancelación con tiempo mínimo? ¿Se penaliza al paciente por cancelaciones reiteradas? |
| **Prioridad** | Alta |
| **Riesgo** | Bajo — Operación directa sin dependencias externas complejas. |
