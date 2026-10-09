# Claude en MLV · manual y recetas del estudio

Borrador v0.1 para revisión de MLV Abogados. Todo con ejemplos ficticios; ningún dato de clientes.

## Qué hay

| Archivo | Qué es |
|---|---|
| `manual-del-estudio.md` | Las instrucciones que Claude lee siempre: datos de personas, citas, quién decide, estilo MLV. |
| `mlv-estudio/` | El paquete de recetas (plugin) que se instala en Claude. |

### Las recetas

| Receta | Para qué | Área |
|---|---|---|
| `verificar-citas` | Lista cada cita del escrito con su riesgo y dónde verificarla. Nada sale con citas «Pendiente». | Todas |
| `revisar-datos-antes` | Detiene el trabajo si el texto trae datos de personas sin tachar. | Todas |
| `minuta-laboral` | Borrador de la actualización laboral mensual, solo con las fuentes entregadas. | Laboral |
| `carta-despido` | Borrador de la carta y lista de control de forma y plazos para el abogado. | Laboral |
| `investigacion-ley-karin` | Plan, cronograma, pauta de entrevistas y estructura del informe. Nunca concluye. | Ley Karin |
| `solicitud-titular` | Solicitudes de titulares: plazos del art. 11 de la Ley 21.719 y cartas en borrador. | Datos personales |
| `informe-cliente` | Informe de una página para gerencia o RR. HH., sin jerga. | Todas |
| `registro-bitacora` | La línea para la Bitácora de IA: tiempo, reescritura y errores. | Todas |
| `nueva-receta` | Para el encargado: convertir un proceso en receta y corregirla con la bitácora. | Gestión |

Las recetas se llaman entre sí: toda receta que produce un escrito termina con `verificar-citas`, y toda receta
que recibe documentos empieza con `revisar-datos-antes`.

## Cómo se instala

**Para todo el estudio (plan Team o Enterprise de Claude).** El administrador sube el paquete `mlv-estudio` en la
configuración de la organización y lo deja disponible para todos; cada abogado lo recibe actualizado sin hacer
nada. El manual se pega en las instrucciones de la organización o de cada proyecto por área.

**En Claude Code (encargado de IA).**

```bash
claude plugin marketplace add dojedacifuentes/MLV
```

```bash
claude plugin install mlv-estudio@mlv
```

Después las recetas se usan escribiendo `/mlv-estudio:verificar-citas`, o simplemente pidiendo el trabajo: Claude
reconoce cuándo aplica cada receta por su descripción.

## Cómo se mantiene

- Cada receta tiene dueño (el dueño del proceso en el Sistema de trabajo), estado y fecha de revisión.
- Los errores se anotan en la Bitácora de IA (`herramientas/bitacora-ia.html`). La pestaña «Recetas» muestra cuáles
  hay que corregir; el encargado las corrige con `nueva-receta` y sube la versión en `plugin.json`.
- Los plazos y artículos que el estudio no ha verificado quedan como «[MLV confirma]». Las recetas no los inventan.
