---
name: nueva-receta
description: Para el encargado de IA del estudio - convierte un proceso documentado en el Sistema de trabajo (o descrito en la conversación) en una receta nueva para Claude, con su archivo SKILL.md, sus reglas de revisión y una prueba. Úsala cuando pidan «crear una receta», «convertir este proceso en receta», «nueva skill para el estudio» o corregir una receta a partir de la bitácora.
---

# Crear o corregir una receta del estudio

Las recetas son del estudio, no de una persona. Cada una tiene un dueño (el dueño del proceso), un estado
(borrador, en prueba, en uso) y una fecha de revisión, igual que los procesos del Sistema de trabajo.

## Para crear una receta

1. **Parte del proceso documentado.** Pide la ficha del proceso (pestaña «Usar con Claude» del Sistema de trabajo) o
   las respuestas a las 10 preguntas de «Documentar un proceso». Sin dueño ni revisión, no hay receta.
2. **Separa lo que hace Claude de lo que decide el abogado.** Todo lo que sea una decisión jurídica (causal,
   conclusión, estrategia) queda del lado del abogado.
3. **Escribe el SKILL.md** con:
   - `name` en minúsculas con guiones y `description` que diga qué hace **y cuándo usarla**, con las frases que
     diría un abogado del estudio;
   - «Antes de empezar» (siempre `revisar-datos-antes` si hay datos de personas; qué pedir si falta);
   - los pasos;
   - «Lo que no haces»;
   - «Al terminar» (siempre `verificar-citas` si produce un escrito).
4. **Plazos y artículos:** solo los que el estudio verificó en la fuente oficial. Los demás van como
   «[MLV confirma]» o «MLV lo completa».
5. **Prueba:** tres casos ficticios (uno normal, uno con información incompleta, uno que debería hacer que Claude
   se detenga) y lo que se espera en cada uno.

## Para corregir una receta con la bitácora

1. Lee los errores anotados para esa receta (pestaña «Recetas» de la Bitácora de IA).
2. Por cada error repetido, agrega una regla concreta en «Lo que no haces» o un control en «Antes de empezar».
3. Sube la versión en `plugin.json`, anota el cambio en el historial del proceso y vuelve la receta a
   «en prueba» hasta que el dueño la apruebe.
