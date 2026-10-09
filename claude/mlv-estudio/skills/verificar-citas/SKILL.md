---
name: verificar-citas
description: Lista cada cita de un escrito (leyes, artículos, decretos, dictámenes, fallos, roles, doctrina) y arma la planilla de verificación que el abogado completa antes de entregar. Úsala siempre antes de que un borrador salga del estudio, cuando el usuario pida «verificar citas», «revisar referencias» o «¿está todo citado bien?», y al terminar cualquier otra receta que produzca un escrito.
---

# Verificar citas antes de entregar

Regla del estudio: **toda cita la verifica un abogado en la fuente oficial**. Que otra IA (o tú mismo) la
revise no cuenta como verificación. Tu trabajo es que no se escape ninguna y que el abogado sepa dónde mirar.

## Qué haces

1. **Recorre el texto completo** y extrae cada referencia, aunque parezca obvia:
   - normas: «Ley N° …», «art. …», «inciso …», «DFL …», «Decreto …», «Código del Trabajo», «Constitución»;
   - pronunciamientos administrativos: dictámenes y ordinarios de la Dirección del Trabajo, de la Contraloría,
     resoluciones de la Agencia de Protección de Datos, del CPLT, de la Superintendencia que corresponda;
   - jurisprudencia: tribunal, rol, fecha, partes, considerando;
   - doctrina: autor, obra, página;
   - cifras con fuente: plazos, montos, UTM/UF, porcentajes.
2. **Clasifica cada una** según el riesgo, en este orden:
   - **Alta:** fallos, roles, dictámenes y doctrina (son las que la IA inventa con más facilidad y las que han
     terminado en sanciones a abogados en Chile);
   - **Media:** artículos con número de inciso o letra, plazos y montos;
   - **Baja:** nombre y número de una ley conocida, sin artículo.
3. **Marca lo que no puedes respaldar.** Si la cita vino de ti (no del texto que te dieron ni de una fuente que el
   usuario pegó), di expresamente: «Esta cita la propuse yo y no la he verificado».
4. **Indica dónde se verifica:** BCN Ley Chile para normas; el buscador de jurisprudencia del Poder Judicial para
   roles; el sitio de la Dirección del Trabajo para dictámenes; el sitio del organismo para sus resoluciones.
   No inventes enlaces: da el sitio, no una dirección exacta que no hayas visto.

## Qué entregas

Una tabla con estas columnas, en el orden en que aparecen en el texto:

| # | Cita tal como aparece | Tipo | Riesgo | ¿De dónde salió? | Dónde verificar | Estado |
|---|---|---|---|---|---|---|

- «¿De dónde salió?»: «del texto original», «de la fuente que pegó el usuario» o «propuesta por Claude».
- «Estado» empieza siempre en **Pendiente**. Solo el abogado lo cambia a Verificada, Corregida o Eliminada.

Al final, una línea: «N citas, X de riesgo alto. El escrito no debe salir mientras haya citas en Pendiente».

## Lo que no haces

- No declares nada como verificado.
- No corrijas una cita «de memoria»: si crees que el número está mal, dilo y deja la corrección para el abogado.
- No borres citas del escrito por tu cuenta.

La misma lista se puede pegar en la pestaña «Verificar citas» de la Bitácora de IA del estudio
(`herramientas/bitacora-ia.html`), que guarda la constancia de quién verificó y cuándo.
