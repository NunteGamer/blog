---
title: Cómo monté servidor casero de fotos
tags:
  - servidor
  - immich
  - xubuntu
  - linux
  - homelab
  - tailscale
  - hardware
---
No quería depender de Google ni de nubes ajenas: solo un sitio donde guardar fotos, acceder desde el móvil y olvidarme del lío de apps y de darle mis datos a compañías multimillonarias. Lo monté con lo que tenía por casa —un ThinkCentre pequeño—, lo escondí en un armario y al final salió algo sorprendentemente funcional.

## La idea
Empezó como una prueba: revivir un PC viejo, instalar una distro ligera y ver cuánto era capaz de aguantar. Era un **Lenovo ThinkCentre M91 UFF** (de los cuales tenia otro exactamente igual por diversas causas que no llegué a usar en este proyecto) cuyas especificaciones podéis leer [aquí](https://www.pc-portatil.com/pub.shop/ordenadores-segunda-mano/Lenovo-Thinkcentre-M91-USFF-Core-i3-2100-5714.html?srsltid=AfmBOookAnO6jX_y_w3LmiERkyjx97dSunrODifKGZrTK7J-a4HfVKUM). Al llevarlo a mi habitación vi que no tenía espacio donde ponerlo, así que decidí montarlo en el armario. No fue ni mucho menos fácil al principio porque todo estaba lleno de cajas y otras cosas que me impedían colocarlo todo como a mí me gustaba. Días después hice una limpieza y el setup se terminó viendo mucho más limpio.

Al principio **ni siquiera sabía** qué iba a hacer con el ordenador. Solo quería ponerle Linux y ver que tenía para ofrecer. Días después me enteré de lo que era [**Immich**](https://immich.app), un proyecto de [código abierto](https://github.com/immich-app/immich) que busca dejar atrás todas estas plataformas para subir fotos para poder hostear la tuya propia. Me sorprendió que tenía muchísimas funciones, desde hacer álbums o mostrar las ubicaciones en un mapa hasta poder crear varios perfiles para todos los miembros de la casa.

## La práctica
Empecé haciendo listado de lo que necesitaba. Para el **sistema operativo** usé **[Xubuntu](https://xubuntu.org)**, una distribución de Linux basada en Ubuntu pero que eliminaba todos los paquetes innecesarios para que la instalación fuese ligera y que el ordenador funcionase bien, lo que me vino perfecto, ya que podía gozar de la compatibilidad de los paquetes de Ubuntu mientras el ordenador solo tenía que cargar las casi inexistentes animaciones de `xfce4`.

Aunque Immich ya viene con su propia guía de instalación también fue necesario instalar **[Docker](https://www.docker.com)** para su funcionamiento, aunque también tiene otros métodos de instalación.

Por último, instalé **[Tailscale](https://tailscale.com)**, un servicio muy bueno y **gratuito** para utilizar como VPN y así poder acceder a mis fotos desde cualquier lugar del planeta.
