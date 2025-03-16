---
title: Liberación
layout: default
nav_order: 5
---

## Tabla de contenidos
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Diferentes maneras de “liberar” chromebooks
{: .no_toc}
Para comprobar la versión del chromebook es tan simple como darle a ALT + V en la pantalla de inicio, en la esquina superior derecha aparecerá la versión de ChromeOS

### Version ChromeOS < 111 y kernver = 1
Simplemente iniciar shimmer y seleccionar (d), alternativamente puedes ejecutar el comando vpd -i RW_VPD -s check_enrollment=0

### Version ChromeOS = 111 y kernver = 1
Revertir a una versión de ChromeOS inferior a 111 y hacer lo mismo que las versiones anteriores.

### Version 125-127 (con el móvil)
Se necesita un móvil android, y activar wifi, bluetooth y geolocalización en el móvil.

1. Restablecer el chromebook de fabrica
2. Conectar a la wifi mediante ajustes rápidos (```SHIFT + ALT + S```)
3. Presionar ```CTRL ALT + Q``` y darle a empezar
4. Transferir wifi desde el móvil
5. Conectar el movil
6. Escanear el código qr y seguir instrucciones
7. Transferir wifi desde el móvil de nuevo
8. cerrar la app en el móvil y desconectar la wifi y bluetooth
9. Iniciar sesion con cuenta de google personal
10. Seguir la configuración del chromebook
11. Cuando termine, presiona ```CTRL + SHIFT + Q + Q``` para volver a la pantalla de inicio, dando a que por ahora esta cuenta es de un solo uso (hasta que se cierre sesión, que es precisamente lo que hacemos)
12. Volver a iniciar sesión con cuenta personal, esta vez va a ser persistente y se quedará en el dispositivo. 
