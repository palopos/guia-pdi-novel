# Primeros trámites UCA — guía de acogida del profesorado novel

Guía de los trámites administrativos que necesita resolver el profesorado recién
incorporado a la Universidad de Cádiz: VPN, gestión de actas, Portafirmas, SIRE,
Portal de Servicios y solicitud de documentación acreditativa.

Elaborada en el marco del proyecto **«Mentoría docente y producción audiovisual
para profesorado novel en la Universidad de Cádiz»**, avalado por la convocatoria
ACTÚA de Actuaciones Avaladas para la Mejora Docente del curso 2025/2026.

## Cómo está montado

El contenido son ficheros Markdown en `docs/`. El sitio se construye con
[Zensical](https://zensical.org/), el generador del equipo de Material for MkDocs,
que lee la configuración `mkdocs.yml` sin cambios.

**El contenido no depende del generador.** Si Zensical dejara de mantenerse, el
mismo `mkdocs.yml` y los mismos ficheros Markdown construyen con
`mkdocs` + `mkdocs-material` sin tocar una línea. Esa portabilidad es
deliberada: la guía debe sobrevivir a la herramienta con la que se publica.

## Trabajar en local

```bash
python -m venv .venv
source .venv/bin/activate      # Windows: .venv\Scripts\activate
pip install -r requirements.txt

zensical serve                 # servidor local con recarga automática
zensical build                 # genera el sitio estático en site/
```

Para construir con MkDocs Material en lugar de Zensical:

```bash
pip install mkdocs-material
mkdocs serve
mkdocs build
```

## Publicar

El resultado de `build` es HTML estático sin dependencias de servidor: se puede
alojar en GitHub Pages o **copiarse tal cual a un servidor web de la Universidad**,
que es lo que cumple el compromiso de repositorio institucional de libre acceso
adquirido en el proyecto.

- **GitHub Pages:** el flujo de trabajo de `.github/workflows/deploy.yml` publica
  en cada `push` a `main`. Hay que activar Pages en los ajustes del repositorio,
  con origen «GitHub Actions».
- **Servidor de la Universidad:** ejecutar `zensical build` y entregar el
  contenido de `site/` a la persona responsable de la web del centro.

Antes de publicar, actualizar `site_url` en `mkdocs.yml` con la dirección
definitiva.

## Cómo contribuir

1. Abre una *issue* si detectas un procedimiento que ha cambiado. Las aplicaciones
   institucionales se actualizan a menudo y ese es el principal riesgo de esta guía.
2. Para corregir algo, edita el `.md` correspondiente y abre una *pull request*.
3. Norma de contenido: **cada afirmación debe poder respaldarse con documentación
   oficial de la UCA**, enlazada al final de la página. Si no hay fuente, no entra.
4. La guía es **neutra respecto al centro**: no debe contener nombres de centros,
   departamentos ni direcciones de correo concretas, salvo las de servicios
   generales de la Universidad. Lo que varía de un centro a otro se redacta como
   «pregunta en tu centro».

## Estructura

```
mkdocs.yml                 configuración del sitio y navegación
requirements.txt           dependencias de construcción
docs/
  index.md                 portada: calendario, índice y checklist
  vpn.md                   VPN de la UCA (requisito previo)
  actas.md                 gestión de actas
  portafirmas.md           Portafirmas
  sire.md                  SIRE, reserva de espacios y recursos
  portal-servicios.md      Portal de Servicios
  documentacion.md         documentación acreditativa
  stylesheets/extra.css    paleta y tipografía
.github/workflows/deploy.yml
```

## Fuentes

Cada página enlaza al final la documentación oficial en la que se basa: guía del
docente de Calificación de Actas Web, manual de usuario de Portafirmas, ayuda de
la aplicación SIRE, documentación de Servicios Informáticos sobre la VPN y
catálogo de procedimientos de la Sede Electrónica.
