# Investigación HTTP

## Tipos de peticiones HTTP más usados y sus funciones. 

HTTP define un conjunto de métodos de petición para indicar la acción que se desea realizar para un recurso determinado. Aunque estos también pueden ser sustantivos, estos métodos de solicitud a veces son llamados HTTP verbs. Cada uno de ellos implementan una semántica diferente, pero algunas características similares son compartidas por un grupo de ellos: ej. un request method puede ser safe, idempotent, o cacheable.

* **GET**

El método GET  solicita una representación de un recurso específico. Las peticiones que usan el método GET sólo deben recuperar datos.

* **HEAD**

El método HEAD pide una respuesta idéntica a la de una petición GET, pero sin el cuerpo de la respuesta.

* **POST**

El método POST se utiliza para enviar una entidad a un recurso en específico, causando a menudo un cambio en el estado o efectos secundarios en el servidor.

* **PUT**

El modo PUT reemplaza todas las representaciones actuales del recurso de destino con la carga útil de la petición.

* **DELETE**

El método DELETE borra un recurso en específico.

* **CONNECT**

El método CONNECT establece un túnel hacia el servidor identificado por el recurso.

* **OPTIONS**

El método OPTIONS es utilizado para describir las opciones de comunicación para el recurso de destino.

* **TRACE**

El método TRACE  realiza una prueba de bucle de retorno de mensaje a lo largo de la ruta al recurso de destino.

* **PATCH**

El método PATCH  es utilizado para aplicar modificaciones parciales a un recurso.

### *Fuente:* [Mozzilla.Org](https://developer.mozilla.org/es/docs/Web/HTTP/Methods)

## Códigos de respuesta HTTP más comunes y sus significados.

### Tipos de respuesta de los códigos de estado HTTP

En principio, los códigos de estado HTTP se dividen en cinco categorías diferentes, identificadas a su vez, por el primer dígito del código. Por ejemplo, el código de estado HTTP 200 forma parte del tipo de respuesta 2xx, el código 404 del tipo de respuesta 4xx. Esta clasificación se deriva principalmente de la importancia y la función de los códigos de estado, divididos principalmente en 5 tipos:

* **Códigos de estado 1xx– Información:**

 Cuando se envía un código de estado HTTP 1xx, el servidor le notifica al cliente que la petición actual aún continúa. Esta clase reúne y proporciona información sobre el procesamiento y envío de una solicitud.

* **Códigos de estado 2xx – Éxito:**  

Los códigos que comienzan con un 2 informan sobre una operación exitosa. Cuando se reciben este tipo de respuestas quiere decir que la solicitud del cliente fue recibida, comprendida y aceptada. Es muy frecuente que los códigos 2xx sean envíados desde el servidor junto con los datos de la página web deseada. Por lo general, el usuario solo percibe la web solicitada.

* **Códigos de estado 3xx – Redirecciones:**

Aquellos códigos que comienzan con 3 indican que la solicitud ha sido recibida por el servidor. Sin embargo, para asegurar un procesamiento exitoso es necesario que el cliente tome una acción adicional. Este tipo de códigos aparecen principalmente cuando hay redirecciones.

* **Códigos de estado 4xx – Errores del cliente:**

 Cuando aparece un código 4xx quiere decir que se ha presentado un error de cliente. Esto quiere decir que el servidor ha recibido la solicitud, pero esta no se puede llevar a cabo. Una de las principales causas de este tipo de respuestas son las solicitudes defectuosas.  Los usuarios de Internet son informados de este error por medio de una página HTML generada automáticamente.

* **Códigos de estado 5xx –Errores del servidor:**

 El servidor indica un error propio cuando usa un código 5xx. Este tipo de respuestas indican que la solicitud correspondiente está temporalmente deshabilitada o es imposible de llevar a cabo. De nuevo, se generará automáticamente una página en formato HTML.

### Códigos de estado HTTP más importantes

Los códigos de estado HTTP juegan un papel importante para los operadores de una página web o para especialistas en SEO. Los únicos códigos visibles para los visitantes son principalmente los códigos de error del cliente, como el 404 (Not Found), o de error del servidor como el 503 (Service Unavailable), ya que estos siempre se muestran automáticamente como páginas en formato HTML. A menudo es común encontrarse con códigos de estado HTTP que únicamente pueden ser vistos y monitoreados por los administradores con herramientas especiales y extensiones del navegador. Determinar y corregir este tipo de errores es útil para optimizar la experiencia del usuario en una página web y mejorar el ranking en los buscadores. A continuación, presentamos una pequeña selección de los códigos de respuesta más comunes.  Si quieres conocer la lista completa, puedes visitar este registro de códigos de estado.

1. ***Código de estado 200 –OK:*** 

El código de respuesta 200 indica que la solicitud ha sido procesada correctamente. Todos los datos solicitados fueron recibidos por el servidor y se trasmitirán al cliente. Los usuarios de Internet no suelen encontrarse este código.

2. ***Código de estado 301 –Moved Permanently:***

El código 301 significa que los datos solicitados por el cliente ya no se encuentran bajo la misma dirección de Internet, sino que han sido desplazados de manera permanente. Debido a que la ubicación actual del contenido solicitado está incluida en el informe de estado, el navegador web podrá redireccionar la petición a la nueva dirección. Así, el usuario es redireccionado y la antigua dirección pierde validez. Este código suele pasar desapercibido ante los ojos de los usuarios, el único cambio visible es la redirección de la URL en la barra de direcciones.

3. ***Código de estado 302 – Moved Temporarily:***

A diferencia del 301, que hace referencia a una reubicación permanente, el código 302 informa que los datos solicitados están disponibles temporalmente en una dirección diferente. Aquí, la ubicación de la información es especificada, lo que genera una redirección automática. La antigua dirección sigue siendo válida.

4. ***Código de estado 403 – Forbidden:***

El código de estado HTTP 403  indica al cliente que los datos solicitados están protegidos y, por ende, se le ha denegado el acceso debido a la falta de autorización del cliente. En estos casos, el usuario de Internet verá una página en formato HTML generada automáticamente que le informará sobre su falta de permisos para ejecutar la acción.

5. ***Código de estado 404 – Not Found:***

 Cuando el servidor envía el código 404 como respuesta significa que no fue posible encontrar los datos de la página web solicitada en el servidor. Esto sucede cuando la dirección ya no existe o los contenidos han sido trasladados sin especificar la nueva dirección. Cuando a un usuario le aparece el código de estado 404, deberá comprobar si ha introducido la URL de manera correcta en la barra de direcciones. Aquellos enlaces que dirigen a páginas inexistentes suelen conocerse como “enlaces muertos”.

6. ***Código de estado 500 –Internal Server Error:***

 Este tipo de respuesta actúa como un código de estado colectivo para un error inesperado en el servidor. Si el servidor falla y está interrumpiendo la recuperación de los datos solicitados, se emitirá automáticamente el código de estado 500. Además de la respuesta al cliente, el servidor web generará un tipo de registro de error interno en donde se expliquen más detalles sobre el error. Este último debe ser analizado por propietarios de páginas web que estén interesados en hacer las respectivas reparaciones en el software del servidor.

7. ***Código de estado 503 –Service Unavailable:***

 Este código de respuesta indica que el servidor web destinado a proporcionar la información está sobrecargado. Es común que esta respuesta del servidor incluya, además, información sobre cuándo se podrá procesar nuevamente la primera solicitud. Aquí, los usuarios de Internet pueden asumir que el administrador está trabajando en el problema y que, por lo tanto, el servidor estará disponible de nuevo.

 ### Fuente [ionos.es](https://www.ionos.es/digitalguide/hosting/cuestiones-tecnicas/una-mirada-a-los-codigos-de-estado-http-mas-comunes/)