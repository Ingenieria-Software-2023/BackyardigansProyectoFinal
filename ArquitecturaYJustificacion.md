# Arquitectura

Una vez establecidos nuetros requerimientos y funcionalidades y teniendo claro el alcance, tiempo y recursos con los que contamos para el desarrollo de nuestro producto, especificados en el documento [Requerimientos](Requerimientos.md) y en [Readme](Readme.md), consideramos que se requiere una arquitectura que favorezca: la disponibilidad de los servicios, así como la independencia de los mismos; la flexibilidad de los lenguajes de desarrollo, ya que diferentes elementos del equipo se especializan en diferentes herramientas; el fácil desarrollo y despliegue continuo.

<p align="center">
  <img src="https://github.com/Ingenieria-Software-2023/BackyardigansProyectoFinal/assets/101894380/c7351c7b-5fea-4617-8062-677bc6e318b1" style="display: block; margin-left: auto; margin-right: auto;"/>
</p>

Considerando los elementos anteriormente mencionados y las ventajas de cada arquitectura que se muestran en la imágen, decidimos que la arquitectura de *microservicios* es ideal para nuestra página web de una cafetería para nuestros requerimientos por las siguientes razones:

 - **Modularidad**: Cada funcionalidad (inicio de sesión, selección de método de pago, personalización de bebidas, reseñas y calificaciones, y el programa de recompensas) puede desarrollarse como un microservicio independiente. Esto facilita la gestión y el mantenimiento, ya que cada microservicio se puede desarrollar, desplegar, operar y escalar de manera independiente.

- **Escalabilidad**: Si bien esperamos que la aplicación no necesite aumentar su escalabilidad, esta característica ayuda a la manipulación según necesidades de los recursos con que se cuenta. Dado que la demanda de diferentes aspectos del sitio web puede variar (por ejemplo, más actividad en el sistema de pago durante las horas pico), una arquitectura de microservicios permite escalar cada servicio independientemente según la necesidad, optimizando recursos y mejorando el rendimiento.

- **Flexibilidad en el desarrollo**: Los equipos de desarrollo pueden trabajar en diferentes microservicios simultáneamente sin interferir unos con otros. Esto acelera el proceso de desarrollo y permite una mayor experimentación e innovación en cada área del sitio web.

- **Resiliencia**: En un sistema de microservicios, si un servicio falla, no necesariamente provoca la caída de toda la aplicación. Por ejemplo, si el servicio de reseñas está inactivo, los usuarios aún podrán realizar pedidos y personalizar sus bebidas.

- **Integración y despliegue continuos**: Los microservicios facilitan la adopción de prácticas de integración y despliegue continuos, lo que permite lanzar nuevas características y correcciones de errores de manera más rápida y eficiente.

- **Especialización tecnológica**: Cada microservicio puede utilizar el stack tecnológico más adecuado para su propósito específico, lo que permite una optimización más efectiva y la utilización de las mejores herramientas disponibles para cada tarea.

- **Facilidad para actualizar y mejorar**: Al estar dividido en microservicios, el sitio web puede actualizarse por partes sin afectar el funcionamiento global. Esto es especialmente útil para añadir nuevas funcionalidades o mejorar las existentes, como la personalización de bebidas o el programa de lealtad .

En resumen, la arquitectura de microservicios ofrece flexibilidad, escalabilidad, y eficiencia para manejar las diversas y complejas funcionalidades de un sitio web para una cafetería moderna, asegurando al mismo tiempo una experiencia de usuario fluida y confiable. Proponemos una distribución de nuestros servicios de la siguiente manera: 

<p align="center">
  <img src="Arquitectura -1.jpg" style="display: block; margin-left: auto; margin-right: auto;"/>
</p>




