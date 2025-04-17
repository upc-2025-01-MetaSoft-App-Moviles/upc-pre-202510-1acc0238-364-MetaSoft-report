# Capítulo III: Requirements specification

---

## 3.1. To-Be Scenario Mapping.

**Josep Grau**

![](../../assets/img/chapter-III/Josep%20Grau.png)


**Luis Gómez**

![](../../assets/img/chapter-III/Luis%20G%C3%B3mez.png)


## 3.2. User Stories.

<table>
<thead>
    <tr>
        <th> Epic ID </th>
        <th> Título </th>
        <th> Descripción </th>
        <th> Criterios de Aceptación </th>
        <th> Relacionado con (Epic ID) </th>
    </tr>
</thead>
<tbody>
    <!-- /////////////////////////////////// FILA DE EPIC 01 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> EPIC-01 </td>
        <!-- ================= Título de EPIC ================= -->
        <td> 
            Gestión Integral del Proceso de Vinificación 
        </td>
        <!-- ================= Descripción de EPIC ================= -->
        <td> 
            Como vinicultor, necesito registrar, monitorear y controlar cada una de las 
            fases del proceso de vinificación desde la recepción del lote hasta el embotellado
            para asegurar la trazabilidad, calidad del producto y cumplimiento de los parámetros 
            técnicos establecidos.
        </td>
        <td> N/A </td>
        <td> N/A </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE EPIC 02 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> EPIC-02 </td>
        <!-- ================= Título de EPIC ================= -->
        <td> 
            Gestión de Insumos en Campo y Bodega
        </td>
        <!-- ================= Descripción de EPIC ================= -->
        <td> 
            Como vinicultor, necesito registrar el inventario de insumos, asociarlos a tareas 
            y controlar su consumo tanto en campo como en bodega, para asegurar la disponibilidad 
            de materiales y evitar interrupciones en el proceso productivo.
        </td>
        <td> N/A </td>
        <td> N/A </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE EPIC 03 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> EPIC-03 </td>
        <!-- ================= Título de EPIC ================= -->
        <td> 
            Planificación y Asignación de Actividades Agrícolas
        </td>
        <!-- ================= Descripción de EPIC ================= -->
        <td> 
            Como vinicultor, necesito planificar, calendarizar y asignar tareas agrícolas a 
            parcelas o lotes, para coordinar eficientemente el trabajo del campo y 
            asegurar la ejecución oportuna de actividades como poda, 
            riego y fertilización.
        </td>
        <td> N/A </td>
        <td> N/A </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE EPIC 04 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> EPIC-04 </td>
        <!-- ================= Título de EPIC ================= -->
        <td> 
            Bitácora de Campo Digital y Reportes
        </td>
        <!-- ================= Descripción de EPIC ================= -->
        <td> 
            Como trabajador de campo, necesito registrar de manera rápida y sencilla la ejecución 
            de tareas, observaciones del terreno e incidencias, para generar una bitácora 
            digital útil para el vinicultor en la toma de decisiones.
        </td>
        <td> N/A </td>
        <td> N/A </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE EPIC 05 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> EPIC-05 </td>
        <!-- ================= Título de EPIC ================= -->
        <td> 
            Historial de Producción y Campañas
        </td>
        <!-- ================= Descripción de EPIC ================= -->
        <td> 
            Como vinicultor, necesito consultar el historial de campañas anteriores con sus 
            respectivos datos de producción y resultados, para realizar comparaciones, tomar 
            decisiones estratégicas y documentar el conocimiento acumulado.
        </td>
        <td> N/A </td>
        <td> N/A </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE EPIC 06 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> EPIC-06 </td>
        <!-- ================= Título de EPIC ================= -->
        <td> 
            Interfaz Móvil Adaptada al Usuario de Campo
        </td>
        <!-- ================= Descripción de EPIC ================= -->
        <td> 
            Como trabajador de campo, necesito una interfaz móvil sencilla, visual y guiada, 
            que facilite la interacción con la aplicación, considerando mi bajo nivel de 
            experiencia digital y el uso frecuente en condiciones de campo.
        </td>
        <td> N/A </td>
        <td> N/A </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE EPIC 07 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> EPIC-07 </td>
        <!-- ================= Título de EPIC ================= -->
        <td> 
            Descubrimiento y Valoración de ElixirLine a través de la Landing Page
        </td>
        <!-- ================= Descripción de EPIC ================= -->
        <td> 
            Como visitante de la landing page, quiero explorar de forma clara y 
            atractiva qué es ElixirLine, cómo puede ayudarme en la gestión 
            de viñedos y vinificación artesanal, y qué beneficios ofrece, 
            para decidir si es una solución adecuada para mis necesidades 
            como productor o trabajador del sector vitivinícola.
        </td>
        <td> N/A </td>
        <td> N/A </td>
    </tr>
</tbody>
</table>

---

<table>
<thead>
    <tr>
        <th> Story ID </th>
        <th> Título </th>
        <th> Descripción </th>
        <th> Criterios de Aceptación </th>
        <th> Relacionado con (Epic ID) </th>
    </tr>
</thead>
<tbody>
    <!-- /////////////////////////////////// FILA DE USER STORY 01 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
     <tr>
        <!-- ================== Story ID ================== -->
        <td>US-01</td>
        <!-- ================== Título ================== -->
        <td>
            Hipervínculos en el encabezado
        </td>
        <!-- ================== Descripción ================== -->
        <td>
            Como visitante que llega a la landing page, quiero que los hipervínculos en el 
            encabezado sean claramente visibles y funcionales para poder navegar fácilmente 
            por la aplicación.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong> Scenario 1: Visualización clara de enlaces de navegación </strong> <br>
            Given un visitante en la landing page<br>
            When el sitio web se carga completamente<br>
            Then los hipervínculos en el encabezado están disponibles para el usuario.
            <br><br>
            <strong> Scenario 2: Navegación efectiva mediante hipervínculos </strong> <br>
            Given un visitante en la landing page <br>
            When el visitante hace clic en cualquier hipervínculo en el encabezado <br>
            Then es redirigido a la sección correspondiente de la landing page.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td>EPIC-09</td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 02 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <!-- ================== Story ID ================== -->
        <td>US-02</td>
        <!-- ================== Título ================== -->
        <td>
            Introducción clara y atractiva sobre ElixirLine
        </td>
        <!-- ================== Descripción ================== -->
        <td>
            Como visitante que llega a la landing page, quiero una introducción clara y 
            atractiva a la aplicación ElixirLine, para entender de forma rápida su propósito 
            y cómo puede ayudarme en el proceso productivo de vinos.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Introducción visible desde el primer vistazo </strong><br><br>
            Given un visitante en la landing page <br>
            When el visitante llega a la página <br>
            Then la introducción de la aplicación está visible y 
            presenta claramente el propósito de ElixirLine.
            <br><br>
            <strong>Scenario 2: Comunicación efectiva del propósito de ElixirLine </strong><br><br>
            Given un visitante en la landing page<br>
            When el visitante lee la introducción<br>
            Then puede entender el propósito de la aplicación y cómo ayuda en el proceso productivo de vinos.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td>EPIC-09</td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 03 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <!-- ================== Story ID ================== -->
        <td>US-03</td>
        <!-- ================== Título ================== -->
        <td>
            Información sobre beneficios de la aplicación
        </td>
        <!-- ================== Descripción ================== -->
        <td>
            Como visitante con rol de vinicultor que evalúa diferentes opciones, quiero ver los 
            beneficios específicos de usar ElixirLine, para comprender cómo puede mejorar la operabilidad del 
            proceso productivo de vinos.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Visualización clara de los beneficios</strong><br><br>
            Given un vinicultor en la landing page<br>
            When el visitante accede a la sección de beneficios<br>
            Then los beneficios específicos de ElixirLine están claramente visibles.
            <br><br>
            <strong>Scenario 2: Comprensión del valor de ElixirLine para vinicultores</strong><br><br>
            Given un vinicultor en la landing page<br>
            When el visitante revisa los beneficios<br>
            Then puede comprender cómo la aplicación mejora la gestión de inventario y procesos de venta.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td>EPIC-09</td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 04 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <!-- ================== Story ID ================== -->
        <td>US-04</td>
        <!-- ================== Título ================== -->
        <td>
            Opciones de precios claras para decisiones informadas
        </td>
        <!-- ================== Descripción ================== -->
        <td>
            Como visitante con rol de vinicultor e interesado en adquirir ElixirLine, quiero 
            ver una tabla de precios clara y detallada, para tomar una decisión informada sobre 
            el plan que mejor se adapta a mis necesidades.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Sección de precios accesible y legible </strong><br><br>
            Given un vinicultor en la landing page<br>
            When el visitante accede a la sección de precios<br>
            Then las opciones de precios están claramente visibles.
            <br><br>
            <strong>Scenario 2: Comparación fácil entre planes disponibles</strong><br><br>
            Given un vinicultor en la landing page<br>
            When el visitante revisa las opciones de precios<br>
            Then puede comparar las características de cada plan y tomar una decisión informada.
        </td>
        <!-- ================== Relacionado con EPIC ================== --> 
        <td>EPIC-09</td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 05 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <!-- ================== Story ID ================== -->
        <td>US-05</td>
        <!-- ================== Título ================== -->
        <td>
            Acceso fácil a soporte y asesoramiento
        </td>
        <!-- ================== Descripción ================== -->
        <td>
            Como visitante que tiene preguntas adicionales, quiero encontrar fácilmente la 
            información de contacto, para poder comunicarme con el soporte o el equipo de 
            ventas de ElixirLine.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Acceso directo a la información de contacto </strong><br><br>
            Given un visitante en la landing page<br>
            When el visitante llega a la sección de contacto<br>
            Then puede encontrar la información de contacto para comunicarse con el equipo de soporte o ventas.
            <br><br>     
            <strong>Scenario 2: Opción de enviar consultas desde la landing page </strong><br><br>
            Given un visitante en la landing page<br> 
            When el visitante busca realizar una consulta<br> 
            Then tiene la opción de enviar su consulta a través de los canales de contacto disponibles.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td>EPIC-09</td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 06 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <!-- ================== Story ID ================== -->
        <td>US-06</td>
        <!-- ================== Título ================== -->
        <td>
            Opiniones de usuarios que inspiran confianza
        </td>
        <!-- ================== Descripción ================== -->
        <td>
            Como visitante con rol de vinicultor que está considerando usar ElixirLine, quiero 
            leer testimonios de otros usuarios, para conocer sus experiencias y validar la 
            efectividad de la aplicación.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Testimonios visibles en sección dedicada</strong><br><br>
            Given un vinicultor en la landing page<br>
            When el visitante llega a la sección de testimonios<br>
            Then puede leer las opiniones de otros usuarios de ElixirLine.
            <br><br>
            <strong>Scenario 2: Validación de la efectividad mediante experiencias de usuarios</strong><br><br>
            Given un vinicultor en la landing page<br>
            When el visitante revisa los testimonios<br>
            Then puede validar la efectividad de la aplicación a partir de las experiencias compartidas.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td>EPIC-09</td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 07 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <!-- ================== Story ID ================== -->
        <td>US-07</td>
        <!-- ================== Título ================== -->
        <td> Navegación fluida en dispositivos móviles </td>
        <!-- ================== Descripción ================== -->  
        <td>
            Como visitante que llega a la landing page, quiero que la navegación de la landing page 
            sea fácil y fluida en mi dispositivo móvil, para poder acceder a la información sin 
            interrupciones o problemas de visualización.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Fluidez en la navegación móvil </strong><br><br>
            Given un usuario accede a la landing page desde un dispositivo móvil<br>
            When carga el sitio web en su totalidad<br>
            Then la navegación es fluida y sin problemas de desplazamiento o funcionalidad.
            <br><br>
            <strong>Scenario 2: Menús responsive adaptados a pantallas pequeñas</strong><br><br>
            Given un usuario accede desde un dispositivo móvil<br>
            When intenta utilizar los menús de navegación<br>
            Then los menús se adaptan correctamente al tamaño de pantalla y permiten una navegación eficiente.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td>EPIC-09</td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 08 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <!-- ================== Story ID ================== -->
        <td>US-08</td>
        <!-- ================== Título ================== -->
        <td>Adaptación de la landing page en tabletas</td>
        <!-- ================== Descripción ================== -->
        <td>
            Como visitante que llega a la landing page, quiero que la navegación de la landing 
            page sea fácil y fluida en mi dispositivo móvil, para poder acceder a la información
            sin interrupciones o problemas de visualización.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Contenido optimizado para pantallas de tabletas </strong><br><br>
            Given un usuario accede a la landing page desde una tableta<br>
            When se carga el sitio web completamente<br>
            Then el contenido se ajusta adecuadamente al tamaño de la pantalla de la tableta.
            <br><br>    
            <strong>Scenario 2: Proporción adecuada de imágenes y textos en tabletas </strong><br><br>
            Given un usuario accede desde una tableta<br>   
            When revisa la disposición de imágenes y textos<br>   
            Then estos elementos mantienen las proporciones correctas y son legibles.
        </td>
        <!-- ================== Relacionado con EPIC ================== --> 
        <td>EPIC-09</td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 09 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-09 </td>
        <!-- ================== Título ================== -->
        <td> 	Registro del lote de uvas </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como vinicultor, quiero registrar los datos del lote de uvas al ingresar a la bodega, para llevar un control desde el inicio del proceso de vinificación.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Registro de información del lote recibido </strong><br><br>
            Given un vinicultor en la interfaz de registro <br>
            When recibe un nuevo lote <br>
            Then puede ingresar variedad, peso, fecha de recolección.
            <br><br>
            <strong>Scenario 2: Asignación de identificador único al lote </strong><br><br>
            Given un lote registrado <br>
            When se completa el formulario <br>
            Then se guarda con un identificador único y fecha de ingreso.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> EPIC-01 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 10 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-10 </td>
        <!-- ================== Título ================== -->
        <td> Seguimiento de la fermentación </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como vinicultor, quiero registrar y consultar los parámetros de fermentación, para asegurar que se mantengan dentro de los rangos adecuados.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Ingreso de parámetros durante fermentación </strong><br><br>
            Given un vinicultor accede al módulo de fermentación<br>
            When se realiza una medición<br>
            Then puede registrar temperatura, densidad y pH.
            <br><br>
            <strong>Scenario 2: Alerta por desviación de parámetros </strong><br><br>
            Given un lote en fermentación<br>
            When revisa su historial<br>
            Then puede ver la evolución de parámetros y recibir alertas si hay desviaciones.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> EPIC-01 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 11 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-11 </td>
        <!-- ================== Título ================== -->
        <td> Control de la fase de clarificación </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como vinicultor, quiero registrar el inicio y los productos usados en la clarificación, para asegurar la transparencia del vino y cumplir con las especificaciones.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Registro de productos utilizados en clarificación </strong><br><br>
            Given un lote que pasa a clarificación <br>
            When se registra la fase <br>
            Then se indican los insumos aplicados y la fecha de inicio.
            <br><br>
            <strong>Scenario 2: Consulta de análisis post-clarificación </strong><br><br>
            Given un lote en clarificación <br>
            When accede al seguimiento <br>
            Then puede ver resultados de análisis posteriores y definir el tiempo de espera.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> EPIC-01 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 12 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-12 </td>
        <!-- ================== Título ================== -->
        <td> Gestión del prensado </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como vinicultor, quiero registrar la fase de prensado y su rendimiento, para evaluar la eficiencia del proceso y planificar las siguientes etapas.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Ingreso de datos del proceso de prensado </strong><br><br>
            Given un lote listo para prensar <br>
            When se inicia la fase <br>
            Then se ingresan los datos de máquina usada, duración y rendimiento.
            <br><br>
            <strong>Scenario 2: Evaluación del rendimiento del prensado </strong><br><br>
            Given un prensado realizado <br>
            When se revisa el resumen <br>
            Then se muestra cantidad extraída y porcentaje respecto al lote original.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> EPIC-01 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 13 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-13 </td>
        <!-- ================== Título ================== -->
        <td> Control del añejamiento </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como vinicultor, quiero registrar el inicio del añejamiento y los parámetros del ambiente, para mantener la calidad del producto durante esta fase.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Registro de condiciones iniciales del añejamiento </strong><br><br>
            Given un lote en barricas <br>
            When se inicia el proceso <br>
            Then se registra tipo de barrica, humedad, temperatura y duración estimada.
            <br><br>
            <strong>Scenario 2: Seguimiento del ambiente en añejamiento </strong><br><br>
            Given un vinicultor revisando el proceso <br>
            When accede al seguimiento <br>
            Then puede consultar cambios de parámetros y notas técnicas.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> EPIC-01 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 14 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-14 </td>
        <!-- ================== Título ================== -->
        <td> Registro del embotellado </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como vinicultor, quiero registrar los detalles del embotellado final, para cerrar el ciclo del lote con toda la trazabilidad documentada.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Ingreso de datos del embotellado final </strong><br><br>
            Given un lote listo para embotellar <br>
            When se realiza la operación <br>
            Then se indican fecha, cantidad de botellas, tipo de envase y etiqueta.
            <br><br>
            <strong>Scenario 2: Visualización de trazabilidad completa </strong><br><br>
            Given un lote embotellado <br>
            When accede al resumen <br>
            Then se visualiza toda la trazabilidad del lote desde la recepción hasta el embotellado.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> EPIC-01 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 15 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-15 </td>
        <!-- ================== Título ================== -->
        <td> Asignación de Tareas a Parcela y Trabajador </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como vinicultor, quiero asignar tareas específicas a trabajadores en parcelas concretas, para coordinar eficientemente las actividades del campo.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Asignación detallada</strong><br><br>
            Given el vinicultor accede al panel de tareas<br>
            When selecciona una tarea y un trabajador<br>
            Then puede asignarla a una parcela específica y establecer fecha de ejecución.
            <br><br>
            <strong>Scenario 2: Notificación al trabajador</strong><br><br>
            Given una tarea ha sido asignada<br>
            When se guarda la asignación<br>
            Then el trabajador recibe la notificación correspondiente en su dispositivo.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> EPIC-03 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 16 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-16 </td>
        <!-- ================== Título ================== -->
        <td> Consulta del Historial de Actividades Agrícolas </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como vinicultor, quiero consultar el historial de actividades realizadas en cada lote, para tener un registro claro y tomar decisiones informadas.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Filtro de historial</strong><br><br>
            Given el vinicultor accede al módulo de historial<br>
            When aplica filtros por lote o fecha<br>
            Then se muestra una lista con las tareas realizadas y sus detalles.<br><br>
            <strong>Scenario 2: Visualización completa</strong><br><br>
            Given una tarea histórica seleccionada<br>
            When revisa los detalles<br>
            Then puede ver el trabajador, fecha, insumos utilizados y comentarios adjuntos.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> EPIC-05 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 17 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-17 </td>
        <!-- ================== Título ================== -->
        <td> Panel de Notificaciones de Campo </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como vinicultor, quiero recibir notificaciones en tiempo real de incidencias o tareas completadas, para estar al tanto del progreso y actuar rápidamente si hay problemas.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Alerta de incidencia</strong><br><br>
            Given un trabajador reporta una incidencia<br>
            When se envía el formulario<br>
            Then el vinicultor recibe una notificación con los detalles del evento.<br><br>
            <strong>Scenario 2: Notificación de tarea completada</strong><br><br>
            Given una tarea es marcada como completada<br>
            When el sistema actualiza el estado<br>
            Then se notifica al vinicultor con la información del lote y el trabajador.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> EPIC-04 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 18 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-18 </td>
        <!-- ================== Título ================== -->
        <td> Visualización de Tareas Asignadas desde el Móvil </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como trabajador de campo, quiero ver las tareas que me han sido asignadas en mi celular, para saber qué actividades debo realizar en el día y dónde.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Lista de tareas diarias</strong><br><br>
            Given el trabajador inicia sesión en su dispositivo<br>
            When accede a su perfil<br>
            Then ve las tareas asignadas con fecha, ubicación e instrucciones.<br><br>
            <strong>Scenario 2: Gestión del estado de tareas</strong><br><br>
            Given el trabajador realiza una tarea<br>
            When actualiza el estado<br>
            Then puede marcarla como “En progreso” o “Completada”.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> EPIC-04 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 19 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-19 </td>
        <!-- ================== Título ================== -->
        <td> Registro Rápido de Incidencias </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como trabajador de campo, quiero registrar rápidamente una incidencia como una plaga o problema técnico, para que el vinicultor pueda tomar acción cuanto antes.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Creación rápida de reporte</strong><br><br>
            Given el trabajador detecta una incidencia<br>
            When accede al formulario de reporte<br>
            Then puede ingresar descripción, foto y ubicación del problema.<br><br>
            <strong>Scenario 2: Envío y notificación</strong><br><br>
            Given un reporte ha sido completado<br>
            When lo envía<br>
            Then el vinicultor es notificado inmediatamente con los datos ingresados.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> EPIC-04 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 20 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-20 </td>
        <!-- ================== Título ================== -->
        <td> Modo Simplificado con Íconos Grandes </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como trabajador con poca experiencia digital, quiero una interfaz con íconos grandes y pasos guiados, para poder usar la app sin confundirme o perderme.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Activación del modo simplificado</strong><br><br>
            Given el trabajador accede a la app<br>
            When elige el modo de uso<br>
            Then puede activar el modo con íconos grandes y navegación guiada.<br><br>
            <strong>Scenario 2: Flujo asistido</strong><br><br>
            Given el modo está activado<br>
            When realiza una acción como “Registrar tarea”<br>
            Then recibe instrucciones paso a paso para completarla correctamente.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> EPIC-06 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY US-21 /////////////////////////////////// -->
<!-- /////////////////////////////////////////////////////////////////////////////////////// -->
<tr>
    <td> US-21 </td>
    <!-- ================== Título ================== -->
    <td> Registro de insumos en bodega y campo </td>
    <!-- ================== Descripción ================== -->
    <td> 
        Como vinicultor, necesito registrar manualmente el inventario de insumos tanto en la bodega como en el campo, para disponer de información actualizada y facilitar mis decisiones de reabastecimiento.
    </td>
    <!-- ================== Criterios de Aceptación ================== -->
    <td>
        <strong>Scenario 1: Registro con datos completos</strong><br><br>
        Given que se inicia el registro de un insumo,<br>
        When se ingresan todos los datos obligatorios (nombre, cantidad, ubicación),<br>
        Then el sistema almacena la información y confirma el registro.<br><br>
        <strong>Scenario 2: Validación de campos obligatorios</strong><br><br>
        Given que se intenta registrar un insumo sin datos obligatorios,<br>
        When se finaliza el proceso de registro,<br>
        Then el sistema rechaza el registro e indica los datos faltantes.
    </td>
    <!-- ================== Relacionado con EPIC ================== -->
    <td> EPIC-02 </td>
</tr>
<!-- /////////////////////////////////// FILA DE USER STORY US-22 /////////////////////////////////// -->
<!-- /////////////////////////////////////////////////////////////////////////////////////// -->
<tr>
    <td> US-22 </td>
    <!-- ================== Título ================== -->
    <td> Actualización manual de detalles de insumos </td>
    <!-- ================== Descripción ================== -->
    <td> 
        Como vinicultor, necesito poder actualizar los detalles de un insumo registrado en campo o bodega, para corregir errores o modificar información según requerimientos.
    </td>
    <!-- ================== Criterios de Aceptación ================== -->
    <td>
        <strong>Scenario 1: Actualización exitosa de insumo</strong><br><br>
        Given que existe un insumo previamente registrado,<br>
        When se ingresan cambios válidos en la información,<br>
        Then el sistema guarda la actualización y confirma el cambio.<br><br>
        <strong>Scenario 2: Manejo de intento de actualización inexistente</strong><br><br>
        Given que se intenta actualizar un insumo no registrado,<br>
        When se procesa la solicitud de actualización,<br>
        Then el sistema retorna un mensaje de error indicando que el insumo no existe.
    </td>
    <!-- ================== Relacionado con EPIC ================== -->
    <td> EPIC-02 </td>
</tr>
<!-- /////////////////////////////////// FILA DE USER STORY US-23 /////////////////////////////////// -->
<!-- /////////////////////////////////////////////////////////////////////////////////////// -->
<tr>
    <td> US-23 </td>
    <!-- ================== Título ================== -->
    <td> Consulta histórica del inventario de insumos </td>
    <!-- ================== Descripción ================== -->
    <td> 
        Como vinicultor, necesito consultar el historial de registros de insumos, para analizar la evolución de mi inventario y apoyar mis decisiones de gestión sin depender de actualizaciones en tiempo real.
    </td>
    <!-- ================== Criterios de Aceptación ================== -->
    <td>
        <strong>Scenario 1: Búsqueda por fecha</strong><br><br>
        Given que se solicita el historial del inventario,<br>
        When se filtra la información por un rango de fechas,<br>
        Then el sistema muestra un listado con los registros de insumos correspondientes.<br><br>
        <strong>Scenario 2: Visualización de información histórica</strong><br><br>
        Given que se accede al historial general,<br>
        When se visualizan los registros,<br>
        Then cada entrada presenta los datos ingresados y la fecha de registro de forma comprobable.
    </td>
    <!-- ================== Relacionado con EPIC ================== -->
    <td> EPIC-02 </td>
</tr>
<!-- /////////////////////////////////// FILA DE USER STORY US-24 /////////////////////////////////// -->
<!-- /////////////////////////////////////////////////////////////////////////////////////// -->
<tr>
    <td> US-24 </td>
    <!-- ================== Título ================== -->
    <td> Modo tutorial interactivo inicial </td>
    <!-- ================== Descripción ================== -->
    <td> 
        Como trabajador de campo, necesito que la aplicación ofrezca un tutorial interactivo en el primer uso, para aprender a utilizar las funciones básicas de forma guiada y sin complicaciones.
    </td>
    <!-- ================== Criterios de Aceptación ================== -->
    <td>
        <strong>Scenario 1: Presentación del tutorial en el primer acceso</strong><br><br>
        Given que el trabajador inicia la aplicación por primera vez,<br>
        When se inicia la sesión inicial,<br>
        Then el sistema despliega un tutorial interactivo que explica las funciones básicas.<br><br>
        <strong>Scenario 2: Acceso a repetición del tutorial</strong><br><br>
        Given que el trabajador requiere repasar el funcionamiento,<br>
        When solicita el tutorial nuevamente desde la sección de ayuda,<br>
        Then el sistema permite reproducir la guía interactiva.
    </td>
    <!-- ================== Relacionado con EPIC ================== -->
    <td> EPIC-06 </td>
</tr>
<!-- /////////////////////////////////// FILA DE USER STORY US-25 /////////////////////////////////// -->
<!-- /////////////////////////////////////////////////////////////////////////////////////// -->
<tr>
    <td> US-25 </td>
    <!-- ================== Título ================== -->
    <td> Navegación simplificada en la aplicación móvil </td>
    <!-- ================== Descripción ================== -->
    <td> 
        Como trabajador de campo, necesito una navegación intuitiva y organizada en la aplicación móvil, para acceder de forma sencilla a mis tareas e información esencial sin distracciones.
    </td>
    <!-- ================== Criterios de Aceptación ================== -->
    <td>
        <strong>Scenario 1: Organización clara de secciones</strong><br><br>
        Given que se requiere acceder a funcionalidades de la aplicación,<br>
        When se visualiza el menú principal,<br>
        Then las secciones se presentan de forma organizada y con iconografía clara.<br><br>
        <strong>Scenario 2: Accesibilidad sin complejidad</strong><br><br>
        Given que el trabajador interactúa con la aplicación,<br>
        When se selecciona una función, por ejemplo "Consultar tareas",<br>
        Then el sistema redirige a la sección correspondiente sin requerir pasos adicionales complejos.
    </td>
    <!-- ================== Relacionado con EPIC ================== -->
    <td> EPIC-06 </td>
</tr>
<!-- /////////////////////////////////// FILA DE USER STORY US-26 /////////////////////////////////// -->
<!-- /////////////////////////////////////////////////////////////////////////////////////// -->
<tr>
    <td> US-26 </td>
    <!-- ================== Título ================== -->
    <td> Retroalimentación de acciones sin dependencia de monitoreo en tiempo real </td>
    <!-- ================== Descripción ================== -->
    <td> 
        Como trabajador de campo, necesito recibir confirmación visual y auditiva de las acciones que realice, para tener seguridad de que se han completado, sin depender de actualizaciones instantáneas en la nube.
    </td>
    <!-- ================== Criterios de Aceptación ================== -->
    <td>
        <strong>Scenario 1: Confirmación inmediata de la acción</strong><br><br>
        Given que el trabajador ejecuta una acción, por ejemplo "Registrar actividad",<br>
        When se finaliza la acción,<br>
        Then el sistema muestra un mensaje de confirmación y emite una señal auditiva de éxito.<br><br>
        <strong>Scenario 2: Disponibilidad de confirmación en modo offline</strong><br><br>
        Given que el trabajador está en modo offline,<br>
        When realiza una acción,<br>
        Then el sistema almacena la acción localmente y muestra un aviso confirmatorio en la pantalla.
    </td>
    <!-- ================== Relacionado con EPIC ================== -->
    <td> EPIC-06 </td>
</tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 27 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-27 </td>
        <!-- ================== Título ================== -->
        <td> Edición del calendario de tareas </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como vinicultor, quiero modificar la fecha o el responsable de una tarea ya asignada, para adaptarme a imprevistos o cambios en la planificación operativa.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Edición de fecha asignada </strong><br><br>
            Given una tarea ha sido previamente asignada<br>
            When el vinicultor edita la fecha de ejecución<br>
            Then el sistema actualiza la tarea con la nueva fecha.
            <br><br>
            <strong>Scenario 2: Reasignación de responsable</strong><br><br>
            Given una tarea cuenta con un trabajador asignado<br>
            When el vinicultor reasigna la tarea a otro trabajador<br>
            Then el sistema guarda y refleja el nuevo responsable asignado.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-03 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 28 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-28 </td>
        <!-- ================== Título ================== -->
        <td> Exportación de reportes de campañas </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como vinicultor, quiero exportar un resumen de una campaña finalizada, para compartir los datos de producción o analizarlos en futuras decisiones.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Generación de reporte con filtros aplicados </strong><br><br>
            Given el vinicultor selecciona una campaña y aplica filtros<br>
            When solicita la generación del reporte<br>
            Then el sistema genera un archivo con la información filtrada.
            <br><br>
            <strong>Scenario 2: Descarga del archivo generado</strong><br><br>
            Given el reporte ha sido generado correctamente<br>
            When el vinicultor decide descargarlo<br>
            Then el sistema permite obtener el archivo en formato compatible (PDF o Excel).
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-05 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 29 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-29 </td>
        <!-- ================== Título ================== -->
        <td> Soporte para zonas sin conexión (modo offline) </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como trabajador de campo, quiero registrar mis actividades sin depender de una conexión a internet, para asegurar el ingreso de datos incluso en zonas rurales.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Registro de actividades en modo offline </strong><br><br>
            Given el dispositivo no cuenta con conexión a internet<br>
            When el trabajador registra una actividad<br>
            Then el sistema almacena la información de forma local.
            <br><br>
            <strong>Scenario 2: Sincronización automática al reconectar</strong><br><br>
            Given el dispositivo recupera la conexión<br>
            When el sistema detecta registros pendientes<br>
            Then sincroniza automáticamente los datos almacenados.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-06 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 30 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-30 </td>
        <!-- ================== Título ================== -->
        <td> Consulta de historial de incidencias por parcela </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como vinicultor, quiero consultar el historial de incidencias reportadas por parcela, para identificar patrones y tomar decisiones preventivas.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Filtro por parcela </strong><br><br>
            Given el vinicultor accede a la sección de incidencias<br>
            When selecciona una parcela específica<br>
            Then el sistema muestra todas las incidencias registradas en esa ubicación.
            <br><br>
            <strong>Scenario 2: Visualización de detalles</strong><br><br>
            Given se selecciona una incidencia del historial<br>
            When el vinicultor revisa la información<br>
            Then puede ver la fecha, descripción, trabajador que la reportó y estado de atención.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-04 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 31 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-31 </td>
        <!-- ================== Título ================== -->
        <td> Confirmación de lectura de tareas asignadas </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como vinicultor, quiero saber si un trabajador ha revisado las tareas que se le asignaron, para asegurarme de que está al tanto de sus actividades diarias.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Registro automático de lectura </strong><br><br>
            Given una tarea ha sido asignada a un trabajador<br>
            When el trabajador accede a su lista de tareas<br>
            Then el sistema registra automáticamente que ha sido leída.
            <br><br>
            <strong>Scenario 2: Visualización por parte del vinicultor</strong><br><br>
            Given el vinicultor accede a la planificación del día<br>
            When revisa una tarea<br>
            Then puede ver si el trabajador correspondiente ya la leyó o no.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-03 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 32 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-32 </td>
        <!-- ================== Título ================== -->
        <td> Registro de comentarios al completar una tarea </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como trabajador de campo, quiero poder añadir un comentario al finalizar una tarea, para dejar observaciones relevantes sobre su ejecución.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Campo opcional de comentarios </strong><br><br>
            Given el trabajador marca una tarea como completada<br>
            When finaliza el registro<br>
            Then puede añadir un comentario si lo considera necesario.
            <br><br>
            <strong>Scenario 2: Acceso del vinicultor al comentario</strong><br><br>
            Given la tarea fue completada con un comentario<br>
            When el vinicultor consulta esa tarea<br>
            Then puede ver el comentario asociado al cierre.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-04 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 33 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-33 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 33 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 33
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 33 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 33</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 34 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-34 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 34 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 34
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 34 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 34</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 35 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-35 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 35 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 35
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 35 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 35</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 36 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-36 </td>
        <!-- ================== Título ================== -->
        <td> Registro detallado del consumo de insumos  </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como vinicultor, quiero que los insumos usados se registren por tarea y lote, para asegurar un control preciso del inventario y trazabilidad.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Registro desde avance de tarea</strong><br><br>
            Given un trabajador de campo completando una actividad <br>
            When registra el avance desde su celular <br>
            Then puede ingresar los insumos utilizados y las cantidades, asociadas automáticamente al lote y tarea.
            <br><br>
            <strong>Scenario 2: Consulta del consumo por lote</strong><br><br>
            Given un vinicultor en el panel de un lote <br>
            When accede a la sección de insumos <br>
            Then puede ver el detalle de uso por tarea, fecha y trabajador.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> EPIC-02 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 37 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-37 </td>
        <!-- ================== Título ================== -->
        <td> Consulta de historial de campañas anteriores </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como vinicultor, quiero consultar campañas pasadas con sus datos de producción, para tomar mejores decisiones estratégicas.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Visualización general del historial</strong><br><br>
            Given un vinicultor accediendo al historial <br>
            When selecciona una campaña pasada <br>
            Then ve datos de cosecha, rendimiento, condiciones e incidencias registradas.
            <br><br>
            <strong>Scenario 2: Comparación entre campañas</strong><br><br>
            Given un vinicultor comparando años anteriores <br>
            When selecciona dos campañas <br>
            Then puede ver comparaciones visuales de rendimiento, fechas clave y resultados.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> EPIC-05 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 38 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-38 </td>
        <!-- ================== Título ================== -->
        <td> Vista semanal de tareas para trabajadores </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como trabajador de campo, quiero ver mis tareas organizadas por día, para planificar mejor mi semana y saber qué debo hacer.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Vista semanal desde el inicio de sesión</strong><br><br>
            Given un trabajador inicia sesión en la app <br>
            When accede al calendario semanal <br>
            Then ve sus tareas asignadas por fecha y tipo de actividad.
            <br><br>
            <strong>Scenario 2: Detalle de tarea desde la vista semanal</strong><br><br>
            Given un trabajador revisando su semana <br>
            When selecciona una tarea del calendario <br>
            Then accede al detalle con lote, hora, descripción e insumos necesarios.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> EPIC-03 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 39 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-39 </td>
        <!-- ================== Título ================== -->
        <td> Reporte automático de actividades diarias </td>
        <!-- ================== Descripción ================== -->
        <td>
             Como vinicultor, quiero recibir un resumen diario de las tareas realizadas en campo, para mantenerme informado del progreso sin tener que revisar cada registro.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Generación de reporte diario al finalizar el día</strong><br><br>
            Given que ha finalizado la jornada <br>
            When el sistema procesa los registros del día <br>
            Then se genera un reporte con las tareas completadas, responsables y observaciones.
            <br><br>
            <strong>Scenario 2: Notificación del reporte al vinicultor</strong><br><br>
            Given un vinicultor suscrito a reportes diarios <br>
            When el sistema genera el resumen <br>
            Then el vinicultor recibe una notificación con acceso al reporte desde su celular.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> EPIC-04 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 40 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-40 </td>
        <!-- ================== Título ================== -->
        <td> Asignación rápida de tareas por lote </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como vinicultor, quiero asignar múltiples tareas a un lote de forma rápida, para planificar el trabajo con mayor eficiencia.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: Asignación desde la vista del lote</strong><br><br>
            Given un vinicultor en el panel de un lote <br>
            When selecciona “Asignar tareas” <br>
            Then puede elegir múltiples actividades y asignarlas por fecha y trabajador.
            <br><br>
            <strong>Scenario 2: Confirmación de asignación</strong><br><br>
            Given que el vinicultor ha completado la asignación <br>
            When guarda los cambios <br>
            Then el sistema confirma la asignación y notifica a los trabajadores correspondientes.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> EPIC-03 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 41 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-41 </td>
        <!-- ================== Título ================== -->
        <td> Registro fotográfico de incidencias </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como trabajador de campo, quiero registrar fotos junto a comentarios sobre problemas detectados, para que el vinicultor pueda tomar decisiones más rápido.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <<strong>Scenario 1: Registro de incidencia con foto</strong><br><br>
            Given un trabajador detecta un problema en el campo <br>
            When selecciona “Registrar incidencia” <br>
            Then puede tomar una foto, escribir un comentario y asociarlo al lote.
            <br><br>
            <strong>Scenario 2: Revisión de incidencias por el vinicultor</strong><br><br>
            Given el vinicultor accede a su panel de incidencias <br>
            When abre una alerta registrada <br>
            Then puede ver la foto, descripción, hora y autor del registro.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> EPIC-04 </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 42 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-42 </td>
        <!-- ================== Título ================== -->
        <td> Interfaz simplificada para registrar tareas </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Como trabajador de campo, quiero una forma rápida y clara de marcar tareas como completadas, para ahorrar tiempo y evitar confusiones.
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
             <strong>Scenario 1: Registro directo desde la pantalla principal</strong><br><br>
            Given un trabajador con una tarea pendiente <br>
            When accede al resumen diario <br>
            Then puede marcar como “completado” y añadir comentarios en pocos pasos.
            <br><br>
            <strong>Scenario 2: Confirmación visual del registro</strong><br><br>
            Given que el trabajador registra una tarea como hecha <br>
            When se confirma el envío <br>
            Then el sistema muestra un mensaje visual claro de éxito y la tarea se oculta del pendiente.
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> EPIC-06 </td>
    </tr>
</tbody>
</table>


## 3.3. Impact Mapping.


## 3.4. Product Backlog.






