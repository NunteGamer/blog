---
title: Cómo monté mi propio servidor de fotos
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

Al principio **ni siquiera sabía** qué iba a hacer con el ordenador. Solo quería ponerle Linux y ver que tenía para ofrecer. Días después me enteré de lo que era **[Immich](https://immich.app)**, un proyecto de [código abierto](https://github.com/immich-app/immich) que busca dejar atrás todas estas plataformas para subir fotos para poder hostear la tuya propia. Me sorprendió que tenía muchísimas funciones, desde hacer álbums o mostrar las ubicaciones en un mapa hasta poder crear varios perfiles para todos los miembros de la casa.

## La práctica
Empecé haciendo listado de lo que necesitaba. Para el **sistema operativo** usé **[Xubuntu](https://xubuntu.org)**, una distribución de Linux basada en Ubuntu pero que eliminaba todos los paquetes innecesarios para que la instalación fuese ligera y que el ordenador funcionase bien, lo que me vino perfecto, ya que podía gozar de la compatibilidad de los paquetes de Ubuntu mientras el ordenador solo tenía que cargar las casi inexistentes animaciones de `xfce4`.

Aunque Immich ya viene con su propia guía de instalación también fue necesario instalar **[Docker](https://www.docker.com)** para su funcionamiento, aunque también tiene otros métodos de instalación.

Por último, instalé **[Tailscale](https://tailscale.com)**, un servicio muy bueno y **gratuito** para utilizar como VPN y así poder acceder a mis fotos desde cualquier lugar del planeta.
## Antes de la práctica
No todo fue un camino de rosas a la hora de poner a funcionar esta piedra de ordenador. Al principio arrancó todo maravillosamente: Xubuntu era ligero y la máquina iba como una bala. Luego, desde el móvil subí 21 GB de fotos en unos minutos y ahí llegaron los primeros sobresaltos: Immich empezó a indexar y generar miniaturas, el sistema tiró de swap (tenía 4 GB de RAM) y la interfaz se volvió algo “a tirones” hasta que terminó el procesado. Luego apagué el ordenador y al encenderlo minutos después, el disco se había corrompido y Xubuntu se negaba a arrancar. Traté de solucionarlo pero no fui capaz y decidí que la solución más sencilla sería reinstalando el SO junto con Immich, para volver a subir las fotos, que fue lo que acabé haciendo.

## El resultado final
A partir de eso, poco más había que pudiese hacerle al ordenador. Me di cuenta de que iba un poco falto de RAM, así que a fecha de escribir esto estoy planteándome comprar dos RAM sticks de 8 GB para poder aprovechar el máximo que soporta el equipo y que así el procesamiento de fotos fuese más rápido y, por supuesto, con menos riesgos de que todo explote.

También decidí mover el ordenador a la estantería de encima para que estuviese más cerca de los periféricos, lo que también me permitió meter el alargador en la primera estantería, haciendo que ahora la puerta del armario cierre casi por completo y apenas se note. Y por si te lo estás preguntando, el calor del ordenador no es casi notable dentro del armario, por lo que tener la puerta del armario cerrada no influye demasiado en la refrigeración.

**¡Gracias por leer!**