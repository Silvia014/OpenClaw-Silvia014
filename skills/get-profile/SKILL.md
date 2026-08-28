---
name: get-profile
description: Obtiene la información del perfil del estudiante autenticado desde la API de 4Geeks.
---

# Get Student Profile

## Purpose

Obtener información básica del estudiante autenticado desde la API de 4Geeks.

## When to use

Usa esta skill cuando el usuario pregunte por:

- su perfil;
- sus datos como estudiante;
- su información académica básica;
- su programa o cohorte, si esta información está disponible en la respuesta.

## Execution

1. Utiliza el sistema de autenticación existente para acceder a la API de 4Geeks.
2. No solicites nuevamente el token si ya está disponible en la configuración o herramientas existentes.
3. Realiza la petición al endpoint de perfil del estudiante.
4. Devuelve únicamente información recibida desde la API.
5. No inventes información.

## Output

Presenta la información de forma clara y breve.

Por ejemplo:

- Nombre
- Email
- Cohorte
- Programa

Incluye únicamente los campos realmente devueltos por la API.

## Error Handling

Si la petición falla:

- informa del error real;
- no inventes datos;
- no afirmes que la información fue obtenida correctamente si la API falló.

## Example

User:

"Muéstrame mi perfil"

Expected behavior:

1. Consultar la API de 4Geeks.
2. Obtener el perfil del estudiante autenticado.
3. Mostrar los datos disponibles.
