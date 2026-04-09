# Tarjeta CRC — Agenda

| Campo | Detalle |
|---|---|
| **Nombre de la clase** | Agenda |
| **Superclase** | — |
| **Subclase** | — |
| **Pensamiento del objeto** | "Soy la agenda de un médico. Conozco los turnos disponibles y ocupados. Puedo bloquearme por vacaciones." |

## Responsabilidades

| Responsabilidad | Colaboraciones |
|---|---|
| Conocer los turnos registrados de un médico | Turno |
| Mostrar turnos disponibles según horario | Turno |
| Registrar un nuevo turno en un horario libre | Turno |
| Liberar un horario al cancelarse un turno | Turno |
| Bloquear un rango de fechas por vacaciones o ausencia | — |
| Verificar si un horario está disponible | — |

## Propiedades

| Propiedad | Tipo |
|---|---|
| medico | Medico |
| turnos | Lista de Turno |
| bloqueos | Lista de Bloqueo |
| horarioAtencion | HorarioAtencion |
