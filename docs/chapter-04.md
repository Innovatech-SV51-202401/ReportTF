# Capitulo IV: Product Design

## 4.1. Style Guidelines.
Especificamos los estilos generales de la aplicación web para el proceso de Front-End

### 4.1.1. General Style Guidelines.

Definimos los colores y el tipo de tipografías que se utilizarán de forma global en el proyecto. A Continuación mostramos una paleta de colores. 

![img.png](../assets/img/GSG-1.png)

![img.png](../assets/img/GSG-2.png)

#### Logo de GlideGo:
Nuestro logo representa un tono de verde limón opaco con el código hexadecimal ADE366, combina una bicicleta y una hoja de planta. La bicicleta simboliza movilidad, libertad y sostenibilidad, por otro lado la hoja representa la naturaleza y el compromiso con el medio ambiente. Esta combinación refleja nuestra visión de ofrecer soluciones de movilidad ecológica y sostenible. 

![img.png](../assets/img/Logo-1.png)

#### Horizontal Logo:

![img.png](../assets/img/logo-h-1.png)
![img.png](../assets/img/logo-h-2.png)

#### Typography:
Justificación porque usamos Open sans(googlear), pistas sencillo minimalista 

![img.png](../assets/img/typography.png)

- Colors
- Primarios
- Secundarios
- Terciarios

Pulcritud, elegancia y sofisticación, a su vez crea un contraste suave
 
![img.png](../assets/img/colors-1.png)
![img.png](../assets/img/colors-2.png)

### 4.1.2. Web Style Guidelines.
Nuestra web utiliza el Patrón Z, una estructura diseñada para guiar al usuario por la página de manera natural y efectiva. En la parte superior se encontrará la barra de navegación con un tono verde grisáceo, que brinda un aspecto serio y confiable. Esta barra contiene el logo y secciones como “Conocenos”, “Servicios”, “Planes” y “Obtener”. El boton de obtener es de color naranja que añade un toque de energia y atencion al diseño, contrasta con el resto de la página para invitar al usuario a descargar y probar la aplicación. 

Las tipografías que se aplicarán para el desarrollo de la web son:
Open Sans

## 4.2. information architecture.

### 4.2.1. Organization Systems.
Para el caso de organización visual utilizaremos el sistema jerárquico, lo que nos permitirá resaltar los componentes a los que deseamos que el usuario preste mayor atención. Esto dirigirá la atención del usuario a componentes de suma importancia como son: “About us”, “Services”, “Plans”, “Contact” y “Register”.

Para el proceso de reservas de vehículos haremos uso de la organización secuencial:
- Solicitud de reserva(clientes):
1. Búsqueda de vehículos
2. Elección del tipo de vehículo
3. Solicitud de reserva
4. Entrega del vehículo
5. Devolución del vehículo
- Solicitud de la inscripción de vehículos(owner):
1. Inscripción de vehículo a la plataforma
2. Establecer tarifa y disponibilidad del vehículo
3. Publicar disponibilidad del vehículo

Para los esquemas de organización utilizaremos los siguientes tipos:

- Organización por orden cronológico para el historial de reservas y las reseñas a los clientes
- Organización por segmentos(uso/tipo) para la sección de “Mis vehículos” del Owner.
- Organización por orden alfabético para la sección “Mis vehículos” del Owner y la sección “Mantenimiento” del mecánico.

### 4.2.2. Labeling Systems.
Para el uso de etiquetas de nuestro landing page, se ha elegido un lenguaje sencillo lo que permite a los usuarios familiarizarse con facilidad a las opciones proporcionadas. Esto logrará que los usuarios puedan navegar de manera intuitiva.

En el Landing Page:

| Etiqueta       | Descripcion                                                                              | 
|----------------|------------------------------------------------------------------------------------------|
| Inicio         | Apartado donde se muestra la información de la aplicación explicando sus características | 
| Sobre nosotros | Apartado donde se informa al usuario sobre el equipo y el propósito.                     |
| Servicios      | Apartado donde se muestra el tipo de usuario que puede ser y sus ventajas.               |
| Planes         | Apartado donde se muestran todos los planes de suscripción                               |
| Contactanos    | Apartado donde el usuario puede comunicarse con nosotros.                                |
| Iniciar Sesion | Apartado para ingresar a la cuenta de usuario.                                           |

Para la página es importante, un sistema de etiquetado efectivo para permitir que los usuarios encuentren fácilmente la información y los servicios que necesitan. Nuestro sistema de etiquetado considera cuidadosamente cómo presentar la información en el sitio web. Después de establecer la organización visual y los esquemas de categorización del contenido, se elegirá etiquetas claras y concisas que reflejan el lenguaje común y la comprensión del usuario con palabras comunes no pasan de tres palabras.  Nos aseguraremos de utilizar etiquetas intuitivas y fáciles de recordar para representar los diferentes conjuntos de información y asociaciones entre ellos. También se utilizarán diferentes colores y diseños para resaltar y diferenciar las etiquetas y conjuntos de información en mi sitio web.  Para evitar confusiones y asegurar la coherencia visual en todo el sitio web, se mantendrá un sistema de etiquetado consistente y se evitará el uso de términos técnicos o jerga que podría ser confuso para los usuarios. Usaremos un botón de “más información”. Dirige a los usuarios a visualizar más detalles de preguntas y respuestas a sus problemas mediante correo por la cual nos brindaras tu nombre, correo y número.  En el parte superior derecho del home page contando con cuatro botones
- Conócenos: Muestra quiénes somos, nuestro propósito y equipo.
- Servicios: Muestra lo que ofrecemos al usuario para mejorar financieramente.
- Planes: Muestra el plan que quiere adquirir lo cual le llevará a registrarse.
- Obtener: Muestra las opciones de descarga para Android y IOS. 

### 4.2.3. SEO Tags and Meta Tags

Title:

![img.png](../assets/img/SEO%20Tags.png)


### 4.2.4. Searching Systems.
En esta sección implementaremos dos métodos para facilitar la experiencia de búsqueda a nuestros usuarios.
Se utilizará un sistema de búsqueda por texto para que nuestros usuarios puedan buscar su vehículo y tener una elección más personalizada.

Además, se incluirá filtros de la siguiente manera:
- Filtros por tipo de vehículo
- Filtros por marca de vehiculo
- Filtros por color de vehículo
- Filtros por disponibilidad de ubicación

### 4.2.5. Navigation Systems.
Como sistema de navegación optamos emplear una barra de menú horizontal que guiará al usuario por las diferentes secciones con títulos claves y estáticos, esto facilitará al usuario a tener todas las herramientas a la mano y así disfrutar de una mejor navegación.
Nuestra barra de menú contará con las siguientes secciones:

- **About us:** El usuario podrá visualizar a qué se dedica la empresa, su misión y visión, y el equipo detrás de esta aplicación
- **Services:** El usuario podrá visualizar los servicios que estamos ofreciendo, si en caso quiera ser un Owner, un cliente o un mecanico.
- **Plans:** Aquí podrá obtener toda la información de los planes semanales, mensuales y trimestrales que la aplicación le ofrece y además de poder registrarse.
- **Contact us:** Donde los usuarios a través de un formulario podrán ponerse en contacto con nosotros .

## 4.3. Landing Page UI Design.
### 4.3.1. Landing Page Wireframe.
Link de figma: https://www.figma.com/file/zI2Ms3m44qqaav0cmkBFEp/INNOVATECH?type=design&node-id=0-1&mode=design&t=QeMym2oXpQQRRkGe-0 

![img.png](../assets/img/landing-1.png)
![img.png](../assets/img/landing-2.png)
![img.png](../assets/img/landing-3.png)
![img.png](../assets/img/landing-4.png)
![img.png](../assets/img/landing-5.png)

### 4.3.2 Landing Page Mock-up.
Link Figma: https://www.figma.com/file/zI2Ms3m44qqaav0cmkBFEp/INNOVATECH?type=design&node-id=75%3A2&mode=design&t=vmMKxEV2F816IZC1-1

![img.png](../assets/img/lading-6.png)
![img.png](../assets/img/landing-7.png)
![img.png](../assets/img/landing-8.png)
![img.png](../assets/img/landing-9.png)
![img.png](../assets/img/landing-10.png)
