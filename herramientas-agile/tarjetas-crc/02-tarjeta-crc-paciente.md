# Tarjeta CRC — Paciente

| Campo | Detalle |
|---|---|
| **Nombre de la clase** | Paciente |
| **Superclase** | Persona |
| **Subclase** | — |
| **Pensamiento del objeto** | "Soy un paciente que solicita turnos médicos. Conozco mi obra social y mi historial de turnos." |

## Responsabilidades

| Responsabilidad | Colaboraciones |
|---|---|
| Conocer obra social | — |
| Solicitar un turno nuevo | Turno, Agenda |
| Cancelar un turno existente | Turno |
| Conocer su historial de turnos | Turno |
| Recibir notificaciones sobre sus turnos | Notificacion |

## Propiedades

| Propiedad | Tipo |
|---|---|
| obraSocial | String |
| historialTurnos | Lista de Turno |
