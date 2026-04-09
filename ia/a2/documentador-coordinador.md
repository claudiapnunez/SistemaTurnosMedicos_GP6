# Documentación de uso de IA — Documentador y Coordinador de Repositorio

## Code Review 1 — PR del Diseñador de Tarjetas CRC

### Prompt utilizado

```
Lee el archivo anexos/introduccion.md como contexto. Revisá los archivos de la carpeta herramientas-agile/tarjetas-crc/ y verificá:
1. Que cada tarjeta CRC corresponda a una clase del boceto de clases de la Actividad N°1.
2. Que los campos estén completos: nombre, superclase/subclase, pensamiento del objeto, responsabilidades, colaboraciones y propiedades.
3. Que las responsabilidades sean coherentes con los requisitos funcionales RF1 a RF5.
4. Que no se use notación de código sino lenguaje natural.
```

### Observaciones y ajustes
- Se verificó que las 6 tarjetas cubren todas las clases del boceto inicial.
- Se solicitó agregar la colaboración entre Notificacion y Turno que estaba ausente.

## Code Review 2 — PR del Modelador de Diagramas de Casos de Uso

### Prompt utilizado

```
Lee anexos/introduccion.md. Revisá los archivos .puml en diagramas/02-casos-de-uso/ y verificá:
1. Que los actores sean correctos para cada caso de uso.
2. Que las relaciones include y extend estén bien aplicadas.
3. Que los 5 casos de uso cubran los RF1 a RF5.
4. Que el código PlantUML sea válido sintácticamente.
```

### Observaciones y ajustes
- Se corrigió la dirección de una relación extend que estaba invertida.
- Se verificó que el naming de archivos sigue la convención propuesta en la consigna.

## Code Review 3 — PR del Especialista en Escenarios

### Prompt utilizado

```
Lee anexos/introduccion.md. Revisá los archivos en diagramas/03-escenarios-casos-de-uso/ y verificá:
1. Que los 5 escenarios tengan todos los campos completos.
2. Que los pasos de la ruta principal sean lógicos y secuenciales.
3. Que las precondiciones y poscondiciones sean coherentes.
4. Que la prioridad y el riesgo estén justificados.
```

### Observaciones y ajustes
- Se solicitó completar poscondiciones faltantes en el escenario de Bloquear Agenda.
- Se verificó coherencia entre los escenarios y los diagramas de casos de uso.

## Code Review 4 — Revisión general de integración

### Prompt utilizado

```
Revisá la estructura completa del repositorio y verificá:
1. Que los índices (diagramasUML.md, herramientas_agile.md, escenarios_de_casos_de_uso.md) enlacen correctamente a todos los archivos.
2. Que el README.md esté actualizado con los nuevos índices.
3. Que el changelog.md refleje todas las contribuciones.
4. Que cada PR incluya su archivo ia/a2/[rol].md.
```

### Observaciones y ajustes
- Se actualizó el README.md para incluir los enlaces a Diagramas UML y Herramientas Agile.
- Se verificó que el changelog.md tenga entradas para cada integrante y PR.
