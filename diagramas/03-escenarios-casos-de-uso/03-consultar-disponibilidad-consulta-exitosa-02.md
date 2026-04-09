# Escenario de Caso de Uso

| Campo | Detalle |
|---|---|
| **Nombre del escenario** | Consulta exitosa de turnos disponibles |
| **Nombre del caso de uso** | Consultar turnos disponibles |
| **ID Única** | ESC-002 |
| **Área** | Gestión de Turnos |
| **Actor(es)** | Secretaria |
| **Descripción** | La secretaria consulta los horarios disponibles de un médico para ofrecer opciones al paciente que solicita turno. |
| **Activar Evento** | Un paciente solicita conocer los horarios disponibles. |
| **Tipo de señal** | Externa — iniciada por el paciente a través de la secretaria. |

## Pasos desempeñados (ruta principal)

1. La secretaria accede al módulo de consulta de turnos.
2. La secretaria selecciona la especialidad médica.
3. El sistema muestra los médicos disponibles para esa especialidad.
4. La secretaria selecciona un médico.
5. El sistema consulta la agenda del médico.
6. El sistema muestra los horarios libres de los próximos días.
7. La secretaria comunica las opciones al paciente.

| Campo | Detalle |
|---|---|
| **Precondiciones** | El médico debe tener una agenda configurada. Debe existir al menos un médico para la especialidad solicitada. |
| **Poscondiciones** | Se muestra al usuario la lista de horarios disponibles. No se modifica ningún dato del sistema. |
| **Suposiciones** | La agenda del médico está actualizada y refleja los bloqueos vigentes. |
| **Reunir requerimientos** | RF2 — El sistema debe mostrar turnos disponibles según horario configurado. |
| **Aspectos sobresalientes** | ¿Con cuántos días de anticipación se muestran los turnos? ¿Se muestra disponibilidad de varios médicos a la vez? |
| **Prioridad** | Alta |
| **Riesgo** | Bajo — Es una consulta de lectura sin modificación de datos. |
