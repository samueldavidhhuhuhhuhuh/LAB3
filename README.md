# Proyecto: Comunicación con Sockets TCP

Este proyecto implementa un **servidor** y un **cliente** en Python para enviar y recibir mensajes mediante sockets TCP.

## Estructura del proyecto

- `server.py`: Servidor TCP que maneja múltiples clientes y soporta mensajes privados/broadcast.
- `client.py`: Cliente que permite enviar mensajes, privados o globales, y recibirlos en consola.
- `utils.py`: Funciones de utilidad (framing, hash MD5, envío/recepción).
- `docs/`: Documentación (diagramas, notas, pruebas).
- `tests/`: Scripts de prueba de conexión e integridad.
- `captures/`: Carpeta para logs y capturas de pantalla.

## Requisitos

- Python 3.9+
- No requiere librerías externas (usa `socket`, `hashlib`, `json`, incluidas en la librería estándar).

## Ejecución

1. Ejecuta el servidor:
   ```bash
   python3 server.py
   ```

2. Ejecuta un cliente:
   ```bash
   python3 client.py
   ```

3. Usa los comandos en el cliente:
   - `/list`: lista de usuarios conectados.
   - `/msg usuario mensaje`: envía mensaje privado.
   - Texto libre: broadcast a todos los usuarios.
   - `/quit`: salir.

