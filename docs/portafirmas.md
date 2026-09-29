# Portafirmas

La plataforma con la que la UCA firma electrónicamente sus documentos administrativos. Como docente la usarás en dos sentidos: para firmar lo que te llega y para enviar a firmar lo que tú tramitas.

## 1 · Antes de entrar: los requisitos

Los tres requisitos se configuran una sola vez en cada equipo.

1. **AutoFirma instalada.** Es la aplicación cliente que hace la firma en tu equipo. En Windows y macOS no necesita Java aparte; en Linux sí requiere un entorno de ejecución de Java de Oracle u OpenJDK. La instalación necesita permisos de administrador.
2. **Navegador compatible** con los requisitos de AutoFirma. Como alternativa existen clientes ligeros de firma para iOS y Android.
3. **Certificado personal** admitido por la plataforma @firma en versión 5.2 o superior. Sirve el Certificado de Empleado Público (CEP).

!!! warning "Si la instalación falla"

    Comprueba que se está ejecutando con permisos de administrador. Si el problema persiste, abre una incidencia en el CAU.

Instala el certificado también en el móvil si prevés firmar fuera del despacho: los clientes móviles de Portafirmas permiten firmar desde iOS y Android.

## 2 · Acceder

1. Abre `pfirma.uca.es`. Si tu organización tiene Single Sign On, la autenticación puede ser automática.
2. Entra con **usuario y contraseña** institucionales, o pulsa **Acceder mediante certificado**: se arrancará el cliente de firma y una ventana emergente te mostrará los certificados instalados en el navegador para que elijas el tuyo.
3. Si activas el **segundo factor de autenticación**, el sistema pedirá además un código enviado a tu correo. Puedes guardar el navegador como dispositivo de confianza para no repetirlo en ese equipo.

!!! info "Primer acceso sin permisos"

    Si no aparecen las opciones esperadas, puede deberse al perfil asignado, que corresponde establecer a un administrador. Escribe al CAU indicando qué necesitas hacer.

## 3 · Qué puedes hacer: los perfiles

Lo que ves en la plataforma depende del perfil que tengas asignado. Conviene comprobarlo antes de reclamar una función que quizá no tengas asignada.

| Perfil | Qué habilita |
| --- | --- |
| **ACCESO** | Entrada básica: solo las bandejas de terminadas y enviadas, más la configuración de usuario. |
| **FIRMA** | Muestra las bandejas de pendientes y en espera, y permite firmar. |
| **REDACCIÓN** | Permite enviar peticiones de firma a otras personas desde la pantalla de redacción. |
| **REDACCIÓN.LIMITADO / .AUTORIZADO** | Igual que el anterior, pero restringido a personas o aplicaciones autorizadas. |
| **EDICIÓN** | Permite modificar líneas de firma, con variantes limitada y autorizada. |
| **SUPERVISOR** | Gestiona las peticiones de un conjunto de aplicaciones. |
| **SHARE.JOB / SHARE.USER** | Compartir bandejas entre cargos o entre personas. |
| **REGISTRO / NOTIFICA** | Registrar y notificar documentos una vez finalizados. |

## 4 · Las cuatro bandejas

Toda la plataforma gira alrededor de estas cuatro bandejas. Cada petición está siempre en una de ellas.

| Bandeja | Qué contiene |
| --- | --- |
| **Pendientes** | Lo que espera una acción tuya: firmar, dar el visto bueno o devolver. |
| **En espera** | Peticiones que aún no te tocan porque van en cascada y hay firmas previas. |
| **Terminadas** | Lo ya firmado o devuelto. Aquí acaba todo lo que pasa por tus manos. |
| **Enviadas** | Las peticiones que has redactado tú y su estado actual. |

- Cada fila muestra remitente o destinatario, asunto, referencia y fecha de actualización; por defecto se ordenan por fecha de actualización.
- Puedes **seleccionar varias peticiones a la vez** con la casilla superior para aplicar acciones en bloque.
- Las bandejas se pueden **exportar** a PDF, XML, hoja de cálculo o texto plano: útil para dejar constancia de lo tramitado en un periodo.
- En Terminadas y Enviadas hay filtros para mostrar solo las peticiones completadas.
- Las **etiquetas** organizan las peticiones y se ven junto al asunto. Hay tres tipos, distinguidos por color: de sistema, propias tuyas y globales definidas por administración, estas últimas con un icono de varias personas.

## 5 · La pantalla de petición

En la versión 3 no hay una pantalla aparte: la petición se despliega dentro de la propia bandeja y muestra allí toda su información.

**Documentos.** Se listan los documentos firmables y los anexos, diferenciados por iconos. Puedes descargarlos, descargar los informes de firma y, sobre lo ya firmado, rectificar documentos y crear peticiones enlazadas.

**Histórico.** Recoge los comentarios y los cambios de estado, empezando por el texto original de la petición. Puedes añadir, editar y borrar tus propios comentarios: es el sitio donde dejar constancia de por qué firmaste o devolviste algo.

**Menú de opciones.** Tras el icono de puntos suspensivos están el resto de herramientas de la petición: filtrar documentos, ver el **árbol de firmantes** con las líneas de firma y su tipo (firma, CSV o visto bueno), consultar los metadatos en una tabla filtrable, acceder a las conversaciones activas, marcar como no leído y **usar la petición como plantilla** para la siguiente igual.

## 6 · Firmar

1. Desde la bandeja de **pendientes**, selecciona la petición o peticiones y pulsa **Firmar**.
2. Se abre una ventana con los datos relevantes del documento. Es la última pantalla antes de que la firma se produzca.
3. Marca la casilla **«Conozco el contenido de los documentos»**. Solo aparece, y es obligatoria, cuando la petición está en estado *Nuevo*.
4. Si procede, activa **«Demorar la fecha de firma del siguiente»** para aplazar la firma de la persona que va detrás de ti.
5. Elige el certificado: del navegador, de tarjeta o custodiado en la nube. Si no tienes ninguno configurado, AutoFirma te deja seleccionarlo desde el navegador o el lector de tarjetas.
6. Al terminar, la petición pasa a estado firmado y se traslada sola a la bandeja de terminadas.

- **Firma en bloque:** puedes seleccionar varias peticiones a la vez. Si alguna tiene una configuración de firma distinta a la establecida en el sistema, esa no se firmará.
- **Firma en segundo plano:** permite seguir trabajando mientras el proceso se completa. Recomendable en lotes grandes.
- Puedes incluir en el histórico la **información del cargo** desde el que firmas, lo que evita ambigüedades cuando ocupas más de un puesto.

## 7 · Devolver una petición

La devolución es la vía prevista para rechazar una petición que no procede firmar. Conviene indicar siempre el motivo.

1. Selecciona una o varias peticiones pendientes y pulsa **Devolver**, o hazlo desde el menú de la propia petición desplegada.
2. Se muestran los datos de la petición y un cuadro de texto para el **motivo de la devolución**. Es la información que recibirá quien redactó la petición.
3. Marca la casilla de conformidad cuando aparezca (de nuevo, solo si el estado es *Nuevo*) y confirma.
4. La petición pasa a terminadas con la etiqueta **Devuelto**, o se elimina del sistema según lo que haya configurado la administración.

## 8 · Redactar tus propias peticiones

Se accede desde **Redactar**, en el menú de peticiones de la izquierda. Requiere tener perfil de redacción.

**Lo mínimo.** Cumplimentar los campos obligatorios y adjuntar al menos un documento.

**Destinatarios.** Puedes añadir personas y puestos de trabajo; el autocompletado busca por nombre, apellidos, DNI o cargo. Los remitentes, si están habilitados, permiten compartir la petición con otras personas interesadas. Según tu perfil (REDACCIÓN, LIMITADO o AUTORIZADO), la lista de firmantes disponibles puede estar restringida.

**Documentos.** Se adjuntan desde el explorador de ficheros, con carga múltiple. Hay que indicar el tipo de documento y si es firmable o anexo. Si está disponible el conversor, se pueden convertir a PDF, y también añadir enlaces web como documentación complementaria.

**Tipo de firma.** En opciones avanzadas eliges el circuito: **cascada** (orden establecido), **paralela** (sin orden) o **distribuida**, pensada para muchos firmantes y recomendada a partir de veinticinco.

**Otras opciones avanzadas.** Avisos por correo en los cambios de estado, fecha de inicio de visibilidad, caducidad (informativa) y definición del visto bueno.

!!! tip "Dos atajos que se agradecen"

    Para una petición recurrente, busca una anterior y usa la opción **«Usar como plantilla»** en lugar de redactarla de nuevo. Elige cascada cuando las firmas deban producirse en un orden determinado, por ejemplo un informe previo a un visto bueno; en el resto de casos la paralela se completa antes.

## 9 · Configuración recomendada

Accesible desde el enlace de la barra superior derecha. Cuatro ajustes que conviene tocar el primer día.

- **Datos de contacto y correo:** revisa que el correo sea el institucional; de él dependen los avisos y el segundo factor.
- **Segundo factor con Google Authenticator** o por correo: actívalo si firmas documentos con efectos administrativos.
- **Etiquetas personalizadas:** créate las tuyas (por ejemplo, por asignatura o por tipo de trámite) para no perder peticiones en bandejas largas.
- **Estilo:** tamaño de letra y menú izquierdo comprimido. La interfaz se adapta sola a móvil y tableta.

## Acceso, manual completo y soporte

- Aplicación: [pfirma.uca.es](https://pfirma.uca.es).
- [Manual de usuario del Portafirmas](https://pfirma.uca.es/pfirma/static/public/help/user/es/index.html) — la referencia completa, con capítulos sobre supervisión, búsqueda, filtros y edición de líneas de firma.
- [Portafirmas en Administración Electrónica UCA](https://administracionelectronica.uca.es/portafirmas/) — guía rápida, manual para personas invitadas y videocurso.
- [Preguntas frecuentes del Portafirmas](https://administracionelectronica.uca.es/faqpfirma/).
- Instrucción **UCA/I01GER/2023**, que concreta el procedimiento de uso del sistema para la firma de documentos públicos o administrativos de la UCA.
- Soporte: `info.ae@uca.es` · [CAU de Administración Electrónica](https://cau.uca.es/cau/grupoServicios.do?id=C03).
