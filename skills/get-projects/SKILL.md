---
name: get-projects
description: Obtiene los proyectos asignados al estudiante desde la API de 4Geeks.
---

# Get Student Projects

## Purpose

Consultar los proyectos asociados al estudiante autenticado utilizando la API de 4Geeks.

## When to use

Usa esta skill cuando el usuario pregunte:

- qué proyectos tiene;
- cuáles son sus proyectos asignados;
- en qué proyectos está trabajando;
- qué proyectos ha completado.

## Execution

1. Utiliza la autenticación existente para acceder a la API de 4Geeks.
2. Consulta el recurso o endpoint correspondiente a los proyectos del estudiante.
3. Obtén únicamente información relacionada con proyectos.
4. Devuelve únicamente datos recibidos desde la API.
5. No inventes información.

## Output

Para cada proyecto disponible, muestra cuando sea posible:

- Nombre
- Estado
- Fecha
- Progreso

Si algún campo no existe en la respuesta de la API, no lo inventes.

## Error Handling

Si la API devuelve un error:

- informa del error real;
- no muestres proyectos ficticios;
- no afirmes que la consulta fue exitosa si falló.

## Example

User:

"¿Qué proyectos tengo?"

Expected behavior:

1. Consultar la API de 4Geeks.
2. Obtener los proyectos del estudiante autenticado.
3. Mostrar una lista clara de los proyectos disponibles.
