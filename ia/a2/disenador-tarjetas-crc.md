# Documentación de uso de IA — Diseñador de Tarjetas CRC

## Prompt utilizado

```
Lee los archivos anexos/introduccion.md y diagramas/01-diagrama-clases/01-boceto-inicial.excalidraw como contexto.

Identificá las clases principales del sistema de gestión de turnos médicos y generá una tarjeta CRC para cada una, siguiendo esta estructura:
- Nombre de la clase
- Superclase (si aplica herencia)
- Subclase (si aplica herencia)
- Pensamiento del objeto (en primera persona, describiendo qué es y qué sabe)
- Responsabilidades principales (qué hace la clase, con qué clases colabora)
- Propiedades (atributos con su tipo)

Las clases deben reflejar el dominio del consultorio médico: turnos, pacientes, médicos, agenda, notificaciones. Usá lenguaje natural, no notación de código.
```

## Archivos de contexto referenciados

- `anexos/introduccion.md` — Descripción del sistema, requisitos funcionales y no funcionales.
- `diagramas/01-diagrama-clases/01-boceto-inicial.excalidraw` — Boceto inicial del diagrama de clases.

## Ajustes realizados al output de la IA

1. Se revisaron las responsabilidades de cada clase para asegurar coherencia con los requisitos funcionales (RF1 a RF5).
2. Se agregó la clase Notificacion que la IA no había incluido inicialmente, necesaria para cubrir el RF4 (notificaciones por WhatsApp).
3. Se corrigió el pensamiento del objeto de la clase Agenda para reflejar que también gestiona bloqueos por vacaciones (RF5).
4. Se eliminó notación de código en las responsabilidades, reemplazando por lenguaje natural según la corrección del docente en la Actividad N°1.
5. Se verificó que las colaboraciones entre clases sean bidireccionales donde corresponde (ej: Turno colabora con Agenda y viceversa).
