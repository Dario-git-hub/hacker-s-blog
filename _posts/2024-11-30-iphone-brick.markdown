---
layout: post
title: "Brickeé mi móvil"
date: 2024-11-30 04:50:00 +0000 
categories: linux ios raspberrypi
---

Mi setup consiste en un raspberry pi 4 con kali linux y ya. El caso es que hice una copia de seguridad del iphone al raspberry usando [idevice](https://libimobiledevice.org/), que es una herramienta que te permite comunicarte de manera fácil con ios desde linux o windows. Después de hacer la copia, empecé a probar comandos de idevice, lo que provocó que me cargase (no se ni como) la partición de iBoot. iBoot es el firmware con el que arrancan los dispositivos de apple. Y el móvil solo se quedaba en la pantalla de restaurar con itunes. 

![https://cdsassets.apple.com/live/7WUAS350/images/ios/ios13-iphone-xs-restore-iphone.jpg](https://cdsassets.apple.com/live/7WUAS350/images/ios/ios13-iphone-xs-restore-iphone.jpg)

Lo que se me ocurrió fue buscar por google el firmware original. Lo encontré y lo dejé flasheando mientras comía. Cuando volví de comer, vi la pantalla de bloqueo y me alegré. Por si la queréis, aquí tenéis [la web para los firmware](https://ipsw.me/). 

Que conste que ya se que el de la foto es el xs y yo tengo el 7, pero es el único que se veía bien.