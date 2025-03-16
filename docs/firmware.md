---
title: Firmware
layout: default
nav_order: 4
---

##  Firmware
Nota: esto es una explicación simple, hay muchísima mas información en la [Documentación de MrChromebox]

El firmware del chromebook es como la bios de un ordenador normal, se encarga de arrancar el sistema operativo y guardar datos esenciales para su funcionamiento.

El firmware sigue un sistema no estricto de versiones, indicado mediante el valor “kernver”, este refleja cambios importantes introducidos por google en el firmware. 

Algunas partes del firmware son esenciales para el correcto funcionamiento del dispositivo, así que el código de estas está bajo un protección de escritura, para que no sean fácilmente modificables.

## Firmware de Mrchromebox

Aparte del firmware normal de los chromebooks, se puede modificar, unas de las modificaciones más fiables y estables son el firmware de MrChromebox, existiendo dos tipos:

__RW_LEGACY__: Añade un bootloader de LEGACY_BIOS al firmware, permitiendo iniciar tanto ChromeOS como imágenes legacy. Windows no funciona. Esta basado en [SeaBios] y [TianoCore EDK II]

__UEFI (Full ROM)__ : Borra completamente el firmware estándar, e instala un firmware que permite el arranque de imágenes UEFI, incluyendo Windows. Esta basado en [Coreboot]


{: .note}
> El programa no permitirá instalar el firmware UEFI si no dispone de una unidad usb para crear un copia de seguridad del firmware estándar.

También se puede restaurar al firmware normal si tienes el de UEFI, mediante el [Firmware Utility Script] , puedes usar tu firmware guardado (muy recomendable), o descargar uno predeterminado desde el repositorio de MrChromebox.

[Firmware Ultility Script]: https://docs.mrchromebox.tech/docs/fwscript.html
[Documentación de MrChromebox]: https://docs.mrchromebox.tech/docs/firmware/
[TianoCore EDK II]: https://github.com/tianocore/edk2
[Coreboot]: https://github.com/coreboot/coreboot
[SeaBios]: https://github.com/coreboot/seabios