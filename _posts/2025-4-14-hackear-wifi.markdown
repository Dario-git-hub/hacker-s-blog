---
layout: post
title: "Cómo hackear wifis"
date: 2025-4-14 1:04:00 +0000 
categories: hacking wifi linux macos
--- 

Hola, después de mucho tiempo sin vernos, aquí estamos. No he publicado nada en todo este tiempo porque un post que estaba preparando no lo pude hacer. 

Hace 2 post, prometí que habría posts sobre hacking wifi, así que aquí estamos.

El primer paso es comprobar si tu antena wifi soporta modo monitor. Un inciso: yo estaré dando las instrucciones **solo** para linux. Tienes que descargar la suite de [aircrack-ng](https://www.aircrack-ng.org/) y ejecutar este comando: `sudo airmon-ng start <interfaz>` , si no da error, singnifica que esa interfaz  y antena soporta modo monitor y que por lo tanto te puedes saltar el siguiente apartado.

¿Qué antena comprar?

Yo siempre recomendaré antenas usb porque son más fáciles de configurar. La antena que tengo es la [anadol lxuss](https://amzn.eu/d/eYj6SMI) (la grande tiene chipset diferente), elegí esa antena por el chipset: lo que significa que cualquier antena con ese mismo chipset funcionará; pero si no quieres hacer investigaciones, usa esta lista. La siguiente antena que he probado (de un amigo) es esta [tp-link **TL-WN722N](https://amzn.eu/d/5WtYUT0),** funciona bien, nada más que decir. Luego tenemos la [panda pau05](https://a.co/d/c5VYdXQ), esta no la he probado personalmente, pero funciona bien. Cualquier [antena de alpha](https://www.tienda-alfanetwork.com/comprar-c-(adaptadores-wifi-usb).php), son muy caras pero de muy buena calidad y mucho alcance.  Si no te convence ninguna de estas, mira [esta lista](https://hackyourmom.com/en/kibervijna/english-usb-wi-fi-adaptery-z-pidtrymkoyu-rezhymu-monitora-ta-bezdrotovyh-inyekczij/).

Pues bien, hoy solo voy a enseñar 1 manera de obtener la contraseña hackeando wifis. Primero, aclarar que estaré enseñando como obtener la contraseña, porque hackear wifis puede ser desde un mitm hasta hackear el router. 

- airgeddon
    
    Este es el método más fácil, ya que es instalarlo y seguir instrucciones. Lo único especial es que tiene mucha comunidad y es muy customizable. El link es este: [https://github.com/v1s1t0r1sh3r3/airgeddon](https://github.com/v1s1t0r1sh3r3/airgeddon)

{% include welcomments/comments.html website_id = "xFWU7xPtPstabNkuqx8RPIq8a" %}