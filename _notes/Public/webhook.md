---
title: Webhook
feed: show
date: 10-03-2025
tags:
  - devOps
  - facebook
curso:
---
Un webhook es simplemente un mecanismo que, al ocurrir un evento en Facebook, envía automáticamente la información a una URL que tú configuras. Ahí, tú decides qué hacer con esos datos, por ejemplo, almacenarlos o procesarlos.

# Ejemplo con guardado de Log
```Python
import logging
from flask import Flask, request, jsonify

app = Flask(__name__)

# Configuración de logging: guarda los logs en "webhook.log" y también los muestra en consola
logging.basicConfig(
    level=logging.INFO,
    format='%(asctime)s %(levelname)s %(message)s',
    handlers=[
        logging.FileHandler("webhook.log"),
        logging.StreamHandler()
    ]
)

VERIFY_TOKEN = 'mi_token_secreto'

@app.route('/webhook', methods=['GET', 'POST'])
def webhook():
    if request.method == 'GET':
        # Verificación inicial de Facebook
        token = request.args.get('hub.verify_token')
        challenge = request.args.get('hub.challenge')
        if token == VERIFY_TOKEN:
            return challenge
        else:
            return 'Token de verificación inválido', 403

    elif request.method == 'POST':
        # Recibe los datos enviados por Facebook
        data = request.get_json()
        # Guarda la información en el log
        logging.info("Datos recibidos: %s", data)
        # Aquí puedes agregar código adicional para almacenar en base de datos, etc.
        return jsonify(status='success'), 200

if __name__ == '__main__':
    app.run(debug=True, port=5000)

```

