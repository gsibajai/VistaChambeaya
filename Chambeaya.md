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

A esta vista podrá acceder cualquier usuario, la vista se conforma por un formulario en el cual se pondrá el correo, nick y contraseña ademas de contar con un captcha, ademas de contar con un botón de envio con el cual nos redirigira a la parte 2 de la página
<p align="center">
  <img src="https://raw.githubusercontent.com/gsibajai/VistaChambeaya/main/Imagenes/Registro1.png" width="550px"/>
</p>

### Registro2

A esta vista se accede despues de pedir el registro por lo que solo solicita el token de autenticación el cual será enviado por correo electronico, este apartado solo contará con un inpút en el cual se pondrá el token y un boton para enviarlo .

<p align="center">
  <img src="https://raw.githubusercontent.com/gsibajai/VistaChambeaya/main/Imagenes/Registro2.png" width="550px"/>
</p>

### Valoracion de Anuncio Vista


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
