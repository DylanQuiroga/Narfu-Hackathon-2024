# Introducción Crisis Hídrica

Dado a que sequía que asota la región de Coquimbo, Chile, a aumentado en los ultimos años, se nos encomendó la tarea de buscar una solución para optimizar el uso del agua en los agricultores, ya que un gran porcentaje de agua dulce está destinada a la agricultura de la región.

Nuestro equipo conformado por Eliam Villegas [Ingeniería en Computación], Jacob Fredes [Diseño], Diego Alfaro [Ingeniería en Computación], Javiera Vivar [Ingeniería Civil Industrial], Vicente Muñoz [Ingeniería en Computación] y yo, Dylan Quiroga [Ingeniería en Computación] dimos una solución mediante el riego tecnificado para reducir el consumo de agua según las necesidades de la pranta.

# Sensores

Mediante el uso de un ESP32, DHT22 y un sensor de humedad para el suelo construimos un prototipo para tomar la temperatura y humedad del ambiente y, asi mismo, la humedad de las raises de las plantas, el cual son enviados a una base de datos MySQL a un pc de manera local utilizando Flask, un framework de Python para crear aplicaciones web.

<p align="center">
  <img src="https://cdn.discordapp.com/attachments/754792314118995990/1325259632188592169/product_template_29541.png?ex=677b23b6&is=6779d236&hm=c8af8e86c694a14cc885b8419f7cb8d852b436b2354cbc9743d864a610849956&" alt="Imagen 1" width="30%">
  <img src="https://cdn.discordapp.com/attachments/832077522383405076/1325259944802652211/raiquen_product_images_1502.png?ex=677b2400&is=6779d280&hm=183fc2915f1dc973b558b52b02531b079bec59ce9d066d2787f22e425f068045&" alt="Imagen 2" width="30%">
  <img src="https://cdn.discordapp.com/attachments/832077522383405076/1325260013731577918/D_NQ_NP_660380-MLC40189424297_122019-O.webp?ex=677b2411&is=6779d291&hm=799aa97033166ce9e3243c978cb2faba9becf3224de92502d7575a3b211902d5&" alt="Imagen 3" width="30%">
</p>

<p align="center">
  De izquierda a derecha, ESP32, DHT22 y un sensor de humedad para el suelo.
</p>

# Pagina

Aprovechando el uso de Flask, montamos una aplicación web para mostrar datos enviados por el ESP32, información del huerto y una grafica con información con los ultimos 15 datos enviados. Además, utilizamos una API de OpenWeatherMap para obtener información del tiempo y mostrarla (en este caso muestra información de Ovalle ya que el proyecto estaba dirigido para ese lugar)

<p align="center">
  <img src="https://cdn.discordapp.com/attachments/832077522383405076/1325262433757171773/image.png?ex=677b2652&is=6779d4d2&hm=cedb8d38ddd5fbb9c71a29bca528278894a021e3fbf8dae150392d7bccc1aa95&" alt="Imagen 4" width="90%">
</p>

<p align="center">
  Inicio de la página.
</p>

# Resultados

Gracias a este proyecto, logramos obtener el segundo lugar de la Hackathon 2024 de la Universidad de La Serena. Estoy muy agradecido con el equipo por su compromiso y dedicación y, de ser posible, me gustaría volver a colaborar con ellos.

<p align="center">
  <img src="https://media.licdn.com/dms/image/v2/D4D2DAQGmFcer0tw4dQ/profile-treasury-image-shrink_800_800/profile-treasury-image-shrink_800_800/0/1727925598909?e=1736643600&v=beta&t=V5Rb3X05luQpgqT72AxTv2hMkBNdTMuVnCPKxuSXH6I" alt="Imagen 4" width="90%">
</p>

# Cosas que se pueden mejorar

<ol>
  <li><b>Base de datos: </b>El uso de una base de datos en MongoDB puede que sea la mejor opción en este caso si se desean implementar más tipos de sensores sin modificar tanto la estructura.</li>
  <li><b>Login: </b>Para evitar intrusos, se puede implementar un sistema de inicio de sesión.</li>
  <li><b>IA: </b>Se tenia pensado entrenar una inteligencia artificial para tomar desiciones sobre el huerto, no obstante, la falta de tiempo y de información dificultó esta tarea.</li>
  <li><b>Estructura del proyecto: </b>No es la mejor, pero se puede mejorar.</li>
</ol>

# Página

La pagina se adaptó con datos estáticos ya que la base de datos ya no existe y no poseo los componentes para volver a montarlo

<a href="https://narfu.vercel.app/">Clickeame para ir a la página Narfu</a>
