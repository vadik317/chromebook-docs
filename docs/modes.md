---
title: Modo desarollador
layout: default
nav_order: 1
---

## Tabla de contenidos
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Pantalla de recuperación

ChromeOS, tiene un modo de recuperación donde se puede recuperar el sistema operativo. 
Algunos ejemplos de la pantalla de recuperación:

<img src="https://docs.mrchromebox.tech/images/cros_recovery_old.jpg" alt="isolated" width="450"/> <img src="https://docs.mrchromebox.tech/images/cros_recovery_old_details.jpg" alt="isolated" width="450"/>
<img src="https://docs.mrchromebox.tech/images/cros_recovery_new.jpg" alt="isolated" width="450"/> <img src="https://docs.mrchromebox.tech/images/cros_recovery_new_details.jpg" alt="isolated" width="450"/>

A este se accede mediante los botones ```ESC + REFRESH + POWER```
Este modo permite la recuperación del sistema, y el acceso a modo desarrollador.

---

## Modo desarrollador y verificación SO

Este modo se accede desde el la pantalla de recuperación, pulsando las teclas ```CTRL + D```, presionando ```ENTER``` en la pantalla de confirmación. En este momento el sistema estará en modo desarrollador, el sistema se reiniciará y estará en modo desarrollador, posteriormente, el sistema se iniciará con una pantalla de aviso, se presiona ```CTRL + D``` para arrancar desde el disco interno.
La primera vez que se inicia en modo desarrollador hay un timer de 5 minutos.
Imagen de ejemplo:


Estando en el modo desarrollador obtenemos más control sobre el sistema:
- Acceso completo al sistema mediante shell VT2 (terminal virtual)
- Modificación del sistema y la kernel
- El arranque de sistemas operativos diferentes mediante un bootloader alternativo (en sistemas que tengan esa función)
- Permite realizar modificaciones al firmware, algunas de las cuales pueden necesitar que se desactive la protección de escritura

Esta pantalla se queda de manera indefinida hasta que el usuario presione nuevamente ```CTRL + D``` cada vez que se arranca el sistema. Si se mantiene en esta pantalla durante 30 segundos, suena un pitido de alerta a máximo volumen.

Para obtener mas información, leer [Documentación de MrChromebox]

[Documentación de MrChromebox]: https://docs.mrchromebox.tech/docs/boot-modes/developer.html