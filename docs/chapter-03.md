# CAPÍTULO III: Requirements Specification

## 3.1. To-Be Scenario Mapping.
En esta sección se presenta el mapeo de los escenarios, realizando una tabla con la situación a mejorar del segmento objetivo, analizando que pasos se realizarán y cómo se siente.
### Segmento 1: Owner

<img src="../assets/to-be-escenario/to-be-owner.png" alt="To be Owner" >

### Segmento 2: User

<img src="../assets/to-be-escenario/to-be-user.png" alt="To be User" >

### Segmento 3: Mechanic

<img src="../assets/to-be-escenario/to-be-mecanico.png" alt="To be Mecanico" >

## 3.2. User Stories.

### User Stories

<table border="1">
    <tr>
        <th>Epic / Story ID</th>
        <th>Título</th>
        <th>Descripción</th>
        <th>Criterios de Aceptación</th>
        <th>Relacionado con (Epic ID)</th>
    </tr>
    <tr>
        <td>US01</td>
        <td>Registrar un Vehículos</td>
        <td><b>Cómo</b> Owner quiero registrar mis vehículos a la aplicación web <b>para</b> poder ofrecerlos a mis clientes potenciales</td>
        <td>
            <b>Scenario 1: Inscripción de vehículos a la aplicación Glidego</b> <br/>
            Given que el owner está en la opción "registration vehicle" de su cuenta. <br/>
            When registra un nuevo vehículo a la aplicación <br/>
            And Ingresa los detalles o caracteristicas del vehículo, como marca, modelo, tipo (bicicleta, scooter, moto eléctrica, etc.), disponibilidad, ubicación del vehículo <br/>
            Then La aplicación válida la información And finalmente confirma su registro satisfactorio. <br/><br/>
            <b>Scenario 2: Modificar datos del vehiculo registrado.</b> <br/>
            Given que el owner está en la sección de "vehicule" <br/>
            When verifica los datos del vehículo y fue registrado con errores<br/>
            Then La plataforma muestra una opción de "Editar" para corregir los datos del vehículo.
            <b>Scenario 3: Registro del vehiculo no válido.</b> <br/>
            Given que el owner está en la sección de "registration vehicle" de su cuenta. <br/>
            When registra un nuevo vehículo a la aplicación <br/>
            And Ingresa los detalles o caracteristicas del vehículo, como marca, modelo, tipo (bicicleta, scooter, moto eléctrica, etc.), disponibilidad, ubicación del vehículo <br/>
            Then La aplicación al validar los datos verifica que no son correctos And muestra un mensaje de "Error el registro" <br/>
        </td>
        <td>EP01</td>
    </tr>
    <tr>
        <td>US02</td>
        <td>Establecer Tarifas</td>
        <td>Cómo Owner quiero establecer tarifas para poder gestionar de manera efectiva la rentabilidad de mi vehículo</td>
        <td>
            <b>Escenario 1: Establecer tarifas según el tipo del vehículo.</b> <br/>
            Given que el Owner está en la sección de "Costos" <br/>
            When decide establecer las tarifas para el vehículo registrado<br/>
            And establece su costo por hora, día y por semana del alquiler del vehículo<br/>
            Then La plataforma procesa la información correctamente y el vehículo queda configurado con las tarifas y disponibilidad establecidas, permitiéndole gestionar de manera efectiva la rentabilidad y accesibilidad del vehículo para los usuarios. <br/><br/>
            <b>Escenario 2: Problema al establecer tarifas.</b> <br/>
            Given que el Owner está en la sección de "Costos" <br/>
            When intenta establecer las tarifas <br/>
            And Al ingresar las tarifas según los parametros que establece la aplicación y comete error <br/>
            Then La plataforma muestra un mensaje de error indicando la razón del problema en la configuración de tarifas.
        </td>
        <td>EP01</td>
    </tr>
    <tr>
        <td>US03</td>
        <td>Eficiencia al organizar los vehículos</td>
        <td>Cómo Owner quiero organizar para gestionar su renta.</td>
        <td>
            <b>Escenario 1: Gestión exitosa de vehículos para renta</b> <br/>
            Given que el Owner de vehículos menores. <br/>
            When Decide gestionar un vehículo para renta. <br/>
            And Accede al sistema de gestión de vehículos y selecciona el vehículo que desea gestionar. <br/>
            Then Puede establecer las tarifas de alquiler, la disponibilidad horaria, los días disponibles y cualquier restricción adicional que desee aplicar. <br/>
            And El vehículo queda configurado y listo para ser ofrecido a los usuarios para su alquiler, permitiéndome gestionar de manera efectiva la renta del vehículo. <br/><br/>
            <b>Escenario 2: Problema al gestionar un vehículo para renta</b> <br/>
            Given que el Owner de vehículos menores. <br/>
            When Intenta gestionar un vehículo para renta. <br/>
            And Al intentar configurar las tarifas, la disponibilidad o cualquier otro detalle, comete un error. <br/>
            Then Debe corregir los datos para poder completar la gestión del vehículo con éxito y ofrecerlo para su renta a los usuarios.
        </td>
        <td>EP01</td>
    </tr>
    <tr>
        <td>US04</td>
        <td>Visualización de Trámites</td>
        <td>Cómo Owner quiero acceder a los estados de trámites de mis vehículos para estar al tanto del progreso de los trámites relacionados.</td>
        <td>
            <b>Escenario 1: Acceso exitoso a los estados de trámites de los vehículos</b> <br/>
            Given que el Owner de vehículos menores. <br/>
            When Accede al sistema de gestión de trámites de vehículos. <br/>
            And Selecciona un vehículo específico para revisar su estado de trámite. <br/>
            Then Puede ver el progreso del trámite, como la renovación de seguros, la inspección técnica, la documentación legal, etc. <br/>
            And Esta al tanto de cualquier actualización o cambio en el estado del trámite, lo que me permite tomar decisiones informadas y planificar adecuadamente. <br/><br/>
            <b>Escenario 2: Problema al acceder a los estados de trámites de los vehículos</b> <br/>
            Given Soy que el Owner de vehículos menores. <br/>
            When Intenta acceder al sistema de gestión de trámites de vehículos. <br/>
            And Encuentra un problema técnico que impide la visualización de los estados de trámites. <br/>
            Then Debe contactar al soporte técnico para obtener asistencia y poder acceder nuevamente a los estados de trámites de sus vehículos.
        </td>
        <td>EP02</td>
    </tr>
    <tr>
        <td>US05</td>
        <td>Visualización del Recorrido</td>
        <td>Cómo Owner quiero visualizar el recorrido y tiempo de uso de los vehículos a través de la API de Google.</td>
        <td>
            <b>Escenario 1: Visualización exitosa del recorrido y tiempo de uso de los vehículos</b> <br/>
            Given que el Owner de vehículos menores. <br/>
            When Accede a la API de Google Maps desde el sistema de gestión de vehículos. <br/>
            And Selecciona un vehículo específico para visualizar su recorrido y tiempo de uso. <br/>
            Then Puede ver en tiempo real el recorrido que ha realizado el vehículo en el mapa, así como el tiempo total de uso durante un período específico. <br/>
            And Tiene acceso a información detallada como la distancia recorrida, las paradas realizadas y la duración de cada trayecto, lo que le permite analizar el uso del vehículo y tomar decisiones informadas. <br/><br/>
            <b>Escenario 2: Problema al visualizar el recorrido y tiempo de uso de los vehículos</b> <br/>
            Given que el Owner de vehículos menores. <br/>
            When Intenta acceder a la API de Google Maps desde el sistema de gestión de vehículos. <br/>
            And Encuentra un problema técnico que impide la visualización del recorrido y tiempo de uso. <br/>
            Then Debe contactar al soporte técnico para obtener asistencia y poder acceder nuevamente a la información del recorrido y tiempo de uso de mis vehículos.
        </td>
        <td>EP02</td>
    </tr>
    <tr>
        <td>US06</td>
        <td>Historial de reserva</td>
        <td>Cómo Owner quiero acceder al historial de mis vehículos reservados para monitorear su uso.</td>
        <td>
            <b>Escenario 1: Acceso exitoso al historial de vehículos reservados</b> <br/>
            Given que el Owner de vehículos menores. <br/>
            When Accede al sistema de gestión de reservas desde la plataforma. <br/>
            And Selecciona un vehículo específico para revisar su historial de reservas. <br/>
            Then Puede ver el historial completo de todas las reservas realizadas para ese vehículo, incluyendo fechas, duración de la reserva, nombre del cliente, tarifas aplicadas, estado de la reserva, etc. <br/>
            And Tiene acceso a información detallada sobre cómo se ha utilizado el vehículo a lo largo del tiempo, lo que le permite monitorear su uso de manera efectiva. <br/><br/>
            <b>Escenario 2: Problema al acceder al historial de vehículos reservados</b> <br/>
            Given que el Owner de vehículos menores. <br/>
            When Intenta acceder al sistema de gestión de reservas desde la plataforma. <br/>
            And Encuentra un problema técnico que impide la visualización del historial de reservas. <br/>
            Then Debe contactar al soporte técnico de la plataforma para obtener asistencia y poder acceder nuevamente al historial de reservas de sus vehículos.
        </td>
        <td>EP02</td>
    </tr>
    <tr>
        <td>US07</td>
        <td>Historial de mantenimiento</td>
        <td>Cómo Owner quiero acceder al historial de mantenimiento y/o reparación realizados a mis vehículos para conocer las condiciones de mis vehículos.</td>
        <td>
            <b>Escenario 1: Acceso exitoso al historial de mantenimiento y reparación</b> <br/>
            Given que el Owner de vehículos menores. <br/>
            When Accede al sistema de gestión de mantenimiento y reparaciones desde la plataforma. <br/>
            And Selecciona un vehículo específico para revisar su historial de mantenimiento y reparaciones. <br/>
            Then Puede ver el historial completo de todas las actividades de mantenimiento y reparaciones realizadas en el vehículo, incluyendo fechas, tipo de servicio, piezas reemplazadas, costos asociados, notas del mecánico, etc. <br/>
            And Tiene acceso a información detallada sobre el estado y las condiciones de sus vehículos. <br/><br/>
            <b>Escenario 2: No hay historial de mantenimiento y reparación</b> <br/>
            Given que el Owner de vehículos menores. <br/>
            When Intenta acceder al sistema de gestión de mantenimiento y reparaciones desde la plataforma. <br/>
            Then Visualiza que su vehículo no tiene historial de mantenimiento.
        </td>
        <td>EP02</td>
    </tr>
    <tr>
        <td>US08</td>
        <td>Visualización del perfil de cliente</td>
        <td>Cómo Owner quiero visualizar el perfil del cliente que hace uso de mi vehículo para conocer a mi cliente.</td>
        <td>
            <b>Escenario 1: Visualización exitosa del perfil del cliente</b> <br/>
            Given que el Owner de vehículos menores. <br/>
            When Accede al sistema de gestión de clientes desde la plataforma. <br/>
            And Selecciona el perfil de un cliente que ha hecho uso de su vehículo. <br/>
            Then Puede ver información detallada del cliente, como nombre, contacto, fotografía y comentarios. <br/><br/>
            <b>Escenario 2: Error al visualizar el perfil del cliente</b> <br/>
            Given que el Owner de vehículos menores. <br/>
            When Intenta acceder al sistema de gestión de clientes desde la plataforma. <br/>
            And Encuentra un problema técnico que impide la visualización del perfil del cliente. <br/>
            Then Debe contactar al soporte técnico de la plataforma.
        </td>
        <td>EP03</td>
    </tr>
    <tr>
        <td>US09</td>
        <td>Retiro de ingresos</td>
        <td>Cómo Owner quiero retirar los ingresos generados por los vehículos para ampliar mi flota.</td>
        <td>
            <b>Escenario 1: Retiro exitoso de ingresos generados por los vehículos</b> <br/>
            Given que el Owner de vehículos menores. <br/>
            When Accede al sistema de gestión financiera desde la plataforma. <br/>
            And Selecciona la opción de retirar ingresos generados por los vehículos. <br/>
            Then Puede ver el monto total de ingresos disponibles para retirar. <br/>
            And Procede a retirar los ingresos y el sistema confirma la transacción exitosa. <br/><br/>
            <b>Escenario 2: Problema al retirar los ingresos generados por los vehículos</b> <br/>
            Given que el Owner de vehículos menores. <br/>
            When Intenta retirar los ingresos generados por los vehículos desde la plataforma. <br/>
            And Utiliza un método de depósito incorrecto. <br/>
            Then el sistema le arroja un aviso de fallo en el pago.
        </td>
        <td>EP03</td>
    </tr>
    <tr>
        <td>US10</td>
        <td>Visualización de catálogo de vehículos</td>
        <td>Como cliente quiero visualizar el catálogo de vehículos disponibles según tipo y disponibilidad para seleccionar el mejor ajuste a mis necesidades.</td>
        <td>
            <b>Escenario 1: Visualización exitosa del catálogo de vehículos disponibles</b> <br/>
            Given que el cliente de la aplicación de alquiler de vehículos menores. <br/>
            When Accede al catálogo de vehículos desde la aplicación. <br/>
            And Selecciona el tipo de vehículo que deseo ver, como bicicletas, scooters, motos eléctricas, etc. <br/>
            Then Se muestra una lista de vehículos disponibles del tipo seleccionado, con información detallada como modelo, características, tarifas por hora o día, ubicación y disponibilidad. <br/>
            And Puede navegar por el catálogo, comparar opciones y seleccionar el vehículo que mejor se ajuste a sus necesidades. <br/><br/>
            <b>Escenario 2: Problema al visualizar el catálogo de vehículos disponibles</b> <br/>
            Given que el cliente de la aplicación de alquiler de vehículos menores. <br/>
            When Intenta acceder al catálogo de vehículos desde la aplicación. <br/>
            And Encuentra un problema técnico que impide cargar o mostrar el catálogo. <br/>
            Then Debe contactar con el soporte técnico de la plataforma.
        </td>
        <td>EP04</td>
    </tr>
    <tr>
        <td>US11</td>
        <td>Reserva de vehículo</td>
        <td>Como cliente quiero reservar un vehículo para desplazarme por la ciudad.</td>
        <td>
            <b>Escenario 1: Reserva exitosa de un vehículo</b> <br/>
            Given que el cliente de la aplicación de alquiler de vehículos menores. <br/>
            When Accede al catálogo de vehículos disponibles desde la aplicación. <br/>
            And Selecciona el vehículo que deseo reservar, considerando la disponibilidad, ubicación y tipo de vehículo que necesita. <br/>
            And Elije la fecha y hora de inicio de su reserva, así como la duración del alquiler. <br/>
            Then Confirma la reserva y la aplicación procesa la solicitud con éxito. <br/><br/>
            <b>Escenario 2: Error de pago al reservar un vehículo</b> <br/>
            Given que el cliente de la aplicación de alquiler de vehículos menores. <br/>
            When Intenta reservar un vehículo desde la aplicación. <br/>
            And Encuentra que su información de pago no cuenta con fondos. <br/>
            Then debe utilizar otro método de pago.
        </td>
        <td>EP04</td>
    </tr>
    <tr>
        <td>US12</td>
        <td>Gestión del servicio</td>
        <td>Como cliente quiero gestionar el servicio para poder finalizarlo cuando lo requiera.</td>
        <td>
            <b>Escenario 1: Gestión exitosa del servicio</b> <br/>
            Given que el cliente de la aplicación de alquiler de vehículos menores. <br/>
            When Accede a su cuenta en la aplicación. <br/>
            And Selecciona el servicio que desea gestionar, como la reserva de un vehículo. <br/>
            And Encuentra la opción de finalizar el servicio dentro de la aplicación. <br/>
            Then Confirma la finalización del servicio y la aplicación procesa la solicitud con éxito. <br/><br/>
            <b>Escenario 2: Problema al gestionar el servicio</b> <br/>
            Given Soy que el cliente de la aplicación de alquiler de vehículos menores. <br/>
            When Intenta gestionar un servicio desde la aplicación. <br/>
            And Encuentra un error falta de conectividad. <br/>
            Then Debe intentar nuevamente la gestión del servicio después de verificar su conexión a internet.
        </td>
        <td>EP04</td>
    </tr>
    <tr>
        <td>US13</td>
        <td>Visualizar tiempo y distancia de recorrido</td>
        <td>Como cliente quiero visualizar en tiempo real la distancia y tiempo recorrido para gestionar mejor mi uso del servicio.</td>
        <td>
            <b>Escenario 1: Visualización en tiempo real de la distancia y tiempo recorrido</b> <br/>
            Given que el cliente de la aplicación de alquiler de vehículos menores. <br/>
            When Accede al servicio de alquiler de vehículos y comienza su viaje. <br/>
            And Utiliza la función de seguimiento en tiempo real dentro de la aplicación. <br/>
            Then Puede ver la distancia recorrida y el tiempo transcurrido en tiempo real mientras usa el vehículo. <br/><br/>
            <b>Escenario 2: Error visualización de la distancia y tiempo recorrido en tiempo real</b> <br/>
            Given Soy que el cliente de la aplicación de alquiler de vehículos menores. <br/>
            When Intenta utilizar la función de seguimiento en tiempo real dentro de la aplicación. <br/>
            And Encuentra un problema técnico que impide la visualización de la distancia y tiempo recorrido en tiempo real. <br/>
            Then Debe contactar al servicio técnico de la plataforma.
        </td>
        <td>EP05</td>
    </tr>
    <tr>
        <td>US14</td>
        <td>Visualizar restricciones</td>
        <td>Como cliente quiero visualizar los límites de uso de mi vehículo reservado a través de la API de Google Maps para asegurarme de cumplir con las restricciones.</td>
        <td>
            <b>Escenario 1: Visualización exitosa de los límites de uso del vehículo</b> <br/>
            Given que el cliente es usuario de la aplicación <br/>
            When Accede a su reserva de vehículo desde la aplicación. <br/>
            And utiliza la API de Google Maps integrada en la aplicación. <br/>
            And La API muestra los límites de uso del vehículo, como zonas restringidas o áreas permitidas. <br/>
            Then puede asegurarse de cumplir con las restricciones y usar el vehículo de manera adecuada dentro de los límites establecidos. <br/><br/>
            <b>Escenario 2: Problema al visualizar los límites de uso del vehículo</b> <br/>
            Given de que el cliente de la aplicación de alquiler de vehículos menores. <br/>
            When intenta visualizar los límites de uso del vehículo a través de la API de Google Maps. <br/>
            And encuentra un problema técnico que impide la visualización de los límites de uso. <br/>
            Then debe cerrar y volver a abrir la aplicación para intentar nuevamente.
        </td>
        <td>EP05</td>
    </tr>
    <tr>
        <td>US15</td>
        <td>Alerta de vías</td>
        <td>Como cliente quiero recibir alertas del estado de vía a través de la API de Google Maps para conocer las condiciones de las vías.</td>
        <td>
            <b>Escenario 1: Recepción exitosa de alertas del estado de vía</b> <br/>
            Given que el cliente de la aplicación de alquiler de vehículos menores. <br/>
            When Accede a la API de Google Maps integrada en la aplicación. <br/>
            And Activa la función de alertas del estado de vía. <br/>
            And La API le envía alertas en tiempo real sobre condiciones de tráfico, accidentes u otros eventos que puedan afectar su viaje. <br/><br/>
            <b>Escenario 2: Consultar el estado de vías en una ruta planificada</b> <br/>
            Given que el cliente ha ingresado las coordenadas geográficas específicas de inicio y destino <br/>
            When consulte con el mapa integrado de la aplicación para obtener la ruta más óptima <br/>
            Then recibe la información detallada del estado de las vías a lo largo de la ruta planificada.
        </td>
        <td>EP05</td>
    </tr>
    <tr>
        <td>US16</td>
        <td>Inscripción de taller</td>
        <td>Cómo mecánico quiero inscribir mi taller a la aplicación, para ofrecer mis servicios.</td>
        <td>
            <b>Escenario 1: Inscripción exitosa del taller a la aplicación</b> <br/>
            Given que el mecánico quiere ofrecer sus servicios a través de la aplicación <br/>
            When accede al sistema de registro de talleres <br/>
            And completa el formulario de inscripción con los datos del taller, como nombre, dirección, servicios que ofrece, horarios de atención e información de contacto. <br/>
            Then La aplicación procesa la solicitud de inscripción con éxito y el taller queda registrado en la plataforma. <br/><br/>
            <b>Escenario 2: Problema al inscribir el taller a la aplicación</b> <br/>
            Given que el mecánico quiere ofrecer sus servicios a través de la aplicación. <br/>
            When intenta inscribir su taller en la aplicación. <br/>
            And se da cuenta que la dirección ingresada a su taller no se encuentra en la base de datos de la aplicación. <br/>
            Then debe verificar la dirección ingresada y asegurarse de que esté correctamente escrita. <br/>
            And si la dirección es correcta, pero aún no se encuentra en la base de datos, debe contactar al equipo de soporte de la aplicación para solicitar la adición de la misma.
        </td>
        <td>EP06</td>
    </tr>
    <tr>
        <td>US17</td>
        <td>Colocación de tarifas</td>
        <td>Cómo mecánico quiero establecer tarifas según el tipo de servicio y disponibilidad para brindar una estructura de precios clara.</td>
        <td>
            <b>Escenario 1: Establecimiento exitoso de tarifas según el tipo de servicio y disponibilidad</b> <br/>
            Given que el mecánico está registrado en la aplicación. <br/>
            When accede a la gestión de tarifas de la plataforma. <br/>
            And selecciona el tipo de servicio al que quiere establecer su tarifa, como mantenimiento o reparación. <br/>
            And define las tarifas para cada tipo de servicio, considerando la complejidad, el tiempo requerido, y otros factores relevantes. <br/>
            Then quedan registradas en la aplicación y son mostradas al cliente. <br/><br/>
            <b>Escenario 2: Rechazo de exceso de tarifas.</b> <br/>
            Given que el mecánico está registrado en la aplicación. <br/>
            When intenta establecer sus tarifas según el tipo de servicio y disponibilidad desde la plataforma. <br/>
            And su solicitud es rechazada por exceder su tarifa al promedio establecido en la aplicación. <br/>
            Then debe intentar nuevamente ingresar la solicitud con una nueva tarifa. <br/>
            And Si el problema persiste, debe contactar al soporte técnico de la aplicación para obtener asistencia y resolver el problema.
        </td>
        <td>EP06</td>
    </tr>
    <tr>
        <td>US18</td>
        <td>Visualizar solicitudes de servicio</td>
        <td>Cómo mecánico quiero acceder a las solicitudes de servicio para poder revisar los detalles.</td>
        <td>
            <b>Escenario 1: Acceso a las solicitudes de servicio</b> <br/>
            Given de que el mecánico está registrado en la plataforma. <br/>
            When accede al sistema de gestión de solicitudes desde la plataforma. <br/>
            Then puede revisar los detalles de cada solicitud, incluyendo la información del cliente, descripción del problema del vehículo, fecha de solicitud y tipo de servicio solicitado. <br/>
            And esto le permite prepararse para realizar las tareas requeridas de la solicitud recibida. <br/><br/>
            <b>Escenario 2: Problema al acceder a las solicitudes de servicio</b> <br/>
            Given que el mecánico está registrado en la plataforma. <br/>
            When intenta acceder al sistema de gestión de solicitudes desde la plataforma. <br/>
            And encuentra un problema técnico que impide la visualización de las solicitudes. <br/>
            Then verifica su conexión a internet y refresca la página, pero el problema persiste. <br/>
            And contacta al soporte técnico de la aplicación para resolver la dificultad técnica.
        </td>
        <td>EP06</td>
    </tr>
    <tr>
        <td>US19</td>
        <td>Envio de informe del mantenimiento</td>
        <td>Cómo mecánico quiero realizar y enviar un informe del servicio brindado para documentar los trabajos realizados.</td>
        <td>
            <b>Escenario 1: Realización y envío del informe</b> <br/>
            Given de que el mecánico que ha completado un servicio. <br/>
            When Accede al sistema de gestión de informes desde la plataforma. <br/>
            And Creo un informe detallado del servicio realizado. <br/>
            Then Envío el informe al cliente a través de la plataforma de comunicación. <br/><br/>
            <b>Escenario 2: Problema al realizar y enviar el informe</b> <br/>
            Given que el mecánico completa un servicio. <br/>
            When crea y envia un informe del servicio desde la plataforma. <br/>
            And encuentra un problema técnico que impide la creación o envío del informe. <br/>
            Then contacta al soporte técnico para resolver la dificultad técnica.
        </td>
        <td>EP06</td>
    </tr>
    <tr>
        <td>US20</td>
        <td>Notificación de finalización del servicio</td>
        <td>Cómo mecánico quiero finalizar y notificar la culminación del servicio para informar al cliente que su vehículo está listo.</td>
        <td>
            <b>Escenario 1: Finalización y notificación del servicio</b> <br/>
            Given que el mecánico completa un servicio. <br/>
            When finaliza el servicio y lo ingresa al sistema. <br/>
            Then el sistema envía una notificación al cliente informando que su vehículo está listo. <br/><br/>
            <b>Escenario 2: Problema al finalizar y notificar el servicio</b> <br/>
            Given el mecánico finaliza un servicio y solicita la notificación al cliente <br/>
            When finaliza el servicio pero encuentra un problema técnico. <br/>
            Then Contacta al soporte técnico para resolver la dificultad. <br/>
            And Una vez solucionado, notifica al cliente sobre la culminación del servicio.
        </td>
        <td>EP06</td>
    </tr>
    <tr>
        <td>US21</td>
        <td>Registro de ingresos</td>
        <td>Cómo mecánico quiero observar los ingresos generados por el servicio para llevar un registro preciso de los pagos recibidos.</td>
        <td>
            <b>Escenario 1: Gestión de ingresos generados por el servicio</b> <br/>
            Given que el mecánico completa un servicio. <br/>
            When accede a su billetera virtual desde la plataforma. <br/>
            And registra el pago recibido por el servicio realizado. <br/>
            Then El sistema actualiza automáticamente el registro de ingresos para llevar un registro preciso de los pagos recibidos. <br/><br/>
            <b>Escenario 2: Problema al gestionar los ingresos generados</b> <br/>
            Given que el mecánico que ha completado un servicio. <br/>
            When registra el pago pero encuentra un problema técnico. <br/>
            Then Contacta al soporte técnico para resolver la dificultad. <br/>
            And Una vez solucionado, registra el pago para mantener un registro preciso de los ingresos generados.
        </td>
        <td>EP06</td>
    </tr>
    <tr>
        <td>US22</td>
        <td>Historial de mantenimiento</td>
        <td>Cómo mecánico quiero acceder al historial de mantenimiento realizado a los vehículos para tener un registro de las reparaciones anteriores.</td>
        <td>
            <b>Escenario 1: Acceso al historial de mantenimiento de vehículos</b> <br/>
            Given que el mecánico está registrado en la plataforma. <br/>
            When accede al sistema de historial de mantenimiento desde la plataforma. <br/>
            And busca el vehículo específico del cual quiere revisar el historial de mantenimiento. <br/>
            Then puede ver un registro detallado de todas las reparaciones y mantenimientos previos realizados a ese vehículo, incluyendo fechas, trabajos realizados, piezas reemplazadas y notas adicionales. <br/><br/>
            <b>Escenario 2: Problema al acceder al historial de mantenimiento</b> <br/>
            Given que el mecánico está registrado en la plataforma. <br/>
            When accede al historial de mantenimiento de un vehículo. <br/>
            And encuentra un problema técnico que impide la visualización del historial. <br/>
            Then contacta al soporte técnico para resolver la dificultad.
        </td>
        <td>EP06</td>
    </tr>
    <tr>
        <td>US23</td>
        <td>Comunicación con soporte</td>
        <td>Cómo Owner quiero comunicarme con alguien de soporte a través del apartado de soporte para solicitar ayuda o presentar algún reclamo.</td>
        <td>
            <b>Escenario 1: Comunicación con el soporte a través del apartado de soporte</b> <br/>
            Given que el Owner está registrado en la plataforma. <br/>
            When accede al apartado de soporte. <br/>
            And envía su solicitud de ayuda o reclamo detallando su problema. <br/>
            Then el equipo de soporte recibe su solicitud y se comunica con el usuario para brindarle asistencia o resolver su reclamo. <br/><br/>
            <b>Escenario 2: Problema al comunicarme con el soporte</b> <br/>
            Given que el Owner está registrado en la plataforma. <br/>
            When se comunica con el soporte pero encuentra un problema técnico. <br/>
            Then verifica la conexión a internet y refresca la página. <br/>
            And si persiste, busca información de contacto alternativa para comunicarse. <br/>
            And Una vez establecida la comunicación, presenta su solicitud al equipo de soporte.
        </td>
        <td>EP07</td>
    </tr>
    <tr>
        <td>US24</td>
        <td>Historial de reservas</td>
        <td>Como cliente quiero ver historial de reservas para llevar un seguimiento de uso.</td>
        <td>
            <b>Escenario 1: Visualización del historial de reservas</b> <br/>
            Given que el cliente está registrado. <br/>
            When accede a su cuenta en la aplicación. <br/>
            Then ve una lista de reservas anteriores con detalles como fecha, vehículo y duración. <br/><br/>
            <b>Escenario 2: Problema al ver historial de reservas</b> <br/>
            Given que el cliente está registrado. <br/>
            When observa el historial de reservas pero hay un problema técnico. <br/>
            Then refresca la página y vuelve a intentar. <br/>
            And si persiste, contacta al soporte técnico para solucionarlo.
        </td>
        <td>EP07</td>
    </tr>
    <tr>
        <td>US25</td>
        <td>Comunicación con soporte</td>
        <td>Como cliente quiero comunicarme con alguien de soporte a través del apartado de soporte para solicitar ayuda o presentar algún reclamo.</td>
        <td>
            <b>Escenario 1: Comunicación con el soporte a través del apartado de soporte</b> <br/>
            Given que el cliente está registrado en la plataforma. <br/>
            When accede al apartado de soporte desde la plataforma. <br/>
            And envía su solicitud de ayuda o reclamo detallando su problema. <br/>
            Then el equipo de soporte recibe su solicitud y se comunica con el cliente para brindarle la ayuda necesaria o resolver su reclamo. <br/><br/>
            <b>Escenario 2: Problema al comunicarme con el soporte</b> <br/>
            Given que el cliente está registrado en la plataforma. <br/>
            When intenta comunicarse con el soporte pero encuentra un problema técnico. <br/>
            Then verifica su conexión a internet y refresca la página. <br/>
            And si el problema persiste, busca información de contacto alternativa para comunicarse.
        </td>
        <td>EP07</td>
    </tr>
    <tr>
        <td>US26</td>
        <td>Comunicación con soporte</td>
        <td>Como mecánico quiero comunicarme con alguien de soporte a través del apartado de soporte para solicitar ayuda o presentar algún reclamo.</td>
        <td>
            <b>Escenario 1: Comunicación con el soporte a través del apartado de soporte</b> <br/>
            Given que el mecánico está registrado en la plataforma. <br/>
            When accede al apartado de soporte desde la plataforma. <br/>
            And envía su solicitud de ayuda o reclamo detallando su problema. <br/>
            Then el equipo de soporte recibe su solicitud y se comunica con el cliente para brindar la asistencia necesaria o resolver su reclamo. <br/><br/>
            <b>Escenario 2: Problema al comunicarme con el soporte</b> <br/>
            Given que el mecánico está registrado en la plataforma. <br/>
            When intenta comunicarse con el soporte pero encuentra un problema técnico. <br/>
            Then verifica su conexión a internet y refresca la página. <br/>
            And Si persiste, busca información de contacto alternativa para comunicarse.
        </td>
        <td>EP07</td>
    </tr>
    <tr>
        <td>US27</td>
        <td>Visualización de planes</td>
        <td>Como cliente quiero ver los planes del servicio para elegir uno adecuado.</td>
        <td>
            <b>Escenario 1: Nuevo usuario interesado en el servicio.</b> <br/>
            Given que el cliente está interesado en el servicio. <br/>
            When ingresa al apartado de planes desde la web estática. <br/>
            Then el cliente podrá observar los planes disponibles. <br/><br/>
            <b>Escenario 2: Elección de plan</b> <br/>
            Given que el cliente conoce los planes. <br/>
            When el cliente selecciona uno de los planes. <br/>
            Then el cliente podrá registrarse en la plataforma con el plan seleccionado.
        </td>
        <td>EP07</td>
    </tr>
    <tr>
        <td>US28</td>
        <td>Servicios</td>
        <td>Como cliente quiero saber los beneficios del servicio para elegir un plan de suscripción.</td>
        <td>
            <b>Escenario 1: Beneficios del cliente</b> <br/>
            Given que el cliente quiere ver el servicio que se ofrece. <br/>
            When accede al apartado de servicios desde la plataforma. <br/>
            Then el cliente observa los servicios que ofrece. <br/><br/>
            <b>Escenario 2: Vehículos disponibles</b> <br/>
            Given que el cliente quiere ver qué vehículos menores se pueden utilizar. <br/>
            When accede al apartado de servicios desde la plataforma. <br/>
            Then el cliente tendrá información sobre los vehículos que están disponibles en la suscripción.
        </td>
        <td>EP07</td>
    </tr>
    <tr>
        <td>US29</td>
        <td>Conocer al equipo</td>
        <td>Como cliente quiero informarme sobre el equipo a cargo del proyecto para conocer sus objetivos.</td>
        <td>
            <b>Escenario 1: Presentación del equipo al cliente</b> <br/>
            Given que el cliente desea saber quiénes son los que realizan el servicio. <br/>
            When ingresa al apartado de sobre nosotros. <br/>
            Then ve el nombre del grupo que realiza el servicio. <br/><br/>
            <b>Escenario 2: Interés del objetivo del equipo</b> <br/>
            Given que el cliente se interesa por el objetivo del servicio. <br/>
            When ingresa al apartado de sobre nosotros. <br/>
            Then observa el objetivo que tiene el equipo.
        </td>
        <td>EP07</td>
    </tr>
    <tr>
        <td>US30</td>
        <td>Información del producto</td>
        <td>Como cliente quiero ver información general sobre el servicio.</td>
        <td>
            <b>Escenario 1: Conocer el producto</b> <br/>
            Given que el cliente quiere conocer el producto. <br/>
            When ingresa al enlace de la web estática. <br/>
            Then ve la información general sobre el servicio. <br/><br/>
            <b>Escenario 2: Obtener mayor información</b> <br/>
            Given que el cliente desea tener mayor información del servicio. <br/>
            When accede a uno de los apartados de la web estática. <br/>
            Then revisa la información que desea ver.
        </td>
        <td>EP07</td>
    </tr>
    <tr>
        <td>US31</td>
        <td>Ingreso de cuenta</td>
        <td>Como cliente quiero ingresar a una cuenta para ver mi suscripción, mi información y la disponibilidad de vehículos.</td>
        <td>
            <b>Escenario 1: Registrar cuenta</b> <br/>
            Given que el cliente quiere suscribirse a un plan. <br/>
            When accede al apartado de empezar desde la web estática. <br/>
            Then se registra con los datos requeridos para registrar su cuenta. <br/><br/>
            <b>Escenario 2: Ingreso a la cuenta</b> <br/>
            Given que el cliente quiere ingresar a su cuenta. <br/>
            When accede al apartado de empezar desde la web estática. <br/>
            Then coloca los datos solicitados para ingresar a su cuenta.
        </td>
        <td>EP07</td>
    </tr>
</table>



## 3.3. Impact Mapping.

En esta sección se muestra un gráfico que incluye los business goals del negocio así como tiene un impacto en nuestras user personas.
### Segmento 1:

<img src="/assets/impact-mapping/Owner.png" alt="IM Owner" >

### Segmento 2:

<img src="/assets/impact-mapping/Client.png" alt="IM Client" >

### Segmento 3:

<img src="/assets/impact-mapping/Mecanico.png" alt="IM Mecanico" >


## 3.4. Product Backlog.

<table border="1">
  <thead>
    <tr>
      <th>#Orden</th>
      <th>User Story Id</th>
      <th>Título</th>
      <th>Descripción</th>
      <th>StoryPoints (1/2/3/5/8)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>US01</td>
      <td>Inscripcion de vehiculos</td>
      <td>Cómo Owner quiero inscribir los vehículos a la aplicación para poder ofrecerlos a potenciales usuarios</td>
      <td>8</td>
    </tr>
    <tr>
      <td>2</td>
      <td>US02</td>
      <td>Establecimiento de Tarifas</td>
      <td>Cómo Owner quiero establecer tarifas y disponibilidad del vehículo para poder gestionar de manera efectiva la rentabilidad y accesibilidad de los vehículos.</td>
      <td>5</td>
    </tr>
    <tr>
      <td>3</td>
      <td>US03</td>
      <td>Gestionamiento de vehiculos</td>
      <td>Cómo Owner quiero gestionar mis vehículos para gestionar su renta</td>
      <td>5</td>
    </tr>
    <tr>
      <td>4</td>
      <td>US04</td>
      <td>Visualización de tramites</td>
      <td>Cómo Owner quiero acceder a los estados de trámites de mis vehículos para estar al tanto del progreso de los trámites relacionados</td>
      <td>3</td>
    </tr>
    <tr>
      <td>5</td>
      <td>US05</td>
      <td>Visualización del recorrido</td>
      <td>Cómo Owner quiero visualizar el recorrido y tiempo de uso de los vehículos a través de la API de google</td>
      <td>5</td>
    </tr>
    <tr>
      <td>6</td>
      <td>US06</td>
      <td>Historial de reserva</td>
      <td>Cómo Owner quiero acceder al historial de mis vehículos reservados para monitorear su uso</td>
      <td>3</td>
    </tr>
    <tr>
      <td>7</td>
      <td>US07</td>
      <td>Historial de mantenimiento</td>
      <td>Cómo Owner quiero acceder al historial de mantenimiento y/o reparación realizados a mis vehículos para conocer las condiciones de mis vehículos</td>
      <td>3</td>
    </tr>
    <tr>
      <td>8</td>
      <td>US08</td>
      <td>Visualización del perfil de cliente</td>
      <td>Cómo Owner quiero visualizar el perfil del cliente que hace uso de mi vehículo para conocer a mi cliente</td>
      <td>5</td>
    </tr>
    <tr>
      <td>9</td>
      <td>US09</td>
      <td>Retiro de ingresos</td>
      <td>Cómo Owner quiero retirar los ingresos generados por los vehículos para ampliar mi flota</td>
      <td>5</td>
    </tr>
    <tr>
      <td>10</td>
      <td>US10</td>
      <td>Visualización de catalogo de vehiculos</td>
      <td>Como cliente quiero visualizar el catálogo de vehículos disponibles según tipo y disponibilidad para seleccionar el mejor ajuste a mis necesidades</td>
      <td>3</td>
    </tr>
    <tr>
      <td>11</td>
      <td>US11</td>
      <td>Reserva de vehiculo</td>
      <td>Como cliente quiero reservar un vehículo para desplazarme por la ciudad.</td>
      <td>8</td>
    </tr>
    <tr>
      <td>12</td>
      <td>US12</td>
      <td>Gestion del servicio</td>
      <td>Como cliente quiero gestionar el servicio para poder finalizarlo cuando lo requiera</td>
      <td>8</td>
    </tr>
    <tr>
      <td>13</td>
      <td>US13</td>
      <td>Visualizar tiempo y distancia de recorrido</td>
      <td>Como cliente quiero visualizar en tiempo real la distancia y tiempo recorrido para gestionar mejor mi uso del servicio</td>
      <td>5</td>
    </tr>
    <tr>
      <td>14</td>
      <td>US14</td>
      <td>Visualizar restricciones</td>
      <td>Como cliente quiero visualizar los límites de uso de mi vehículo reservado a través de la API de google maps para asegurarme de cumplir con las restricciones</td>
      <td>5</td>
    </tr>
    <tr>
      <td>15</td>
      <td>US15</td>
      <td>Alerta de vias</td>
      <td>Como cliente quiero recibir alertas del estado de vía a través de la API de google maps para conocer las condiciones de las vías</td>
      <td>5</td>
    </tr>
    <tr>
      <td>16</td>
      <td>US16</td>
      <td>Inscripcion de taller</td>
      <td>Cómo mecánico quiero inscribir mi taller a la aplicación, para ofrecer mis servicios</td>
      <td>8</td>
    </tr>
    <tr>
      <td>17</td>
      <td>US17</td>
      <td>Colocación de tarifas</td>
      <td>Cómo mecánico quiero establecer tarifas según el tipo de servicio y disponibilidad para brindar una estructura de precios clara</td>
      <td>5</td>
    </tr>
    <tr>
      <td>18</td>
      <td>US18</td>
      <td>Visualizar solicitudes de servicio</td>
      <td>Cómo mecánico quiero acceder a las solicitudes de servicio para poder revisar los detalles</td>
      <td>5</td>
    </tr>
    <tr>
      <td>19</td>
      <td>US19</td>
      <td>Envio de informe del mantenimiento</td>
      <td>Cómo mecánico quiero realizar y enviar un informe del servicio brindado para documentar los trabajos realizados</td>
      <td>5</td>
    </tr>
    <tr>
      <td>20</td>
      <td>US20</td>
      <td>Notificación de finalización del servicio</td>
      <td>Cómo mecánico quiero finalizar y notificar la culminación del servicio para informar al cliente que su vehículo está listo</td>
      <td>3</td>
    </tr>
    <tr>
      <td>21</td>
      <td>US21</td>
      <td>Gestión de ingresos</td>
      <td>Cómo mecánico quiero gestionar los ingresos generados por el servicio para llevar un registro preciso de los pagos recibidos</td>
      <td>5</td>
    </tr>
    <tr>
      <td>22</td>
      <td>US22</td>
      <td>Visualizar historial de mantenimiento</td>
      <td>Cómo mecánico quiero acceder al historial de mantenimiento realizado a los vehículos para tener un registro de las reparaciones anteriores</td>
      <td>3</td>
    </tr>
    <tr>
      <td>23</td>
      <td>US23</td>
      <td>Comunicación con soporte</td>
      <td>Cómo Owner quiero comunicarme con alguien de soporte a través del apartado de soporte para solicitar ayuda o presentar algún reclamo</td>
      <td>3</td>
    </tr>
    <tr>
      <td>24</td>
      <td>US24</td>
      <td>Visualizar historial de reservas</td>
      <td>Como cliente quiero ver historial de reservas para llevar un seguimiento de uso</td>
      <td>3</td>
    </tr>
    <tr>
      <td>25</td>
      <td>US25</td>
      <td>Comunicación con soporte</td>
      <td>Como cliente quiero comunicarme con alguien de soporte a través del apartado de soporte para solicitar ayuda o presentar algún reclamo.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>26</td>
      <td>US26</td>
      <td>Comunicación con soporte</td>
      <td>Como mecánico quiero comunicarme con alguien de soporte a través del apartado de soporte para solicitar ayuda o presentar algún reclamo.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>27</td>
      <td>US27</td>
      <td>Visualizacion de planes</td>
      <td>Como cliente quiero ver los planes del servicio para elegir uno adecuado.</td>
      <td>5</td>
    </tr>
    <tr>
      <td>28</td>
      <td>US28</td>
      <td>Servicios</td>
      <td>Como cliente quiero saber los beneficios del servicio para elegir un plan de suscripción.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>29</td>
      <td>US29</td>
      <td>Conocer al equipo</td>
      <td>Como cliente quiero informarme sobre el equipo a cargo del proyecto para conocer sus objetivos.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>30</td>
      <td>US30</td>
      <td>Información del producto</td>
      <td>Como cliente quiero ver informacion general sobre el servicio.</td>
      <td>5</td>
    </tr>
    <tr>
      <td>31</td>
      <td>US31</td>
      <td>Ingreso de cuenta</td>
      <td>Como cliente quiero ingresar a una cuenta para ver mi suscripción, mi información y la disponibilidad de vehiculos.</td>
      <td>8</td>
    </tr>
  </tbody>
</table>
