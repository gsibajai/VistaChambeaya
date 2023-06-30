# Descripción de pantallas de Chambeaya


## Descripción de las vistas correspondientes al grupo 01
## Vista de Mis Datos
![image](https://raw.githubusercontent.com/rapulidom/sources/main/images/varias/misdatos.png)

## Componente de mis datos Vista

### Datos Fijos
- Título de la página
### Datos Dinámicos
- Nombre del trabajador
- Oficio del trabajador
- Cantidad de calificaciones
### Componentes
- Imagen de perfil
Este componente tendrá la opción de cambiarse al dar clic se abrirá el Cropper y se remplazará la imagen.
 
- Calificación
Componente donde se le pasara un número del 0 al 10 y este retornara en estrellas la calificación solicitada 10 = 5 estrellas y 0 = 0 estrellas 5 = 2.5 estrellas

- Card de últimos trabajos
    - Título
    - Usuario que dio la evaluación
    - comentario
    - Componente de calificación en estrellas
    - Link para ir al detalle del trabajo
- Botón para ir a la vista de edición de información.


# Vista de Mis Datos Edición
![image](https://raw.githubusercontent.com/rapulidom/sources/main/images/varias/misdatosedicion.png)

- Formulario con los campos
  - Texto:
    - Nombre completo
    - Dirección
    - Correo electrónico
    - Número de teléfono
  - Boleanos:
    - Servicio a domicilio
    - Emite Facturas
  - MultiSelect Checkbox:
    - Métodos de pago:
      - Efectivo
      - Tarjeta
      - Da Crédito
      - Trasferencia Bancaria

# Vista de Formulario de pago
## Componente de formulario a pasos
### Paso 1 Selección de plan

![image](https://raw.githubusercontent.com/rapulidom/sources/main/images/varias/plan1.png)

3 Opciones de los planes con componentes

Componente:
- Imagen relacionada con el plan
- Título del plan
- Costo del plan
- Frecuencia de pago
- Botón para seleccionar

Componente colapsado
- Nombre del plan
- Costo
- Botón para cambiar selección
  
### Paso 2 Selección de Tarjeta
![image](https://raw.githubusercontent.com/rapulidom/sources/main/images/varias/plan2.png)

Importación de tarjetas guardadas

Componente:
- imagen de tarjeta
- Dueño de tarjeta
- Últimos 4 dígitos
- Botón para más detalles

- botón / link para agregar otro método de pago, muestra modal de tarjetas guardadas 

### Paso 3 Confirmar
![image](https://raw.githubusercontent.com/rapulidom/sources/main/images/varias/plan3.png)

- Checkbox:
  - Aceptar términos y condiciones
  - Se requiere factura



# Vista de ingreso de tarjeta
![image](https://raw.githubusercontent.com/rapulidom/sources/main/images/varias/tarjeta1.png)
## Selección de Tarjeta

Importación de tarjetas guardadas

Componente:
- imagen de tarjeta
- Dueño de tarjeta
- Últimos 4 dígitos
- Botón para más detalles

- botón / link para agregar otro método de pago, muestra modal de tarjetas guardadas 

![image](https://raw.githubusercontent.com/rapulidom/sources/main/images/varias/tarjeta2.png)
- Formulario
  - Número de tarjeta
  - Nombre en tarjeta
  - Fecha de expiración
  - CVC
  - Botón para agregar

## Descripción de las vistas correspondientes al grupo 02
#### Menú lateral (Sidebar)
Tiene por objetivo ofrecerle al usuario un conjunto de accesos directos para que acceda a las principales secciones de la plataforma que permiten editar y registrar datos.

Este menú se va a localizar en la parte izquierda de la pantalla y será mostrado solo en aquellas páginas que requieren de una previa autenticación. Este sidebar se compone de diversos enlaces acompañados de iconos que ilustran cada una de las opciones.
<p align="center">
  <img src="https://github.com/ejreyesh/ejreyesh-prueba/blob/main/src/images/sidebar.png" width="150px"/>
</p>
<br/>

#### Registrar un servicio
Esta página permite que los usuarios puedan registrar el servicio que ofrecen, sin embargo, para poder acceder a este apartado del sistema es necesario tener un pago vigente de los planes que se ofrecen en la plataforma.

La vista incluye la presencia del sidebar en la parte izquierda de la pantalla, sin embargo, el elemento más importante es el formulario en donde se ingresan los datos del servicio ofrecido. Dicho formulario se divide en 3 secciones; la primera de ellas contiene los campos para ingresar el título del servicio, una descripción detallada, la categoría del servicio ofrecido y las actividades que el anunciante realiza.
<p align="center">
  <img src="https://github.com/ejreyesh/ejreyesh-prueba/blob/main/src/images/registro-servicio-1.png" width="550px"/>
</p>
<br/>

En la segunda sección del formulario, se cuenta con un campo para ingresar la dirección en la que se ubica el taller del anunciante, esto con la finalidad de que el contratante pueda ir a hacer un trato directo si así lo desea.

Además, en esta parte del formulario se permite al usuario subir imágenes donde muestre evidencias de su trabajo. Para esta acción se hará uso de un componente `Image Cropper` para el usuario pueda editar sus fotografías dentro de la misma plataforma.
<p align="center">
  <img src="https://github.com/ejreyesh/ejreyesh-prueba/blob/main/src/images/registro-servicio-2.png" width="550px"/>
</p>
<br/>

En la tercera sección del formulario para el registro de un servicio, solo se muestra un resumen de la información ingresada por el usuario, esto con el propósito de que el anunciante verifique el contenido de su publicación antes de que sea guardada. Es importante mencionar que el formulario cuenta con los mecanismos necesarios para avanzar y regresar a alguna de sus secciones.
<p align="center">
  <img src="https://github.com/ejreyesh/ejreyesh-prueba/blob/main/src/images/registro-servicio-3.png" width="550px"/>
</p>
<br/>

#### Listado de oficios
Esta vista contempla un listado de `cards` con la información más relevante de cada uno de los oficios que se tienen registrados dentro de la plataforma, por cada oficio registrado se podrá visualizar el nombre, su descripción y una imagen ilustrativa, así mismo, se tendrá un enlace para poder ver a detalle toda la información del registro.
<p align="center">
  <img src="https://github.com/ejreyesh/ejreyesh-prueba/blob/main/src/images/listado-oficios.png" width="550px"/>
</p>
<br/>

#### Visualización de un oficio
Esta vista es de carácter informativo, ya que muestra toda la información relacionada con un determinado oficio. Dentro de los elementos utilizados están los cuadros de texto, una imagen y un listado, además, si se tiene el rol de administrador, se habilitará el botón para editar el registro de los oficios.
<p align="center">
  <img src="https://github.com/ejreyesh/ejreyesh-prueba/blob/main/src/images/lectura-oficio.png" width="550px"/>
</p>
<br/>

#### Registrar o editar un oficio
A esta vista solo podrán acceder los administradores de la plataforma, ya que su objetivo es permitir registrar o editar la información de los oficios almacenados dentro del sistema. La vista se compone de un formulario en el que se podrá subir una imagen alusiva al oficio, un nombre, una descripción y además, una serie de actividades que se relacionan con el oficio.
<p align="center">
  <img src="https://github.com/ejreyesh/ejreyesh-prueba/blob/main/src/images/registro-oficio.png" width="550px"/>
</p>
<br/>

Las actividades relacionadas con el oficio, se podrán eliminar y agregar según sean necesarias, para eliminarlas solo hay que presionar el botón rojo que se antepone al texto de la actividad. Y para agregar nuevas actividades, es necesario hacer uso del modal que se despliega al momento de presionar el botón `Agregar nueva actividad`. Para guardar los cambios, solo se debe presionar el botón `Guardar`.
<p align="center">
  <img src="https://github.com/ejreyesh/ejreyesh-prueba/blob/main/src/images/registro-oficio-modal.png" width="550px"/>
</p>
<br/>

## Descripción de las vistas correspondientes al grupo 03

### Registro 

Página de registro 

La página de registro es la página donde el usuario podrá crear su cuenta y cuenta con los siguientes elementos:

1. Logo de la compañia del lado superior izquierdo el cual redirigira a home en caso de que solo quieras ver la página sin tener cuenta

2. Botón de inicio de sesión del lado superior derecho el cual redirigira al formulario para iniciar sesion en caso de que ya se cuente con un usuario

3. Imagen de fondo

4. Formulario de registro en el cual encontramos 3 diferentes inputs de correo, nick y contraseña los cuales contarán con validaciones.

5. Icono de ojo en caso de querer ver la contraseña que se esta ingresando para la creación de la cuenta

6. Captcha para evitar el spam de cuentas

7.  Botón de continuar que enviara la información del formulario y en caso de tener los campos correctos redireccionara a la página de registro2

8. Footer

<p align="center">
  <img src="https://raw.githubusercontent.com/gsibajai/VistaChambeaya/main/Imagenes/Registro1.png" width="550px"/>
</p>

### Registro2

La página de registro2 es la página donde el usuario ingresará el token para poder terminar con el proceso de creación de su cuenta:

1. Logo de la compañia del lado superior izquierdo el cual redirigira a home en caso de que solo quieras ver la página sin tener cuenta

2. Botón de inicio de sesión del lado superior derecho el cual redirigira al formulario para iniciar sesion en caso de que ya se cuente con un usuario

3. Imagen de fondo

4. Texto de indicaciones para ingresar el Token

5. Input que recibira el token enviado al correo electronico

6. Botón para enviar formulario

7. Footer.

<p align="center">
  <img src="https://raw.githubusercontent.com/gsibajai/VistaChambeaya/main/Imagenes/Registro2.png" width="550px"/>
</p>

### Página de valoración de anuncio Vista

La página de valoración de anuncio estara integrada para calificar al trabajador el cual ya presto los servicios esta página incluirá los siguientes elementos
 
1.  Logo de la compañia del lado superior izquierdo el cual redirigira al menú principal

2. Imagen de fondo

3. Imagen de perfil del prestador del servicio

4. Nombre del prestador del servicio

5. Profesion del prestador del  servicio

6. Nombre y fecha de realización del servicio

7.  Calificacion y comentarios asignados o por asignar

8. Icono de lapiz para calificar en caso de que este pendiente.

9. footer

<p align="center">
  <img src="https://raw.githubusercontent.com/gsibajai/VistaChambeaya/main/Imagenes/ValoracionAnuncioVista.png" width="550px"/>
</p>

Página de valoración de anuncio Edición

La página de valoración de anuncio estará integrada para calificar al trabajador el cual ya presto los servicios esta página incluirá los siguientes elementos
 
1.  Logo de la compañia del lado superior izquierdo el cual redirigira al menú principal

2. Imagen de fondo

3. Imagen de perfil del prestador del servicio

4. Nombre del prestador del servicio

5. Profesion del prestador del  servicio

6. Nombre y fecha de realización del servicio

7.  Input para asignar calificación al servicio

8. Cajon para agregar comentarios

9. Botón para enviar evaluación 

9. footer

<p align="center">
  <img src="https://raw.githubusercontent.com/gsibajai/VistaChambeaya/main/Imagenes/ValoracionAnuncioEdit.png" width="550px"/>
</p>

### Página valoración del cliente

La página de valoración del cliente esta implementada para que los trabajadores puedan evaluar a las personas que los contrataron  esta página incluye los siguientes apartados:


1.  Logo de la compañia del lado superior izquierdo el cual redirigira al menú principal

2. Imagen de fondo

3. Imagen de perfil del cliente 

4. Nombre del cliente

5. Nombre y fecha de realización del servicio

6.  Calificacion y comentarios asignados o por asignar

7. Icono de lapiz para calificar en caso de que este pendiente.

8. footer

<p align="center">
  <img src="https://raw.githubusercontent.com/gsibajai/VistaChambeaya/main/Imagenes/ValoracionUsuarioVista.png" width="550px"/>
</p>


### Página valoración del cliente Edición

La página de valoración del cliente esta implementada para que los trabajadores puedan evaluar a las personas que los contrataron  esta página incluye los siguientes apartados:

1.  Logo de la compañia del lado superior izquierdo el cual redirigira al menú principal

2. Imagen de fondo

3. Imagen de perfil del cliente

4. Nombre del cliente

5. Nombre y fecha de realización del servicio

6.  Input para asignar calificación al servicio

7. Cajon para agregar comentarios

8. Botón para enviar evaluación 

9. footer

<p align="center">
  <img src="https://raw.githubusercontent.com/gsibajai/VistaChambeaya/main/Imagenes/ValoracionUsuarioEdit.png" width="550px"/>
</p>


## Descripción de las vistas correspondientes al grupo 04

### Pagina de publicaciones pendientes

En esta página, en la parte superior, no se agregó el estilo del encabezado; sin embargo, del lado izquierdo se colocó el logo de la página y del lado derecho el nombre del usuario que está en sesión en ese momento.

En el cuerpo:

- Se agregó una imagen de fondo tipo papel tapiz.

- Como encabezado, se muestra el título de la página, que en este caso es "Publicaciones pendientes".

- En la parte inferior del título, se encuentran tarjetas que contienen algunos datos del cliente que desea solicitar el servicio, como la foto de perfil, el nombre, la categoría a la que pertenece su servicio y un botón llamado "ver publicación" (Estas tarjetas solo corresponden a los servicios que requieren aceptación o rechazo, por lo que no hay un número específico de cuántas tarjetas hay).

    - Al presionar el botón "ver publicación", se abre una ventana modal que muestra los datos completos de la publicación de este servicio, que incluyen:

      - Título del servicio.
      - Descripción detallada del servicio.
      - Categoría del oficio.
      - Actividades que realiza.
      - Dirección donde se encuentra el servicio.
      - Un carrusel de imágenes que el cliente ha subido para que los posibles contratantes puedan ver su servicio.
      - Además, hay dos botones:

        - Uno para aceptar la publicación del servicio y que quede publicado.
        - El otro para rechazarla en caso de haber inconsistencias en los datos. Si se presiona este botón, se abre otro modal que muestra un título llamado "Motivo del rechazo". Luego, se incluye un campo de entrada etiquetado como "comentarios", donde se puede agregar el motivo del rechazo. Por último, hay dos botones: "enviar", para enviar los comentarios al cliente, y "cancelar", para regresar a la ventana anterior.

- Por último, también se incluye un numerador de páginas. En caso de haber muchas publicaciones, se podrá cambiar de página para ver las siguientes.


En el footer se encuentran los siguientes enlaces:

Términos y condiciones.
Avisos de privacidad.
Accesibilidad.
Ayuda.

<img width="452" alt="image" src="https://raw.githubusercontent.com/rusanchezg/templates-images/main/paginas/publicaciones-pendientes.png">

<img width="453" alt="image" src="https://raw.githubusercontent.com/rusanchezg/templates-images/main/paginas/publicaciones-pendientes2.png">

<img width="282" alt="image" src="https://raw.githubusercontent.com/rusanchezg/templates-images/main/paginas/publicaciones-pendientes3.png">


### La página Opiniones-Historial

La página "Opiniones-Historial" tiene la siguiente estructura:

En el header, se encuentra únicamente el logo de la página en la parte superior izquierda.

En el body, hay una división de dos columnas:

Columna izquierda: Menú con los siguientes campos:

Mis datos.
Seguridad.
Facturación.
Tarjeta de crédito.
Configuración.
Dirección.
Opiniones.

Columna derecha: Encabezado con el título de la página, "Opiniones" (tomado del menú de la columna izquierda). A continuación, se muestra un subtitulo llamado "Historial". Posteriormente, se presentan cards que contienen la foto del usuario calificado, su nombre y el título del trabajo realizado. También se muestra la puntuación otorgada y un carrusel que muestra las imágenes de los trabajos realizados, una por una.

Por último, en el footer se encuentran los siguientes enlaces:

Términos y condiciones.
Aviso de privacidad.
Accesibilidad.
Ayuda.

<img width="448" alt="image" src="https://raw.githubusercontent.com/rusanchezg/templates-images/main/paginas/opiniones-historial.png">


### Opiniones por calificar

La página "Opiniones-pendientes" tiene la siguiente estructura:

En el header, se encuentra únicamente el logo de la página en la parte superior izquierda.

En el body, hay una división de dos columnas:

Columna izquierda: Menú con los siguientes campos:

Mis datos.
Seguridad.
Facturación.
Tarjeta de crédito.
Configuración.
Dirección.
Opiniones.

En la sección llamada "Pendientes", se muestran las tarjetas de los trabajos del usuario que aún no han sido calificados. Cada tarjeta incluye la foto del usuario, su nombre y una breve descripción del trabajo realizado. A diferencia del historial, estas tarjetas de trabajos pendientes cuentan con un botón que permite calificar el servicio. Al hacer clic en este botón, el usuario puede asignar una puntuación al trabajo realizado.
Además, en esta sección también se incluye un carrusel que muestra de forma individual las imágenes

Por último, en el footer se encuentran los siguientes enlaces:

Términos y condiciones.
Aviso de privacidad.
Accesibilidad.
Ayuda.

<img width="433" alt="image" src="https://raw.githubusercontent.com/rusanchezg/templates-images/main/paginas/opiniones-pendientes.png">


### Pagina Contratar

En esta página, el encabezado (header) solo muestra el logotipo de la página en la parte superior derecha.

En el cuerpo (body) se encuentra lo siguiente:

- Un fondo que simula un papel tapiz.
- A continuación, se muestra una tarjeta (card) que contiene la foto de perfil del usuario y su categoría.
- A continuación, se muestra la calificación otorgada en forma de estrellas, junto con la cantidad de calificaciones recibidas.
- Seguidamente, se presentan los dos últimos servicios realizados, acompañados de imágenes que muestran los trabajos realizados.
- También se incluye una descripción de las actividades que realiza el usuario y una descripción de su servicio.
- Se ha añadido un botón para contratar el servicio.
- Luego de esto, solo se encuentra la sección de preguntas y respuestas.


Por último, en el footer se encuentran los siguientes enlaces:

Términos y condiciones.
Aviso de privacidad.
Accesibilidad.
Ayuda.

<img width="203" alt="image" src="https://raw.githubusercontent.com/rusanchezg/templates-images/main/paginas/contratar.png">


## Descripción de las vistas correspondientes al grupo 05

## Header

![Screenshot from 2023-06-29 19-54-46](https://github.com/iecamachog/template-and-images/assets/132395694/aaa39690-6ab5-4d76-b48e-60382d350a4b)


Es un componente que se mostrará en todas las páginas en la parte superior, este componente tiene 3 versiones, dependiendo la página mostrada, será el header, las versiones son las siguiente:
Header con solo el **logo** en la parte izquierda.
Header con logo en la parte izquierda, icono de usuario de lado derecho y a su lado etiqueta de **inicia sesión**, esta etiqueta al darle clic, se redirigirá a la página de **login**.

## Footer

![Screenshot from 2023-06-29 19-55-32](https://github.com/iecamachog/template-and-images/assets/132395694/6e0bdab2-d5ab-4f94-bd46-9a4adeae3d98)


Es un componente que se mostrará en todas las páginas en la parte inferior de todas las páginas, este componente nunca cambiara, el contenido del footer es una etiqueta de **Términos y condiciones**, **Avisos de privacidad**, **Accesibilidad**, **Ayuda** y leyenda **Copyright © 1999-2023 El presente canal de instrucción o ambiente, es operado por DeRemate.Com de México, S. de R.L. de C.V. identificada bajo la marca comercial “Chambeaya". Insurgentes Sur 1602 Piso 9 Suite 900, Crédito Constructor Benito Juarez, 03940 Ciudad de México, CDMX, Mexico**

## Página principal (home)

![Screenshot from 2023-06-29 19-56-25](https://github.com/iecamachog/template-and-images/assets/132395694/7880113f-4eff-432b-a5e1-1afcb0727987)


Esta página será la primera en mostrarse una vez que se ingrese la url de la página, el contenido de la página es una **barra de búsqueda**, **carrusel de cards cada uno con una imagen y titulo del oficio, carrusel de cards con una imagen, foto de perfil, nombre y servicio del usuario trabajador**, leyenda de **Ofrecer un servicio. Para poder unirte al equipo de chambeaya debes dar de alta tu servicio en la plataforma, únicamente busca tu oficio, ¡llenar el formulario de las especificaciones y listo! **, leyenda de **¿Tienes algún comentario queja o sugerencia?** y debajo un botón de **Crear comentario**.

La barra de búsqueda listara los oficios de interés del usuario.
Carrusel de cards de oficio al darle clic se abrirá la página de lista de trabajadores, que comparten el oficio seleccionado.
Carrusel de cards de trabajador al darle clic se abrirá una nueva página de detalles del servicio.
Botón de Crear comentario, desplegara un modal de enviar comentario.

## Acerca de nosotros 

![Screenshot from 2023-06-29 19-57-13](https://github.com/iecamachog/template-and-images/assets/132395694/f4c1472e-eea8-4c80-966f-cce66ab0ed7d)


Es una página será meramente informativa, tendrá el título de **Acerca de nosotros**, el contenido principal es una leyenda, la cual es:

*Nuestra filosofía:

El resultado de la colaboración, es mayor al total de la suma de las partes. Ayudando a los demás, nos ayudamos a nosotros mismos. Creemos en la responsabilidad de abrir el camino para que quienes nos sigan lleguen aún más lejos; Creemos en que el sol sale para todos.

Nuestra misión:

Encontrar soluciones innovadoras y accesibles para grandes retos, y así contribuir a que la gente sea más productiva y feliz.

Si eres un profesional en un oficio ¡tienes que estar en este sitio!

Regístrate totalmente gratis Chambeaya, tus servicios de profesional lo aras llegar a muchas personas fácil y rápido. *

Por último, un botón **Volver a página principal** que redirige a la página principal.

## Preguntas frecuentes

![Screenshot from 2023-06-29 19-58-15](https://github.com/iecamachog/template-and-images/assets/132395694/6b94ca7a-52b9-4ef0-9505-453c384103b2)


Sera un componente el cual llevara un registro de las preguntas que le han realizado al trabajador sobre su servicio, estas preguntas ayudaran a los clientes a identificar información más detallada sobre un servicio.
El contenido de este componente es foto de perfil del cliente y un cuadro de texto con relación a un comentario del cliente, foto de perfil del trabajador y un cuadro de texto con relación a la respuesta del cliente cuadro de texto para ingresar una nueva pregunta y botón para enviar nueva pregunta.

 
##  Detalle de mis servicios

![Screenshot from 2023-06-29 19-58-52](https://github.com/iecamachog/template-and-images/assets/132395694/bc675709-462a-4ccc-b339-da0bbb90ab1e)


Esta página sirve como una plataforma para mostrar información relevante sobre un trabajador específico, incluyendo detalles sobre su oficio, servicios que ofrece y trabajos previos realizados. Algunos de los elementos que se pueden encontrar en esta página incluyen:

Información del trabajador: Esta sección proporciona detalles sobre el trabajador, como su nombre, experiencia laboral y posiblemente información de contacto.

Tema del servicio: Aquí se especifica el tipo de servicio que ofrece el trabajador. Puede incluir una amplia gama de oficios, como plomería, carpintería, jardinería, pintura, entre otros.

Imágenes de los trabajos realizados: Se muestran fotografías o imágenes que representan los trabajos previos realizados por el trabajador. Esto brinda a los clientes potenciales una idea visual de la calidad y el tipo de trabajo que el trabajador puede realizar.

Descripción detallada: En esta sección, se proporciona una descripción detallada de los servicios ofrecidos por el trabajador. Esto puede incluir información sobre las técnicas utilizadas, los materiales utilizados y cualquier especialización adicional que el trabajador pueda tener.

Actividades que realiza: Aquí se enumeran las diversas actividades o tareas que el trabajador puede realizar en el contexto de su oficio. Por ejemplo, un plomero puede realizar reparaciones de tuberías, instalación de grifos, inspecciones de sistemas de fontanería, etc.

Categoría del oficio: Se indica la categoría o tipo de oficio al que pertenece el trabajador. Esto ayuda a los clientes a identificar rápidamente si el trabajador se especializa en el área de servicio que están buscando.

Tipo de pago: Se menciona cómo se lleva a cabo el proceso de pago por los servicios del trabajador. Esto puede incluir información sobre tarifas por hora, tarifas fijas o cualquier otro método de pago aceptado.

Calificación: Se muestra la calificación del trabajador, que es la suma de las calificaciones dadas por los clientes anteriores. Esto brinda a los nuevos clientes una indicación de la satisfacción de los clientes anteriores con los servicios proporcionados.

Dirección del taller: Si el trabajador tiene un taller o una ubicación física donde realiza su trabajo, se proporciona la dirección en esta sección. Esto es útil para los clientes que deseen visitar o contactar al trabajador en persona.

En resumen, esta página proporciona una visión general completa de un trabajador, sus servicios, trabajos anteriores, información de contacto y otros detalles relevantes para los clientes que buscan contratar sus servicios.

## Detalle de mis servicios editar información 

![Screenshot from 2023-06-29 20-15-41](https://github.com/iecamachog/template-and-images/assets/132395694/4d777974-1f8d-4949-be7a-214afc356117)


Esta página contiene la lista de las fotos de trabajos realizados, en cada una lleva la opción de borrar la foto, los datos editables son: 
Título del servicio.
Descripción detallada.
Actividades que realiza.
Dirección del taller. 
Los campos que no son editables Categoría oficio, ya que esta opción no es modificable para evitar conflictos del trabajo que promueve el usuario trabajador.

## Descripción de las vistas correspondientes al grupo 06


###  Inicio de sesión

En la página de **inicio de sesión** tenemos un navbar sencillo, de color blanco en el extremo izquierdo se encuentra el logo de chambeaya, y en el otro extremo tenemos un link que nos lleva a la pestana de **Registro usuario**

El contenido principal de la página es una imagen de fondo con un recuadro situado del lado izquierdo en el cuál tenemos dos input uno solicita el *correo del usuario* y el otro solcita la *contraseña del usuario*.

Una vez que los dos campos se hayan llenado se da click al boton de que se encuentra debajo de los campos para poder acceder a la sesión.
En dado caso de no recordar tu contraseña correcta debajo del campo de contraseña hay un link que lleva a la pǵina de **Olvide contraseña**

Por último tenemos el footer el cual es de color azul verdoso que tiene algunos links para la página de **términos y condiciones**, **aviso de privacidad**, **accesibilidad** y **ayuda**.

<p align="center">
  <img src="https://github.com/gsibajai/VistaChambeaya/blob/main/Imagenes/inicioSesion.jpg" width="550px"/>
</p>

###  Olvidé contraseña
En la página de **Olvide mi contraseña** tenemos un navbar sencillo, el cual tiene solo dos elementos, en el extremo izquierdo esta el logo de chambeaya y en el extremo derecho tenemos un link que nos dirige a la página de **Iniciar sesión**

El contenido de la página es una imagen de fondo, y en el centro tenemos un recuadro que tiene por titulo *Olvide mi contraseña* un texto informativo:

*Para restablecer la contraseña se enviará un token a tu cuenta de correo al presionar el botón de continuar aparecerá una ventana con el opción para igresar el token, una vez se compruebe que el token es el correcto te redirigira al cambio de contraseña.*

y un campo en el cuál se solicita el correo del usuario que quiere reestablecer su contraseña.
En la esquina inferior derecha tenemos un boton para continuar.

<p align="center">
  <img src="https://github.com/gsibajai/VistaChambeaya/blob/main/Imagenes/forgotpass2.jpg" width="550px"/>
</p>

###  Token Olvidé contraseña
En la página de **Token Olvide mi contraseña** tenemos un navbar sencillo, el cual tiene solo dos elementos, en el extremo izquierdo esta el logo de chambeaya y en el extremo derecho tenemos un link que nos dirige a la página de **Iniciar sesión**

El contenido de la página es una imagen de fondo, y en el centro tenemos un recuadro que tiene por titulo *Token de validación* un texto informativo:

*Ya se ha enviado el token, ingresalo en el siguiente apartado y podrás cambiar tu contraseña,*

*Recuerda que el token es válido unicamente por 15 minutos*

y un campo en el cuál se solicita el token que se le envio al usuario por correo.
Para enviar el token es necesario que des click al boton de confirmar que se encuentra abajo.

<p align="center">
  <img src="https://github.com/gsibajai/VistaChambeaya/blob/main/Imagenes/token.png" width="550px"/>
</p>

###  Cambiar contraseña
En la página de **Cambiar mi contraseña** tenemos un navbar sencillo, el cual tiene solo dos elementos, en el extremo izquierdo esta el logo de chambeaya y en el extremo derecho tenemos un link que nos dirige a la página de **Iniciar sesión**

El contenido de la página es una imagen de fondo, y en el centro tenemos un recuadro que tiene por titulo *Cambiar Contraseña* 

y dos campos en donde se solicitala contraseña nueva del usuario.
Para cambiarla es necesario que des click al boton de confirmar que se encuentra abajo.

<p align="center">
  <img src="https://github.com/gsibajai/VistaChambeaya/blob/main/Imagenes/changePass.jpg" width="550px"/>
</p>

### Componente Quejas, sugerencia y comentarios

El componente se encuentra en la página **principal**
Como título pregunta lo siguiente:

*¿Tienes algún comentario queja o sugerencia?*

Como subtítulo tiene lo siguiente:

*Deja tu mensaje, tu opinión es muy importante pronto nos contactaremos contigo.*

Solicita dos campos
1. El correo electronico
2. El mensaje que quieres enviar

Por último en la esquina inferior derecha tienes un boton para enviar la información.


<p align="center">
  <img src="https://github.com/gsibajai/VistaChambeaya/blob/main/Imagenes/quejas.jpg" width="550px"/>
</p>

### Términos y condiciones

La página de **Términos y condiciones** es una página de texto plano, tiene un navbar sencillo que solo tiene el logo de chambeaya en el extremo izquierdo.
Tenemos el título de "Términos y condiciones" centrado en la página y debajo del titulo tenemos el escrito de los terminos y condiciones que tiene chambeaya.

En el inferior de la página tenemos un boton que nos regresa a la página principal.

<p align="center">
  <img src="https://github.com/gsibajai/VistaChambeaya/blob/main/Imagenes/terminosCondiciones.jpg" width="550px"/>
</p>

### Aviso de privacidad

La página de **Aviso de privacidad** es una página de texto plano, tiene un navbar sencillo que solo tiene el logo de chambeaya en el extremo izquierdo.
Tenemos el título de "Aviso de privacidad" centrado en la página y debajo del titulo tenemos el escrito de los terminos y condiciones que tiene chambeaya.

En el inferior de la página tenemos un boton que nos regresa a la página principal.

<p align="center">
  <img src="https://github.com/gsibajai/VistaChambeaya/blob/main/Imagenes/aviso.png" width="550px"/>
</p>

### Buscador
La página del buscador  tenemos un navbar más completo, que tiene tres elementos:
1. En el extremo izquierdo esta el logo de Chambeaya.
2. En el centro tenemos un buscador.
3. En el extremo derecho tenemos el perfil del ususario

Tenemos un componente que sirve como filtro en el lado izquierdo, el componente muestra dos formas de filtrar la información en este se puede filtrar por fecha y por categoría.

Fecha
- Ultimo mes
- Ultima semana
- Ultimos el día de hoy

Categoria
- Plomero
- Carpintero
- Electricista
- Pintor

En el centro tendremos un carrousel que mostrara cuatro cards que tendranla foto del ususario, su nombre y oficio, la puntuaciòn y una imagen de sus servicios.

<p align="center">
  <img src="https://github.com/ejreyesh/ejreyesh-prueba/blob/main/src/images/listado-oficios.png" width="550px"/>
</p>

### Componente y formulario  preguntas del anuncio
El componete de preguntas se encuentra en la página de los servicios donde las personas pueden resolver sus dudas publicando preguntas o viendo las preguntas que otros usuarios ya realizaron.
Este apartado solo es de vista, del lado izquierdo podemos ver la foto del usuario que pregunta y su pregunta
mientras que del otro lado podemos ver la foto del usuario que ofrece el servicio y la contestacion que dio.
Abajo de este apartado tenemos un boton que abre un modal en el cual nosotros podemos realizar una pregunta, pero para poder hacer esto es necesario que estes registrado, en dado caso de no estarlo te enviará a la página de iniciar sesión.


Si ya habias iniciado sesión se abrirá un modal en el que tendras un campo a llenar que es donde se cóloca la pregunta o la duda que tienes.

<p align="center">
  <img src="https://github.com/gsibajai/VistaChambeaya/blob/main/Imagenes/preguntas.jpg" width="550px"/>
</p>
