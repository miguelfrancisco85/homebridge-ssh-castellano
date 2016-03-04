homebridge-ssh-castellano
==============

Es una modificacion de homebridge-ssh pero al castellano intento controlar mi TV Samsung 55H6400

## Instalacion

1. Instalar homebridge: `npm install -g homebridge`
2. Instalar mi plugin homebridge-ssh-castellano: `npm install -g homebridge-ssh-castellano`
3. Pongo un ejemplo de archivo de configuracion que tendra que ser modificado.

## Configuration

"accessories": [

 {
              "accessory": "SSH-CASTELLANO",
              "name": "Television",
              "encender": "./encender-tv.sh",
              "apagar": "./apagar-tv.sh",
              "state": "osascript -e 'tell application \"iTunes\" to get player state'",
              "abrirValue" : "playing",
              "exact_match": true,
              "ssh": {
                "user": "Usuario del Host",
                "host": "IP del Host",
                "port": 22,
                "password": "Tu password",
                "key": "path to private key file"
              }
    }


]
# homebridge-ssh-castellano
