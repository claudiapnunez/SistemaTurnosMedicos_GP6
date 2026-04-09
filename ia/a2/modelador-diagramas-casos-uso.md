# Documentación de uso de IA — Modelador de Diagramas de Casos de Uso

## Prompt utilizado

```
Lee el archivo anexos/introduccion.md como contexto.

Generá el código PlantUML para 5 diagramas de casos de uso del sistema de gestión de turnos médicos, basándote en los requisitos funcionales RF1 a RF5. Cada diagrama debe incluir:
- Actores principales del sistema
- Casos de uso con relaciones de asociación
- Relaciones de inclusión (<<include>>) donde un caso de uso requiere otro obligatoriamente
- Relaciones de extensión (<<extend>>) donde un caso de uso es opcional

Los casos de uso son:
1. Registrar turno
2. Consultar turnos disponibles
3. Cancelar/Reprogramar turno
4. Enviar notificación por WhatsApp
5. Bloquear agenda por vacaciones

Usá la directiva left to right direction y skinparam packageStyle rectangle.
```

## Archivos de contexto referenciados

- `anexos/introduccion.md` — Requisitos funcionales que definen los casos de uso.

## Ajustes realizados al output de la IA

1. Se separó el caso de uso "Cancelar turno" y "Reprogramar turno" en un mismo diagrama pero como casos de uso distintos, ya que comparten el paso de buscar turno existente.
2. Se corrigió el diagrama de notificaciones: la IA había puesto al Paciente como actor que inicia el caso de uso, pero en realidad es el Sistema el que dispara la notificación automáticamente.
3. Se agregó la Secretaria como actor en el caso de uso de Bloquear Agenda, ya que en el dominio real es ella quien opera el sistema por indicación del médico.
4. Se ajustaron las relaciones include/extend: la IA había usado extend donde correspondía include (verificar disponibilidad es obligatorio al registrar turno, no opcional).
5. Se verificó que cada diagrama use el naming correcto para los archivos .puml según la consigna.
