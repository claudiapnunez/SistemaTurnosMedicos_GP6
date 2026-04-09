# Tarjeta CRC — Turno

| Campo | Detalle |
|---|---|
| **Nombre de la clase** | Turno |
| **Superclase** | — |
| **Subclase** | — |
| **Pensamiento del objeto** | "Soy un turno médico. Conozco mi fecha, hora, paciente y médico asignado. Puedo ser confirmado, cancelado o reprogramado." |

## Responsabilidades

| Responsabilidad | Colaboraciones |
|---|---|
| Conocer fecha y hora del turno | — |
| Conocer el paciente asignado | Paciente |
| Conocer el médico asignado | Medico |
| Conocer el tipo de consulta | — |
| Confirmar el turno | Notificacion |
| Cancelar el turno | Notificacion, Agenda |
| Reprogramar el turno a nueva fecha | Agenda, Notificacion |
| Conocer su estado actual (pendiente, confirmado, cancelado) | — |

## Propiedades

| Propiedad | Tipo |
|---|---|
| fecha | Date |
| hora | Time |
| paciente | Paciente |
| medico | Medico |
| tipoConsulta | String |
| estado | String |
