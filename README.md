# Ollama

Este proyecto contiene contenedores para la aplicación Ollama.

## Requisitos

- Docker
- Docker Compose

## Uso

Para iniciar los contenedores, ejecuta:
```bash
docker compose up -d
```

Para instalar  modelos manualmente, ejecuta:
```bash
docker compose exec ollama ollama pull tinyllama
docker compose  exec ollama ollama pull tinydolphin
```

Para detener los contenedores, ejecuta:
```bash
docker compose down
```

Para acceder al entorno gráfico de la aplicación, se utiliza `webui`, que escucha en el puerto `3000` por defecto.

Para acceder a la interfaz gráfica, abre tu navegador web y dirígete a `http://localhost:3000`.

## Modelos

### Modelos instalados

Para ver los modelos instalados, ejecuta:
```bash
docker compose exec ollama ollama list
```

### Modelos disponibles

Para consultar los modelos disponibles para descargar, visita la página web oficial de Ollama en [https://www.ollama.com/models](https://www.ollama.com/models).