Titulo: Configurando un servidor NGINX con reverse-proxy y Node JS. Parte 1.
Categoría: Infraestructura, Data Center, Servidores, Configuración, Tutoriales
Tags: dev, servers, desarrollo, nginx, tutoriales, reverse, proxy, servidor, 

# Objetivos 
Hace poco tuve la oportunidad de empezar un curso sobre Node JS. La idea era tener un conocimiento básico del funcionamiento de Node y popder configurar un servidor Express para disponer de una REST API en condiciones para mis distintos laboratorios. 

Con esa idea en mente, inicio esta serie de posts para ir explicando, paso a paso, el proceso que estoy siguiendo para configurar un servidor NGINX en Linux capaz de exponer el acceso de un servicio NodeJS. 

# Fase 1: Instalación 
Para este laboratorio voy a utilizar una distribución de Ubuntu virtualizada.
Para ello voy a lanzar un contenedor (Docker) con una versión limpia de NGINX. 

