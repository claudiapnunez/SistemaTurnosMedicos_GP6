# Documentación de uso de IA — Especialista en Escenarios de Casos de Uso

## Prompt utilizado

```
Lee el archivo anexos/introduccion.md y la plantilla de escenarios de casos de uso como contexto.

Para cada uno de los 5 casos de uso del sistema de turnos médicos (Registrar turno, Consultar disponibilidad, Cancelar turno, Enviar notificación, Bloquear agenda), completá un escenario con todos los campos requeridos:
- Nombre del escenario y del caso de uso
- ID única (ESC-001 a ESC-005)
- Área del sistema
- Actores involucrados
- Descripción del caso de uso
- Evento activador y tipo de señal (externa o temporal)
- Pasos de la ruta principal (flujo normal)
- Precondiciones y poscondiciones
- Suposiciones
- Requerimientos que cubre
- Aspectos sobresalientes (preguntas abiertas)
- Prioridad y riesgo con justificación

Usá lenguaje natural, sin notación de código.
```

## Archivos de contexto referenciados

- `anexos/introduccion.md` — Requisitos funcionales y no funcionales del sistema.

## Ajustes realizados al output de la IA

1. Se corrigieron las precondiciones del escenario de Registrar Turno: la IA no incluía la condición de que el médico tenga agenda configurada.
2. Se ajustó el tipo de señal del escenario de Notificación: la IA lo marcó como "externa" cuando en realidad es "temporal" ya que lo dispara el sistema automáticamente.
3. Se revisaron los pasos de la ruta principal de Cancelar Turno para incluir la liberación del horario en la agenda, paso que la IA había omitido.
4. Se justificó el riesgo del escenario de Notificación como "Alto" en lugar de "Medio" que sugirió la IA, porque depende de un servicio externo (API de WhatsApp).
5. Se agregaron aspectos sobresalientes relevantes al dominio del consultorio que la IA no consideró, como políticas de cancelación y anticipación mínima.
