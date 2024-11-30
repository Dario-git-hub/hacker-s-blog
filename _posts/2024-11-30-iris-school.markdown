---
layout: post
title: "iRiS School"
date: 2024-11-30 02:01:59 +0000 
categories: chromebook exploit
---

iRiS School es una extensión muy molesta que nos instaló nuestra escuela en los chromebooks escolares, haciéndolos más lentos, la batería se gasta más rápido, nos bloqueaba webs necesarias para trabajar...etc.
Además, tiene demasiados permisos

![Los exagerados permisos de la extensión iRiS School](/docs/iris-school.png)

Una semana después de que nos instalaran tremenda mierda descubrí un repositorio que se llama [rigtools](https://github.com/Sincereham222/rigtools-newui) que funciona desde la versión de chromeOS 124 hasta la 129. Lo que hacía era: aprovechándose de [websockets de javascript](https://es.javascript.info/websocket), ejecutaba código como una extensión privilegiada. Lo cuál servía para desactivar la extensión de iRiS. 

Al cabo de una semana, los chromebooks se actualizaron a la versión 130 (una en la que ya no funciona el exploit de las rigtools). Yo estaba completamente perdido sobre cómo podría desactivar iRiS. Pero ese mismo lunes, a las 10:30 am, descubrí EL exploit. Ese exploit abusaba de que iRiS usa [service workers](https://www.arsys.es/blog/service-worker) y de que en chrome puedes ver y controlar los services workers en proceso metiéndote en `chrome://serviceworker-internals` y desde allí, solo sería buscar el id de extensión de iRiS y, usando la [API de chrome.management](https://developer.chrome.com/docs/extensions/reference/api/management?hl=es-419), desactivarla. Y lo mejor de todo, es que ese exploit es universal para todas las versiones. Esa manera esta basada en un exploit llamado [LTBEEF](https://compactcow.com/), que tiene mucha comunidad. 

Lo único malo de todo esto, es que al cabo de 2-3 días iRiS volverá y abrá que repetir ete proceso. Esto pasa por un asunto relacionado con la sincronización del servidor.