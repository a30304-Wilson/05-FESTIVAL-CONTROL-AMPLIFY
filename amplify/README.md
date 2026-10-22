# Backend de Amplify para Festival Control

Este directorio contiene la parte del backend para la app de control del festival.

## Qué define

- Un modelo `FestivalEvent` con id, artista, escenario, hora y estado.
- Una API GraphQL gestionada por AWS Amplify.
- Autorización pública con API key para una demo de clase.

## Comandos de trabajo

```bash
npx ampx sandbox
npx ampx generate
```

Estos comandos crean el entorno local y el cliente de GraphQL que la app puede consumir.

## Despliegue real

Cuando tengas credenciales de AWS y el proyecto enlazado con Amplify Console, puedes publicar la app con:

```bash
npx ampx push
```

La app frontend dejaría de depender de datos en memoria y pasaría a guardar cambios en DynamoDB a través de la API de Amplify.
