---
title: "Enviar mensajes desde el chat de Roblox a Discord"
description: "Tutorial para aprender cómo enviar mensajes de texto desde el chat de tu juego en Roblox hacia un canal en un servidor de Discord."
lead: "Aprende a enviar mensajes de texto desde el chat de tu juego en Roblox a un canal en tu servidor de Discord."
date: 2022-06-05T11:30:00-05:00
lastmod: 2022-06-05T11:30:00-05:00
draft: false
weight: 50
images: ["crear-servidor-discord.png"]
contributors: ["Darlismeta"]
---

## Entendiendo el problema y la solución

Si estas creando o administrando un juego de Roblox, puedes utilizar el chat de tu juego o cualquier otra entrada, para enviar información a un canal en Discord.
Podrías enviar mensajes con novedades que ocurren en tu juego, como un nuevo logro alcanzado por un jugador o equipo,  crear un sistema de sugerencias o tal vez para un mensaje del administrador.

Para hacer esto, necesitas utilizar el servicio de Roblox llamado [HttpService](https://developer.roblox.com/en-us/api-reference/class/HttpService) y, obviamente un servidor de Discord donde tengas permisos de administrador para crear un WebHook (mas adelante te explicaré que significa eso :wink:).

## 1. Crea un servidor de Discord (si no lo tienes) y configura un Webhook

Primero inicia por crear un servidor de Discord, si aun no lo tienes. 
Es muy simple, solo entra a tu cuenta en la aplicación o web de Discord y en la barra de la izquierda, da clic en el boton verde con signo +, y sigue las instrucciones para crear tu servidor.

<img title="Crear un servidor en Discord" src="crear-servidor-discord.png#center" alt="Crear un servidor en Discord">

Ya que esta creado tu servidor, vamos a crear un **Webhook**.
Este webhook es como un servicio o evento, que esta esperando a que le envien información, para realizar una acción, en este caso, enviar un mensaje a un canal de tu servidor en Discord.

Dirigete a "Ajustes del Servidor", como se observa a continuación:

<img title="Ajustes del Servidor" src="ajustes-de-servidor.png#center" alt="Ajustes del Servidor">

Y posteriormente, ingresa a Integraciones > Crear webhook.

<img title="Crear webhook" src="crear-webhook.png#center" alt="Crear webhook">

Ahora, vamos a configurar nuestro webhook, indicando el nombre con el que se veran los mensajes que lleguen a Discord, y el canal a donde quieres que lleguen los mensajes. Opcionalmente puedes definir tambien una imagen de usuario.

<img title="Configurar webhook" src="configurar-webhook.png#center" alt="Configurar webhook">

Luego de configurarlo, solo resta dar clic en "Copiar URL del webhook", y estaremos listos para ir a programar en Roblox Studio :sunglasses:.

archivo code.js
```lua {hl_lines=[1],linenostart=10}
local var = "1"

print(var)

function(var)
    js.vari(asd)
end
``` 

`{ my code }`