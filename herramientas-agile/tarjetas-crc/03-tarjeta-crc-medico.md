# Tarjeta CRC — Medico

| Campo | Detalle |
|---|---|
| **Nombre de la clase** | Medico |
| **Superclase** | Persona |
| **Subclase** | — |
| **Pensamiento del objeto** | "Soy un médico del consultorio. Conozco mi especialidad, gestiono mi agenda y atiendo turnos." |

## Responsabilidades

| Responsabilidad | Colaboraciones |
|---|---|
| Conocer especialidad médica | — |
| Conocer matrícula profesional | — |
| Gestionar su agenda de turnos | Agenda |
| Bloquear agenda por vacaciones o ausencias | Agenda |
| Consultar turnos asignados del día | Turno, Agenda |

## Propiedades

| Propiedad | Tipo |
|---|---|
| especialidad | String |
| matricula | String |
| agenda | Agenda |
