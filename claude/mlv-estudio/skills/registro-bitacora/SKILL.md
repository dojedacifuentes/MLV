---
name: registro-bitacora
description: Al cerrar un trabajo hecho con Claude, arma la línea para la Bitácora de IA del estudio - receta usada, minutos estimados sin IA y con IA, cuánto se reescribió y los errores que hubo. Úsala cuando el usuario diga «anótalo en la bitácora», «registra esto», «terminamos» o al final de cualquier receta del estudio.
---

# Registro en la bitácora

La bitácora es como el estudio sabe si Claude ahorra tiempo de verdad y dónde se equivoca. Cada error anotado
sirve para corregir la receta para todos.

## Qué haces

Pregunta lo que no sepas (son respuestas cortas) y entrega un bloque con estos campos, listo para copiar en la
pestaña «Registrar» de `herramientas/bitacora-ia.html`:

```
Fecha: 09-10-2026
Abogado (iniciales): 
Área: Laboral | Ley Karin | Datos personales | Corporativo | Derecho público | Litigación | Gestión del estudio
Receta: (por ejemplo, carta-despido; «sin receta» si no se usó ninguna)
Trabajo: (una línea, sin nombres de clientes ni de personas)
Minutos sin IA (estimado): 
Minutos con IA (real, incluida la revisión): 
Cuánto se reescribió: Nada | Poco | Mucho | Se descartó
Errores: Cita inexistente | Cita mal atribuida | Norma o plazo errado | Dato personal sin tachar | Omisión relevante | Estilo o tono | Ninguno
Qué pasó (si hubo error): 
Se informó al cliente del uso de IA: Sí | No | No aplica
```

## Reglas

- **Nunca** pongas nombres de clientes, de las partes ni de testigos: el trabajo se describe en general
  («carta de despido por necesidades de la empresa»).
- Si hubo un error, describe qué dijo Claude y qué era lo correcto, en una o dos líneas. Eso es lo que el encargado
  usa para corregir la receta.
- Si apareció un dato personal sin tachar en una cuenta o herramienta no autorizada, agrega:
  «Avisar hoy al dueño del protocolo (posible incidente)».
