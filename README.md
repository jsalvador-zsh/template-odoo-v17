# Instalación y configuración de Odoo 17

## Configuración inicial
1. Instalar docker -> https://docs.docker.com/get-docker/
2. Instalar docker-compose -> https://docs.docker.com/compose/install/

## Instalación de Odoo con Docker
1. Descargar el repositorio usando este comando:
```bash
git clone https://github.com/escuelafullstack template_odoo_docker_compose.git
```

2. Ingresar a la carpeta creada
```bash
cd template-odoo-v17
```

3. Crear los archivos .env y docker-compose.yml
```bash
cp template.env .env
cp template.docker-compose.yml docker-compose.yml
```

4. Editar los parámetros del archivo .env
```bash
Ejm:
WEB_HOST=name_odoo
```

5. Opcional: Editar el archivo docker-compose.ymlen caso se requiera agregar nuevos servicios o modificar parámetros.

6. Ejecutar docker-compose para levantar el contenedor
```bash
docker-compose up -d
```