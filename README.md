# MUSICA en Bot Desinger For Discord

- **Primer Paso**
Obten el repositorio en tus manos.

   - Video tutorial [click aqui](https://github.com/IzanaonYT/MusicScript/blob/main/Tutos/githubtuto.mp4)
- **Segundo Paso**
Obten un Host Gratuito con un subdominio para que el bot funcione correctamente.
Vamos usar [Railway.app](https://railway.app), recuerda inicar sesion con tu cuenta git hub

   - Video tutorial [click aqui](https://streamable.com/9qtqhr)
   
    No olvides poner la variable de entorno llamada "DISCORD_TOKEN" mas el el valor de tu token de tu bot.
    Recuerda esperar que la API cargue correctamente o causaras problemas en el bot.


- **Tercer Paso**
Usa los codigos pero recuerda ejecutarlo en un canal de voz y estar unido a este, que esperas para escuchar tu musica preferida?, asi de simple y gracias por ser parte de BDS World

```python
$onlyIf[$message!=;Escribe algo para escuchar]
$var[dominio; tu url de render aqui]
$var[json;{
    "guild_id": $guildID,
    "channel_id": $channelID,
    "user_id": $authorID,
    "url": "$url[encode;$message]"
}]
$httpPost[$var[dominio]/api/musica/;$var[json]]
$httpResult
```

- Codigos mas avanzados con el repositorio: [Click aqui](https://github.com/IzanaonYT/MusicScript/blob/main/Tutos/codes_bdfd.md)
