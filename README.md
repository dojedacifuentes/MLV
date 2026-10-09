# MLV Abogados · Herramientas Ley 21.719

Asesoría a Cristóbal Luksic Ziliani (Abogado Director, MLV Abogados) para crear herramientas que ayuden a
los clientes de la firma a adecuarse a la Ley 21.719 de protección de datos personales.

## Qué hay aquí

| Carpeta | Contenido |
|---|---|
| `herramientas/panel-clientes.html` | Panel de clientes: cada cliente con el estado de su adecuación a la Ley 21.719. |
| `herramientas/derechos-y-consentimientos.html` | Para la empresa cliente: usos de datos con su base legal (las seis de los arts. 12 y 13), solicitudes de titulares con sus plazos del art. 11 y cartas borrador, consentimientos y revocaciones, formulario para titulares e historial con huellas encadenadas (SHA-256). Demo con una empresa ficticia. |
| `herramientas/tachar.html` | Tachador: cambia nombres, RUT, direcciones y otros datos por etiquetas antes de pegar un texto en una IA. |
| `herramientas/diagnostico.html` | Diagnóstico de herramientas: encuesta anónima (Microsoft Forms) sobre cómo el estudio usa y crea herramientas e IA; carga el Excel de Forms y arma el informe con riesgos y prioridades. Demo con respuestas ficticias. |
| `herramientas/sistema-de-trabajo.html` | Sistema de trabajo del estudio: procesos con dueño y revisión, tablero de casos por proceso e instrucciones para Claude. |
| `index.html` | Portada con las herramientas. |
| `reunion/` | Material para las reuniones con MLV. |

Todo son páginas sueltas: se abren con doble clic en Chrome o Edge, sin instalar nada y sin internet.
Ninguna envía datos fuera del computador (lo bloquea la propia página).

Las cinco herramientas comparten el mismo diseño: los mismos colores y botones, un enlace de vuelta a la portada,
y una guía de primer uso que se abre sola la primera vez y después con «Cómo se usa». En los tableros, las tarjetas
se mueven con los botones «Volver» y «Avanzar» (en el computador también se pueden arrastrar). El código de la guía
es idéntico en las cinco (busca «Guía de primer uso»): si se corrige en una, hay que copiarlo a las otras.

## Reglas

- **Ningún dato real de clientes entra a este repositorio.** Los respaldos y llaves (`.json`) quedan fuera
  (ver `.gitignore`). Los ejemplos son ficticios.
- La Ley 21.719 rige desde el 01-12-2026, salvo que se apruebe la postergación (boletín 18.623-07).
  Verificar el estado antes de citar fechas.
