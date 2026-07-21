# Sistema eléctrico — Actualización 21/07/2026

En este documento reporto el estado de los sistemas eléctricos y cómo los tengo configurados.

## Equipos

| Equipo | Tipo | Potencia |
|---|---|---|
| Switch Cisco Catalyst 2960 | Switch | Sin datos |
| Dell PowerEdge R320 | Servidor 1U | ~110 W |
| MGE Ellipse Premium 800 | SAI | 800 VA |

## Conexiones

Todos los equipos están conectados al SAI, salvo una de las PSU del servidor, que está conectada directamente a la red.

## Planes a futuro

- Configurar una alerta de caída eléctrica desde el BMC del servidor, basada en la pérdida de energía de la PSU no conectada al SAI.
- Conectar el router del ISP al SAI para garantizar conectividad en caso de caída eléctrica.
  - Sería necesario mover de sitio el router y, por tanto, tirar fibra.
- Eliminar SPOF de única toma de corriente para todos los sistemas.
