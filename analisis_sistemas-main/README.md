# Proyecto final de analisis y sistemas
- Lisbeth Mendoza 2021 1072
- Lizandro
- "UCATECI"

## Introduccion
Se analizara y aran prubas de lo que es una pagina con todos sus componentes, en la que vamos a analizar en especifico contiene, nginx, postgres, api, redis, client-react y worker. Con la finalidad de comprender para que sirve cada uno de estos y el porque se estan utilizando. 
## Teoria
### Postgres
Es una base de datos sql relacional que nos sirve en este caso para poder guardar los datos del cliente. 

### Nginx
Nos permite controlar en una sola direccion varios puertos, en este caso lo hace en, cliente, servidor y el api de la app.

### API Rest y Node.js
 API Rest son el puente de comunicación entre frontend y backend. El recurso que consultamos desde el frontend para responder a las interacciones de un usuario. Y la respuesta que entrega el backend después de procesar solicitudes y consultar bases de datos.

 Node.js es un entorno que trabaja en tiempo de ejecución, de código abierto, multi-plataforma, que permite a los desarrolladores crear toda clase de herramientas de lado servidor y aplicaciones. 

### React 
Ayuda a crear interfaces de usuario interactivas de forma sencilla. En este caso junto con HTML Y Js

### Redis
Es un almacén de estructura de datos de valores de clave en memoria rápido y de código abierto. Redis incorpora un conjunto de estructuras de datos en memoria versátiles

### Docker 
Te permite utilizarlo como un servidor atravez de contenedores por separado. 

## Conclusion
  client/public= Se encarga de la interfaz sencilla, como lo es el icono y titulo de la pagina y formato de esto. 
  client/src= Sobre envio y acualizacion de informacion (Fib.js) y algunos diseños graficos

 nginx/default.conf= Para la conexion de los diferentes servidores y puertos

 Server/index.js y key.js= Van de la mano y control a lo que resive la base de datos dado por los clientes

 Worker/index.js y key.js= calcula el numero dado y la informacion la guarda en la base de datos.  

 Cada uno con su "DOCKERFILE.DEV" con la variacion del From, para especificar la imagen sobre la que los pasos e imágenes siguientes se desarrollan en el sistema. (La imagen ejecuta un codigo detro de un contenedor)

 # Video
 
## Problemas
- Al escribir string la pagina deja de funcionar 
- Graficamente no es muy entendible 
- Para  los numeros igual y menores que 0 te va a devolver siempre un 1
- Cuando agregas un valor nuevo no se actualiza la pagina
- No especifica que el limite es hasta el numero 40 