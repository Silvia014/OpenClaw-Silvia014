---
name: get-pending-work
description: Obtiene las tareas, ejercicios o trabajos pendientes del estudiante desde la API de 4Geeks.
---

# Get Pending Work

## Purpose

Consultar las actividades pendientes del estudiante autenticado utilizando la API de 4Geeks.

## When to use

Usa esta skill cuando el usuario pregunte:

- qué tengo pendiente;
- qué ejercicios debo hacer;
- qué tareas me faltan;
- qué trabajo tengo por completar.

## Execution

1. Utiliza la autenticación existente para acceder a la API de 4Geeks.
2. Consulta únicamente la información relacionada con trabajo pendiente.
3. Muestra únicamente actividades que no estén completadas.
4. No mezcles esta información con proyectos u otros recursos.
5. No inventes tareas.

## Output

Para cada actividad pendiente, muestra cuando esté disponible:

- Nombre
- Estado
- Fecha límite
- Proyecto o módulo relacionado

## Error Handling

Si no existen tareas pendientes, indícalo claramente.

Si la API falla:

- informa del error real;
- no inventes actividades;
- no afirmes que la consulta fue exitosa.

## Example

User:

"¿Qué tengo pendiente?"

Expected behavior:

1. Consultar la API de 4Geeks.
2. Obtener las actividades pendientes.
3. Mostrar únicamente las actividades que todavía no están completadas.
