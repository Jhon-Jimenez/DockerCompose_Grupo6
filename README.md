# Desarrollo con Docker Compose

## Integrantes - Grupo 6

- Jhon Janner Jimenez Zuleta
- Sergio Rodriguez Cabana

## Descripción

Este proyecto configura un entorno utilizando Docker Compose, que consta de tres contenedores interconectados:

1. Proxy (Nginx): Funciona como un proxy reverso, gestionando las solicitudes que llegan al puerto 80.
2. Aplicación Web 1: Ejecutada en el contenedor app1.
3. Aplicación Web 2: Ejecutada en el contenedor app2.

## Estructura del Proyecto

```bash
DockerCompose_Grupo6/
│
├── docker-compose.yml       # Configuración de Docker Compose
├── nginx.conf               # Configuración de Nginx como proxy
├── App1                     # Contiene la Aplicación Web 1
│   ├── LogisimWeb/           # Archivos de la Aplicación Web 1
│   └── Dockerfile
└── App2                     # Contiene la Aplicación Web 2
    ├── Sintaxify/          # Archivos de la Aplicación Web 2
    └── Dockerfile
```

## Instrucciones de Uso

### Configuración Inicial

1. **Clona o descarga el repositorio**: Obtén los archivos necesarios para el proyecto.

2. **Verifica que Docker Compose esté instalado**: Confirma la instalación con el siguiente comando:

```bash
docker-compose --version
```
### Ejecución
1. **Accede al directorio del proyecto**:

```bash
cd DockerCompose_Grupo6
```

2. **Inicia los contenedores**:

```bash
docker-compose up --build
```

Este comando construirá y lanzará los contenedores definidos en el archivo docker-compose.yml.

### Acceso a las Aplicaciones

Abre tu navegador web y visita las siguientes URLs:

* Página de bienvenida: http://localhost:8081
* Aplicación Web 1: http://localhost/c2/
* Aplicación Web 2: http://localhost/c3/
