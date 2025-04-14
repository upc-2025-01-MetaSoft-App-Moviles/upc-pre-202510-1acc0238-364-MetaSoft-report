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
        <td> Título User Story 15 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 15
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 15 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 15</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 16 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-16 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 16 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 16
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 16 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 16</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 17 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-17 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 17 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 17
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 17 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 17</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 18 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-18 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 18 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 18
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 18 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 18 </strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 19 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-19 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 19 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 19
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 19 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 19</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 20 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-20 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 20 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 20
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 20 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 20</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 21 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-21 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 21 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 21
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 21 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 21</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 22 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-22 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 22 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 22
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 22 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 22</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 23 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-23 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 23 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 23
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 23 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 23</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 24 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-24 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 24 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 24
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 24 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 24</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 25 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-25 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 25 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 25
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 25 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 25</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 26 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-26 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 26 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 26
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 26 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 26</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 27 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-27 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 27 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 27
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 27 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 27</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 28 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-28 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 28 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 28
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 28 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 28</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 29 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-29 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 29 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 29
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 29 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 29</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 30 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-30 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 30 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 30
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 30 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 30</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 31 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-31 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 31 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 31
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 31 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 31</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 32 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-32 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 32 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 32
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 32 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 32</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
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
        <td> Título User Story 36 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 36
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 36 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 36</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 37 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-37 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 37 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 37
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 37 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 37</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 38 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-38 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 38 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 38
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 38 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 38</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 39 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-39 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 39 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 39
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 39 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 39</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 40 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-40 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 40 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 40
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 40 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 40</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 41 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-41 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 41 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 41
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 41 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 41</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
    <!-- /////////////////////////////////// FILA DE USER STORY 42 /////////////////////////////////// -->
    <!-- /////////////////////////////////////////////////////////////////////////////////////// -->
    <tr>
        <td> US-42 </td>
        <!-- ================== Título ================== -->
        <td> Título User Story 42 </td>
        <!-- ================== Descripción ================== -->
        <td> 
            Descripción User Story 42
        </td>
        <!-- ================== Criterios de Aceptación ================== -->
        <td>
            <strong>Scenario 1: User Story 42 </strong><br><br>
            <br><br>
            <strong>Scenario 2: User Story 42</strong><br><br>
        </td>
        <!-- ================== Relacionado con EPIC ================== -->
        <td> Epic-# </td>
    </tr>
</tbody>
</table>


## 3.3. Impact Mapping.


## 3.4. Product Backlog.






