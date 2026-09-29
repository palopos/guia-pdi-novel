# VPN de la UCA

Requisito previo de varias de las aplicaciones recogidas en esta guía, que no son accesibles desde fuera de la red universitaria. Conviene configurarla al incorporarse.

## Qué es y qué te desbloquea

La Red Privada Virtual extiende la red universitaria hasta tu ordenador esté donde esté, mediante un túnel cifrado contra los servidores de RedUCA. Solo el tráfico dirigido a direcciones de la Universidad pasa por el túnel; el resto de tu navegación sale a Internet con normalidad, así que puedes dejarla conectada mientras trabajas.

- Acceder al **ordenador de tu despacho** desde casa.
- Consultar el **correo por POP3 o IMAP** con Thunderbird, Outlook o similares.
- Entrar en las **aplicaciones web restringidas a la red UCA**.
- Usar las **aplicaciones de gestión**: actas, Universitas XXI y compañía.
- En esta guía la necesitas, en concreto, para el [Sistema de Información](documentacion.md), de donde salen los informes de encuestas de satisfacción docente.

## 1 · Primero el doble factor, sin excepción

!!! warning "Sin 2FA la VPN no funciona"

    El doble factor de autenticación es obligatorio desde el 15 de septiembre de 2023. Si no lo has activado, la conexión no se establecerá, por muy bien que hayas instalado el cliente. Es el orden correcto: primero el 2FA, después el programa.

1. Instala una **aplicación autenticadora**: aplicación de móvil, extensión de navegador o programa de escritorio. Las recomendadas por la UCA son Google Authenticator y la extensión Authenticator del navegador.
2. Entra en [cau.uca.es/vpn-2fa](https://cau.uca.es/vpn-2fa) con tus credenciales UCA.
3. **Escanea el código QR** que aparece, o copia la clave, desde tu aplicación autenticadora.
4. A partir de ahí, la aplicación te genera un código de seis cifras que cambia cada treinta segundos. Ese es el tercer dato que pedirá la VPN, además de usuario y contraseña.

!!! danger "No dejes el autenticador en un solo dispositivo"

    Si el autenticador está configurado únicamente en el móvil, perderlo o cambiarlo impide el acceso. Guarda la clave de recuperación o configúralo también en una extensión de navegador.

Hay guías en PDF del CAU para las dos opciones, con [Google Authenticator](https://cau.uca.es/docs/Uso-2FA-VPN-FortiClient-GoogleAuthenticator.pdf) y con la [extensión del navegador](https://cau.uca.es/docs/Uso-2FA-VPN-FortiClient-ChromeExtension.pdf).

## 2 · Elegir cliente

Hay dos clientes admitidos. EduVPN está disponible en todos los sistemas, así que es la opción sencilla si no tienes un motivo para lo contrario.

| Sistema | Clientes disponibles |
| --- | --- |
| Windows | EduVPN · FortiClient |
| macOS | EduVPN · FortiClient 6.2 |
| Linux | EduVPN |
| Android | EduVPN · FortiClient |
| iOS | EduVPN · FortiClient |

## 3 · Instalar y conectar con EduVPN

El procedimiento descrito es el de Windows; en el resto de sistemas la secuencia es equivalente, cambiando solo la descarga.

1. Descarga el cliente desde [eduvpn.org/client-apps](https://www.eduvpn.org/client-apps/) e instálalo con las opciones por defecto.
2. Abre la aplicación y, en el campo de búsqueda, escribe `Cadiz`. Selecciona **Universidad de Cádiz** en la lista.
3. Se abrirá una ventana del navegador pidiendo tus credenciales universitarias: tu identificador **uDNI** o tu dirección de correo institucional.
4. Introduce a continuación el **código de 2FA** que te muestre tu aplicación autenticadora.
5. Autoriza a la aplicación a acceder a tu perfil de EduVPN.
6. Vuelve a la aplicación, donde ya aparecen los datos de conexión, y pulsa el botón de activación para levantar el túnel. El icono de la barra de tareas te indica en todo momento si estás conectado.

!!! warning "El perfil caduca a los siete días"

    Pasado ese plazo hay que volver a autenticarse. Es el comportamiento previsto del cliente, no un error de configuración.

## 4 · Llegar al ordenador del despacho (Windows)

1. Con la VPN conectada, abre **Inicio → Ejecutar** y escribe `\\nombre_ordenador\directorio`.
2. Si no resuelve el nombre, añade los **sufijos DNS** `uca.es` y `uca` en la configuración de red.
3. Asegúrate de tener instalado el **Cliente para Redes Microsoft**.

## Manuales por sistema y soporte

- [Red Privada Virtual de la UCA](https://informatica.uca.es/vpn-uca/) — página principal, con los manuales de instalación de cada cliente y sistema operativo.
- [EduVPN en Windows](https://informatica.uca.es/vpn-uca-eduvpn-windows/) · [FortiClient en Windows](https://informatica.uca.es/vpn-uca-forticlient-windows/) · [FortiClient en Android](https://informatica.uca.es/vpn-uca-forticlient-android/) · [FortiClient en iPhone y iPad](https://informatica.uca.es/vpn-uca-forticlient-iphone-ipad/).
- Incidencias: [CAU de Servicios Informáticos](https://cau.uca.es/).
