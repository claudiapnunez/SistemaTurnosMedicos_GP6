# Escenario de Caso de Uso

| Campo | Detalle |
|---|---|
| **Nombre del escenario** | Registro exitoso de turno médico |
| **Nombre del caso de uso** | Registrar turno |
| **ID Única** | ESC-001 |
| **Área** | Gestión de Turnos |
| **Actor(es)** | Secretaria, Paciente |
| **Descripción** | El paciente solicita un turno y la secretaria lo registra en el sistema seleccionando médico, fecha y hora disponibles. El sistema confirma el turno y envía una notificación al paciente. |
| **Activar Evento** | El paciente se comunica con el consultorio para solicitar un turno. |
| **Tipo de señal** | Externa — iniciada por el paciente. |

## Pasos desempeñados (ruta principal)

1. El paciente solicita un turno indicando especialidad y preferencia de fecha.
2. La secretaria ingresa al módulo de turnos del sistema.
3. La secretaria selecciona el médico según la especialidad solicitada.
4. El sistema muestra los horarios disponibles del médico.
5. La secretaria selecciona fecha y hora.
6. La secretaria ingresa los datos del paciente.
7. El sistema verifica que no haya superposición de turnos.
8. El sistema registra el turno con estado "confirmado".
9. El sistema envía una notificación de confirmación al paciente por WhatsApp.

| Campo | Detalle |
|---|---|
| **Precondiciones** | El médico debe tener agenda configurada con horarios disponibles. El paciente debe estar registrado o se registra en el momento. |
| **Poscondiciones** | El turno queda registrado en la agenda del médico con estado "confirmado". El paciente recibe la notificación de confirmación. |
| **Suposiciones** | El paciente cuenta con un número de WhatsApp válido. La agenda del médico no está bloqueada en la fecha solicitada. |
| **Reunir requerimientos** | RF1, RF2, RF4 — El sistema debe registrar turnos, mostrar disponibilidad y enviar notificación. |
| **Aspectos sobresalientes** | ¿Qué sucede si el paciente no tiene WhatsApp? ¿Se permite registrar turnos para el mismo día? |
| **Prioridad** | Alta |
| **Riesgo** | Medio — Depende de la integración con el servicio de WhatsApp. |
