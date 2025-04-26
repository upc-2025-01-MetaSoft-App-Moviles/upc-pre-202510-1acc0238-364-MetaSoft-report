# Capítulo IV: Solution Software Design

---

## 4.1. Strategic-Level Domain-Driven Design

### 4.1.1. EventStorming

Para el desarrollo de esta sección, se adoptó la técnica de Event Storming, un método colaborativo que facilita la 
exploración profunda del dominio de una aplicación. A través de diversas sesiones de trabajo, y con el apoyo de 
la herramienta Miro, fue posible construir el flujo general y detallar los pasos clave del proceso. En una primera 
fase, se recopilaron diferentes perspectivas sobre los eventos relevantes del dominio, los cuales fueron organizados 
según criterios como su frecuencia y relevancia, entre otros.

**Step 1: Unstructured Exploration**

En esta fase, se definieron los eventos principales que reflejan las acciones más relevantes dentro del sistema.

<img src="../../assets/img/chapter-IV/EventStorming-Unstructured-Exploration.png" alt="">

--- 

**Step 2: Timelines**

Luego, se dispusieron los eventos en una línea de tiempo con el objetivo de visualizar el flujo 
de interacciones y la secuencia entre ellos. Esta disposición cronológica ayuda a identificar 
dependencias y momentos clave, lo que contribuye a un diseño más claro y coherente del sistema.

<img src="../../assets/img/chapter-IV/EventStorming-Timelines.png" alt="">

--- 

**Step 3: Paint Points**

En el tercer paso, identificamos "Pain Points" o cuellos de botella en el flujo de eventos.

<img src="../../assets/img/chapter-IV/EventStorming-Paint-Points.png" alt="">

--- 

**Step 4: Pivotal Points**

Identificamos los "Pivotal Points",  Estos puntos son esenciales para el flujo del sistema, y su correcta implementación asegura un funcionamiento fluido.

<img src="../../assets/img/chapter-IV/EventStorming-Pivotal-Points.png" alt="">

--- 

**Step 5: EventStorming-Commands**

Finalmente, se definieron los comandos que pueden ser ejecutados por los distintos roles dentro del sistema. Cada rol cuenta con permisos específicos, lo que garantiza que los usuarios tengan acceso únicamente a las funciones que les corresponden según su perfil

<img src="../../assets/img/chapter-IV/EventStorming-Commands.png" alt="">


#### 4.1.1.1. Candidate Context Discovery

**Step 6: Policies**

En esta etapa, se definieron políticas específicas para regular la interacción entre los distintos componentes del sistema. Estas directrices permiten mantener la coherencia del funcionamiento general y contribuyen a reducir posibles riesgos operativos.

**Step 7: Read Models**

Se definieron modelos de lectura que representan el estado actual del sistema. Estos modelos permiten acceder a información actualizada en todo momento, lo cual facilita la consulta de datos relevantes y apoya una mejor toma de decisiones por parte de los usuarios.

**Step 8: External-Systems**

Se identificaron sistemas externos que interactúan con la aplicación, los cuales son esenciales para la ejecución de ciertas funciones. Para manejar estas interacciones, se implementaron mecanismos que permiten gestionar adecuadamente las dependencias y asegurar una integración eficiente.

<img src="../../assets/img/chapter-IV/External-Systems.png" alt="">

**Step 9: Aggregates**

Se definieron agregados que agrupan de forma lógica entidades relacionadas, lo cual ayuda a mantener la coherencia interna y promueve el modularidad del sistema.

**Step 10: Bounded Context**

Finalmente, se definieron los Bounded Contexts, cada uno con responsabilidades claras y bien delimitadas. Esto permite una mejor organización del sistema, facilita el mantenimiento y asegura una alineación más efectiva con los objetivos del negocio.

<img src="../../assets/img/chapter-IV/Bounded-Context.png" alt="">

#### 4.1.1.2. Domain Message Flows Modeling

En esta sección se presenta el modelado de los flujos de mensajes dentro del dominio, utilizando
la técnica de EventStorming. Esta metodología permitió identificar los eventos clave y 
comprender sus interacciones. Con base en estos eventos, se elaboraron diagramas que ilustran 
cómo se comunican los distintos componentes del sistema para cumplir con los objetivos del 
negocio. A continuación, se muestran los diagramas de flujo de mensajes correspondientes a los
contextos previamente definidos.

**Step 11: Domain Message Flows Modeling**

<img src="../../assets/img/chapter-IV/Domain-Message-Flows-Modeling.png" alt="">


#### 4.1.1.3. Bounded Context Canvases

Para lograr una mejor organización del dominio y una comunicación clara entre equipos, 
se desarrollaron Bounded Context Canvases que delimitan responsabilidades, definen 
modelos clave y establecen interacciones entre contextos. Esta sección presenta los 
canvases elaborados, los cuales sirvieron como guía para estructurar y alinear el 
diseño del sistema.

**Bounded Context Canvas: Vinification Process Management**

<img src="../../assets/img/chapter-IV/Vinification-Process-Management-Bounded-Context-Canvas.jpg" alt="">

**Bounded Context Canvas: Supply Management**

<img src="../../assets/img/chapter-IV/Supply-Management-Bounded-Context-Canvas.jpg" alt="">

**Bounded Context Canvas: Agricultural Activities**

<img src="../../assets/img/chapter-IV/Agricultural-Activities-Bounded-Context-Canvas.jpg" alt="">

**Bounded Context Canvas: Digital Field Log**

<img src="../../assets/img/chapter-IV/Digital-Field-Log-Bounded-Context-Canvas.jpg" alt="">

**Bounded Context Canvas: Production History and Campaigns**

<img src="../../assets/img/chapter-IV/Production-History-and-Campaigns-Bounded-Context-Canvas.jpg" alt="">

**Bounded Context Canvas: Identity and Access Management - IAM**

<img src="../../assets/img/chapter-IV/Identity-and-Access-Management-IAM-Bounded-Context-Canvas.jpg" alt="">


### 4.1.2. Context Mapping

En esta sección, se presenta el mapeo de contextos, que permite visualizar las interacciones 
y dependencias entre los diferentes contextos delimitados en la fase anterior. 
Este mapeo es fundamental para comprender cómo se relacionan los distintos componentes 
del sistema y cómo fluyen los datos entre ellos.



### 4.1.3. Software Architecture

En esta sección, se presenta la arquitectura de software del sistema, que incluye tanto la arquitectura de alto nivel como la de bajo nivel. La arquitectura de alto nivel proporciona una visión general de los componentes principales y sus interacciones, mientras que la arquitectura de bajo nivel detalla la implementación específica de cada componente.

#### 4.1.3.1. Software Architecture Context Level Diagrams

El diagrama de nivel de contexto de ElixirLine muestra las interacciones clave entre el sistema principal, sistema externo y sus usuarios principales:

* Vinicultor: Responsables de gestionar el ciclo completo de producción
* Trabajador de campo: Encargados de ejecutar tareas agrícolas bajo la dirección del vinicultor

<img src="../../assets/img/chapter-IV/Diagrama-contexto-ElixirLine.png" alt="">


#### 4.1.3.2. Software Architecture Container Level Diagrams

Este diagrama detalla la arquitectura de los contenedores de ElixirLine, mostrando los componentes principales del sistema:

* Landing Page: Sitio web donde los vinicultores pueden informarse sobre la aplicación y registrarse.
* Mobile App: Aplicación móvil destinada a los trabajadores de campo para recibir y reportar tareas agrícolas asignadas por el vinicultor.
* Backend: Servicio REST que gestiona y procesa la información de los datos.
* Database: Base de datos donde se almacena la información relacionada con las actividades de producción del viñedo, vinicultores y trabajadores de campo.

<img src="../../assets/img/chapter-IV/Diagrama-contenedores-ElixirLine.png" alt="">

#### 4.1.3.3. Software Architecture Deployment Diagrams

Nuestro servidor backend y de base de datos se desplegará utilizando la nube de Google Cloud Platform (GCP).

<img src="../../assets/img/chapter-IV/Software-Architecture-Deployment-ElixirLine.png" alt="">


## 4.2. Tactical-Level Domain-Driven Design

### 4.2.1.  Bounded Context: "Bounded Context Name"

En esta sección, nuestro equipo presenta las clases identificadas detalladas a manera de
diccionario, explicando para cada una su nombre, propósito y la documentación de
atributos y métodos considerados, junto con las relaciones entre ellas.

---

### **Bounded Context Name: "Vinification Process Management"**

<table>
<thead>
    <tr>
        <th>Class Name: WineBatch</th>
    </tr>
</thead>
<tbody>
    <tr>
        <td>
            Propósito: <br>
            Representa un conjunto de uvas procesadas de manera conjunta a lo largo de las etapas de vinificación.
        </td>
    </tr>
    <tr>
        <td>
            <strong> Atributos: </strong><br> 
            batchId: UUID – Identificador único del lote.<br> 
            grapeVariety: String – Tipo de uva utilizada (e.g., Tempranillo, Malbec).<br> 
            receptionDate: Date – Fecha de ingreso del lote al sistema.<br> 
            currentStage: Enum (Recepción, Fermentación, Clarificación, etc.) – Etapa actual del proceso.<br> 
            technicalParameters: Parámetros Técnicos – Parámetros técnicos asociados.<br> 
            stages: List[VinificationStage] – Historial completo de las etapas por las que ha pasado el lote.<br> 
        </td>
    </tr>
    <tr>
        <td>
            <strong> Métodos: </strong><br>
            advanceStage(): Cambia la etapa del lote y actualiza el historial.<br>
            addParameters(params: TechnicalParameters): Asocia parámetros a una etapa.<br>
            completeBatch(): Marca el lote como completado para el histórico.<br>
        </td>
    </tr>
</tbody>
</table>


<table>
<thead>
    <tr>
        <th>Class Name: VinificationStage</th>
    </tr>
</thead>
<tbody>
    <tr>
        <td>
            Propósito: <br>
            Representa una etapa específica dentro del proceso de vinificación.
        </td>
    </tr>
    <tr>
        <td>
            <strong> Atributos: </strong><br> 
            stageType: Enum (Recepción, Fermentación, Clarificación, etc.) <br>
            startDate: Date <br> 
            endDate: Date? <br>
            status: Enum (Pendiente, En curso, Finalizada, Incidencia) <br>
            notes: String? <br>
        </td>
    </tr>
    <tr>
        <td>
            <strong> Métodos: </strong><br> 
            start(): Cambia estado a "En curso". <br> 
            complete(): Establece fecha de fin y cambia estado. <br>
            reportIncident(comentario: String): Registra desviación con comentario. <br>
        </td>
    </tr>
</tbody>
</table>

<table>
<thead>
    <tr>
        <th>Class Name: TechnicalParameters</th>
    </tr>
</thead>
<tbody>
    <tr>
        <td>
            Propósito: <br>
            Representa los parámetros técnicos asociados a una etapa de vinificación.
        </td>
    </tr>
    <tr>
        <td>
            <strong> Atributos: </strong><br> 
            brix: Double – Grado Brix (azúcares).<br>
            ph: Double – Nivel de acidez.<br>
            temperature: Double – Medición en °C.<br>
            measurementDate: Date<br>
        </td>
    </tr>
    <tr>
        <td>
            <strong> Métodos: </strong><br> 
            validarRango(): Verifica si los valores están dentro de límites aceptables.
        </td>
    </tr>
</tbody>
</table>

<table>
<thead>
    <tr>
        <th>Class Name: ProcessAlert</th>
    </tr>
</thead>
<tbody>
    <tr>
        <td>
            Propósito: <br>
            Representa una alerta generada por el sistema en caso de desviaciones o problemas en el proceso.
        </td>
    </tr>
    <tr>
        <td>
            <strong> Atributos: </strong><br> 
            alertId: UUID <br> 
            alertType: Enum (Desviación técnica, Retraso, Parámetro fuera de rango) <br> 
            description: String <br> 
            date: Date <br> 
            associatedBatch: WineBatch <br> 
        </td>
    </tr>
    <tr>
        <td>
            <strong> Métodos: </strong><br> 
            enviarNotificacion(): Dispara un evento para ser visualizado o registrado. <br> 
            esCritica(): Devuelve true si la alerta compromete la calidad del lote. <br> 
        </td>
    </tr>
</tbody>
</table>

<table>
<thead>
    <tr>
        <th>Class Name: ProcessLog</th>
    </tr>
</thead>
<tbody>
    <tr>
        <td>
            Propósito: <br>
            Consolidación de toda la información generada durante el ciclo de vida del lote, para consulta o exportación.        </td>
    </tr>
    <tr>
        <td>
            <strong> Atributos: </strong><br> 
            lote: LoteDeVino <br> 
            parametrosHistoricos: List[ParametrosTecnicos> <br> 
            etapas: List[EtapaVinificacion> <br> 
            alertas: List[AlertaProceso] <br> 
        </td>
    </tr>
    <tr>
        <td>
            <strong> Métodos: </strong><br> 
            exportarFormato(tipo: String): Genera archivo en PDF/Excel.<br> 
            resumenLote(): Devuelve resumen estructurado del ciclo de vida del lote. <br> 
        </td>
    </tr>
</tbody>
</table>

**Relaciones Clave**

1. [ ] WineBatch tiene una lista de VinificationStage
2. [ ] Cada VinificationStage puede contener un conjunto de TechnicalParameters
3. [ ] WineBatch puede generar múltiples ProcessAlert
4. [ ] ProcessLog actúa como agregador de toda la información del lote

---

### **Bounded Context Name: "Supply Management"**

<table>
<thead>
    <tr>
        <th>Class Name: SupplyItem</th>
    </tr>
</thead>
<tbody>
    <tr>
        <td>
            Propósito: <br>
            Representa un insumo o material utilizado en el proceso de vinificación.
        </td>
    </tr>
    <tr>
        <td>
            <strong> Atributos: </strong><br> 
            supplyId: UUID – Identificador único del insumo.<br>
            name: String – Nombre del insumo (ej. fertilizante, levadura, solución de limpieza).<br>
            category: String – Tipo de insumo (ej. agrícola, procesamiento, limpieza).<br>
            quantityAvailable: Double – Cantidad disponible actualmente.<br>
            unit: String – Unidad de medida (ej. kg, L, unidades).<br>
            minimumStockLevel: Double – Nivel mínimo de stock para disparar una alerta.<br>
            lastUpdated: Date – Fecha de última actualización del inventario.<br>
        </td>
    </tr>
    <tr>
        <td>
            <strong> Métodos: </strong><br> 
            decreaseQuantity(amount: Double): Disminuye la cantidad disponible del insumo en la cantidad especificada.<br> 
            increaseQuantity(amount: Double): Incrementa la cantidad disponible del insumo en la cantidad especificada.<br> 
            isBelowMinimum(): Verifica si la cantidad disponible está por debajo del nivel mínimo permitido.<br> 
        </td>
    </tr>
</tbody>
</table>
 

<table>
<thead>
    <tr>
        <th>Class Name: SupplyMovement</th>
    </tr>
</thead>
<tbody>
    <tr>
        <td>
            Propósito: <br>
            Representa un movimiento de insumo, ya sea entrada o salida del inventario.
        </td>
    </tr>
    <tr>
        <td>
            <strong> Atributos: </strong><br> 
            movementId: UUID – Identificador único del movimiento de insumo. <br>
            supplyItem: SupplyItem – Referencia al insumo afectado por el movimiento. <br>
            movementType: Enum (Inbound, Outbound, Adjustment) – Tipo de movimiento: entrada, salida o ajuste. <br> 
            quantity: Double – Cantidad involucrada en el movimiento. <br>
            movementDate: Date – Fecha en que se realizó el movimiento. <br>
            associatedTaskOrBatchId: UUID? – ID opcional de la tarea o lote asociado al movimiento. 
        </td>
    </tr>
    <tr>
        <td>
            <strong> Métodos: </strong><br> 
            registerMovement(): Registra el movimiento y actualiza el stock correspondiente.
        </td>
    </tr>
</tbody>
</table>


<table>
<thead>
    <tr>
        <th>Class Name: StockAlert</th>
    </tr>
</thead>
<tbody>
    <tr>
        <td>
            Propósito: <br>
            Representa una alerta generada por el sistema cuando un insumo está por debajo del nivel mínimo de stock.
        </td>
    </tr>
    <tr>
        <td>
            <strong> Atributos: </strong><br> 
            alertId: UUID – Identificador único de la alerta. <br> 
            supplyItem: SupplyItem – Insumo asociado a la alerta. <br> 
            alertType: Enum (StockBelowMinimum) – Tipo de alerta generada. <br> 
            description: String – Descripción breve del motivo de la alerta.
        </td>
    </tr>
    <tr>
        <td>
            <strong> Métodos: </strong><br> 
            triggerNotification(): Envía una notificación sobre la alerta de bajo stock.
        </td>
    </tr>
</tbody>
</table>

<table>
<thead>
    <tr>
        <th>Class Name: SupplyAssignment</th>
    </tr>
</thead>
<tbody>
    <tr>
        <td>
            Propósito: <br>
            Representa la asignación de insumos a tareas o lotes específicos dentro del proceso de vinificación.
        </td>
    </tr>
    <tr>
        <td>
            <strong> Atributos: </strong><br> 
            assignmentId: UUID – Identificador único de la asignación. <br> 
            supplyItem: SupplyItem – Insumo asignado. <br> 
            assignedTo: UUID – Identificador de la tarea o lote al que se asigna el insumo. <br> 
            assignedQuantity: Double – Cantidad de insumo asignada. <br> 
            assignmentDate: Date – Fecha de la asignación.
        </td>
    </tr>
    <tr>
        <td>
            <strong> Métodos: </strong><br> 
            confirmAssignment(): Confirma la asignación del insumo a la tarea o lote correspondiente. <br> 
        </td>
    </tr>
</tbody>
</table>


**Relaciones Clave**

1. [ ] SupplyItem es referenciado por SupplyMovement, SupplyAssignment y StockAlert.
2. [ ] SupplyMovement modifica la cantidad de SupplyItem.
3. [ ] SupplyAssignment asocia insumos a tareas o lotes de vinificación.
4. [ ] StockAlert se dispara cuando SupplyItem.isBelowMinimum() es true.

---

### **Bounded Context Name: "Agricultural Activities"**

<table>
<thead>
    <tr>
        <th>Class Name: AgriculturalTask</th>
    </tr>
</thead>
<tbody>
    <tr>
        <td>
            Propósito: <br>
            Representa una tarea agrícola específica que debe ser ejecutada por un trabajador de campo.
        </td>
    </tr>
    <tr>
        <td>
            <strong> Atributos: </strong><br> 
            taskId: UUID – Identificador único de la tarea.<br> 
            title: String – Título breve de la tarea (ej. "Poda de invierno").<br> 
            description: String – Descripción detallada de la actividad a realizar.<br> 
            parcelId: UUID – Identificador del lote o parcela donde se realizará la tarea.<br> 
            assignedTo: UUID – Identificador del trabajador asignado.<br> 
            scheduledDate: Date – Fecha programada para ejecutar la tarea.<br> 
            status: Enum (Scheduled, InProgress, Completed, Cancelled) – Estado actual de la tarea.<br> 
        </td>
    </tr>
    <tr>
        <td>
            <strong> Métodos: </strong><br> 
            startTask(): Cambia el estado de la tarea a "InProgress". <br>
            completeTask(): Marca la tarea como completada. <br>
            cancelTask(reason: String): Cancela la tarea con una justificación. <br>
        </td>
    </tr>
</tbody>
</table>


<table>
<thead>
    <tr>
        <th>Class Name: TaskExecutionReport</th>
    </tr>
</thead>
<tbody>
    <tr>
        <td>
            Propósito: <br>
            Almacena información sobre la ejecución real de una tarea agrícola.
        </td>
    </tr>
    <tr>
        <td>
            <strong> Atributos: </strong><br> 
            reportId: UUID – Identificador único del reporte. <br> 
            taskId: UUID – Tarea agrícola a la que pertenece el reporte. <br> 
            executorId: UUID – Usuario que ejecutó la tarea. <br> 
            executionDate: Date – Fecha real de ejecución. <br> 
            observations: String – Comentarios o notas del ejecutor. <br> 
            evidencePhotos: List[String> – URLs de fotos o evidencia visual adjunta. <br> 
        </td>
    </tr>
    <tr>
        <td>
            <strong> Métodos: </strong><br> 
            attachEvidence(photoUrl: String): Agrega una foto como evidencia al reporte. <br>
            updateObservations(text: String): Modifica las observaciones del reporte. <br>
        </td>
    </tr>
</tbody>
</table>


<table>
<thead>
    <tr>
        <th>Class Name: TaskNotification</th>
    </tr>
</thead>
<tbody>
    <tr>
        <td>
            Propósito: <br>
            Representa una notificación enviada a un usuario sobre una tarea agrícola.
        </td>
    </tr>
    <tr>
        <td>
            <strong> Atributos: </strong> <br> 
            notificationId: UUID – Identificador único de la notificación. <br> 
            recipientId: UUID – Usuario que recibirá la notificación. <br> 
            taskId: UUID – Tarea asociada a la notificación. <br> 
            message: String – Mensaje a mostrar. <br> 
            sentDate: Date – Fecha de envío. <br> 
            readStatus: Boolean – Indica si el usuario ya leyó la notificación.
        </td>
    </tr>
    <tr>
        <td>
            <strong> Métodos: </strong><br> 
            markAsRead(): Cambia el estado de la notificación a "Leída". <br> 
        </td>
    </tr>
</tbody>
</table>


<table>
<thead>
    <tr>
        <th>Class Name: Parcel</th>
    </tr>
</thead>
<tbody>
    <tr>
        <td>
            Propósito: <br>
            Representa una parcela o lote específico donde se realizan actividades agrícolas.
        </td>
    </tr>
    <tr>
        <td>
            <strong> Atributos: </strong> <br> 
            parcelId: UUID – Identificador único de la parcela. <br> 
            name: String – Nombre o referencia de la parcela. <br> 
            area: Double – Tamaño de la parcela en hectáreas. <br> 
            cropType: String – Tipo de cultivo actual. <br> 
            location: String – Descripción o coordenadas geográficas. <br> 
        </td>
    </tr>
    <tr>
        <td>
            <strong> Métodos: </strong><br> 
            updateCropType(newCrop: String): Actualiza el tipo de cultivo de la parcela.
        </td>
    </tr>
</tbody>
</table>


**Relaciones Clave**

1. [ ] AgriculturalTask se relaciona con Parcel mediante parcelId.
2. [ ] TaskExecutionReport está vinculado a AgriculturalTask.
3. [ ] TaskNotification está asociada a AgriculturalTask y a un usuario.
4. [ ] Parcel agrupa tareas por ubicación geográfica.

---

### **Bounded Context Name: "Digital Field Log"**

<table>
<thead>
    <tr>
        <th>Class Name: FieldLogEntry</th>
    </tr>
</thead>
<tbody>
    <tr>
        <td>
            Propósito: <br>
            Representa un registro digital de observaciones o eventos en campo.
        </td>
    </tr>
    <tr>
        <td>
            <strong> Atributos: </strong><br> 
            entryId: UUID – Identificador único del registro. <br>
            authorId: UUID – Identificador del trabajador que creó la entrada. <br>
            parcelId: UUID – Parcela o lote asociado al registro. <br>
            entryType: Enum (Incident, Observation, CompletedTask) – Tipo de entrada registrada. <br>
            description: String – Descripción del evento, incidencia o actividad observada. <br>
            timestamp: DateTime – Fecha y hora del registro. <br>
        </td>
    </tr>
    <tr>
        <td>
            <strong> Métodos: </strong><br> 
            updateDescription(newText: String): Permite modificar la descripción. <br>
            reclassifyEntry(newType: Enum): Cambia el tipo de entrada. <br>
        </td>
    </tr>
</tbody>
</table>


<table>
<thead>
    <tr>
        <th>Class Name: PhotoEvidence</th>
    </tr>
</thead>
<tbody>
    <tr>
        <td>
            Propósito: <br>
            Representa una foto o evidencia visual asociada a un registro de campo.
        </td>
    </tr>
    <tr>
        <td>
            <strong> Atributos: </strong><br> 
            photoId: UUID – Identificador único de la foto. <br>
            entryId: UUID – Identificador del registro al que está asociada la foto. <br>
            photoUrl: String – URL donde se almacena la imagen. <br>
            description: String? – Descripción opcional de la foto. <br>
        </td>
    </tr>
    <tr>
        <td>
            <strong> Métodos: </strong><br> 
            updateDescription(text: String): Modifica la descripción de la imagen.<br>
            removePhoto(): Elimina la evidencia visual del sistema <br>
        </td>
    </tr>
</tbody>
</table>


<table>
<thead>
    <tr>
        <th>Class Name: TaskCompletionRecord</th>
    </tr>
</thead>
<tbody>
    <tr>
        <td>
            Propósito: <br>
            Representa el registro de la finalización de una tarea agrícola.
        </td>
    </tr>
    <tr>
        <td>
            <strong> Atributos: </strong><br> 
            recordId: UUID – Identificador único del registro. <br> 
            taskId: UUID – Tarea asociada al registro. <br>
            workerId: UUID – Usuario que completó la tarea. <br>
            completedAt: DateTime – Fecha y hora de finalización. <br> 
            comments: String – Comentarios adicionales sobre la ejecución. <br>
        </td>
    </tr>
    <tr>
        <td>
            <strong> Métodos: </strong><br> 
            editComments(text: String): Permite actualizar los comentarios del registro.
        </td>
    </tr>
</tbody>
</table>

<table>
<thead>
    <tr>
        <th>Class Name: FieldUser</th>
    </tr>
</thead>
<tbody>
    <tr>
        <td>
            Propósito: <br>
            Representa a los trabajadores de campo que interactúan con el sistema.
        </td>
    </tr>
    <tr>
        <td>
            <strong> Atributos: </strong><br> 
            userId: UUID – Identificador único del trabajador. <br>
            name: String – Nombre completo. <br>
            role: Enum (FieldWorker, Supervisor) – Rol del usuario. <br>
            assignedParcels: List[UUID> – Lista de parcelas asignadas al usuario. <br> 
        </td>
    </tr>
    <tr>
        <td>
            <strong> Métodos: </strong><br> 
            assignParcel(parcelId: UUID): Asigna una nueva parcela al trabajador. <br> 
            changeRole(newRole: Enum): Cambia el rol del usuario. <br> 
        </td>
    </tr>
</tbody>
</table>



**Relaciones Clave**

1. [ ] FieldLogEntry se relaciona con Parcel y con FieldUser.
2. [ ] PhotoEvidence está vinculada a una FieldLogEntry.
3. [ ] TaskCompletionRecord complementa una tarea agrícola ejecutada y puede generar una entrada en FieldLogEntry.
4. [ ] FieldUser crea entradas y reportes de ejecución.

---

### **Bounded Context Name: "Production History and Campaigns"**

<table>
<thead>
    <tr>
        <th>Class Name: ProductionRecord</th>
    </tr>
</thead>
<tbody>
    <tr>
        <td>
            Propósito: <br>
            Representa un registro de producción asociado a un lote específico.
        </td>
    </tr>
    <tr>
        <td>
            <strong> Atributos: </strong><br> 
            recordId: UUID – Identificador único del registro de producción. <br>
            batchId: UUID – Identificador del lote asociado. <br> 
            startDate: DateTime – Fecha de inicio del registro productivo. <br>
            endDate: DateTime – Fecha de finalización del registro. <br>
            volumeProduced: Float – Volumen producido en litros. <br>
            qualityMetrics: Map[String, Float> – Indicadores de calidad asociados (pH, °Brix, acidez, etc.). <br>
        </td>
    </tr>
    <tr>
        <td>
            <strong> Métodos: </strong><br> 
            updateVolumeProduced(volume: Float): Permite actualizar el volumen registrado.
            addQualityMetric(metricName: String, value: Float): Agrega un nuevo indicador de calidad.
            closeRecord(): Marca el registro como cerrado/finalizado
        </td>
    </tr>
</tbody>
</table>


<table>
<thead>
    <tr>
        <th>Class Name: BatchHistory</th>
    </tr>
</thead>
<tbody>
    <tr>
        <td>
            Propósito: <br>
            Representa el historial de producción de un lote específico.
        </td>
    </tr>
    <tr>
        <td>
            <strong> Atributos: </strong><br> 
            historyId: UUID – Identificador único del historial. <br> 
            batchId: UUID – Lote asociado al historial. <br> 
            productionRecords: List[ProductionRecord> – Lista de registros de producción asociados. <br> 
            totalProduced: Double – Total producido en litros. <br> 
        </td>
    </tr>
    <tr>
        <td>
            <strong> Métodos: </strong><br> 
            addProductionRecord(record: ProductionRecord): Agrega un nuevo registro al historial.<br> 
            calculateTotalProduced(): Calcula el total producido a partir de los registros.<br> 
        </td>
    </tr>
</tbody>
</table>


**Relaciones Clave**

1. [ ] ProductionRecord está vinculado a un Batch.
2. [ ] BatchHistory agrega múltiples ProductionRecord para un mismo lote.

---

#### 4.2.1.1. Domain Layer


#### 4.2.1.2. Interface Layer


#### 4.2.1.3. Application Layer


#### 4.2.1.4. Infrastructure Layer


#### 4.2.1.5. Bounded Context Software Architecture Component Level Diagrams

En esta sección se presentan los diagramas de nivel de componente de la arquitectura del API REST del contexto delimitado. Estos diagramas ilustran la estructura interna de los componentes,

<img src="../../assets/img/chapter-IV/Diagrama-de-componentes-ElixirLine.png" alt="">

#### 4.2.1.6. Bounded Context Software Architecture Code Level Diagrams


#### 4.2.1.6.1. Bounded Context Domain Layer Class Diagrams


#### 4.2.1.6.2. Bounded Context Database Design Diagram