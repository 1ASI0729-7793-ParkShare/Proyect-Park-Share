###  4.1. Style Guidelines.
### 4.1.1. General Style Guidelines.

El diseño visual de Proyect-Park-Share se basa en los principios de claridad, confiabilidad y agilidad operacional. Está pensado para conductores que buscan un estacionamiento sin perder tiempo y propietarios que desean rentabilizar sus cocheras de manera segura y sin complicaciones.

Se prioriza una interfaz limpia e intuitiva, fácil de usar tanto para jóvenes acostumbrados a aplicaciones móviles como para propietarios de mayor edad que prefieren evitar procesos complejos.

#### Principios de diseño:

* Simplicidad: Interfaces despejadas y con baja carga cognitiva para que la reserva o publicación de una cochera se realice en pocos pasos.

* Consistencia: Uso uniforme de patrones visuales, botones y componentes en toda la plataforma para facilitar el aprendizaje.

* Jerarquía visual: Organización de la información según su urgencia, destacando datos críticos como el estado de la reserva, la ubicación en el mapa y el costo por hora.

* Accesibilidad: Diseñado con contrastes adecuados, tipografía legible y botones amplios para asegurar un uso cómodo en cualquier condición.

#### Paleta de colores:
La combinación de colores transmite seguridad, transparencia y dinamismo urbano:


![PaletadeColores](/report/assets/paletadecolores.png)


### Tipografía:
Se selecciona la familia tipográfica Inter por su excelente legibilidad en pantallas digitales de diversos tamaños y su apariencia clara y moderna.

#### Jerarquía tipográfica:

* Heading 1: Títulos principales, Inter, Bold, 28px – 34px.

* Heading 2: Subtítulos y secciones, Inter, Semi-Bold, 20px – 24px.

* Heading 3: Encabezados de tarjetas o modales, Inter, Medium, 16px – 18px.

* Body Text: Texto principal y formularios, Inter, Regular, 14px – 16px.


#### Espaciado:
Se adopta un sistema basado en múltiplos de 8px para asegurar una alineación precisa:

8px: Separación mínima entre elementos estrechos.

16px: Separación estándar entre campos de formulario y botones.

24px: Distancia entre tarjetas o bloques de información.

32px: Margen entre secciones principales del documento o pantalla.


#### Tono de comunicación:

Práctico y accesible: Pensado para agilizar la interacción.

Formal pero cercano: Brinda seguridad en los pagos sin ser rígido.

Claro y sereno: Enfocado en resolver la necesidad de parqueo sin distracciones ni lenguaje confuso.

### 4.1.2. Web Style Guidelines.

1. #### Diseño y Distribución de la Pantalla (Layout)

* La plataforma web de Proyect-Park-Share está diseñada para que la búsqueda y el alquiler de cocheras se realicen de forma rápida e intuitiva.

* Menú Lateral: Una barra fija a la izquierda permite gestionar las cocheras registradas, revisar el historial de reservas y configurar la cuenta.

* Área Principal: Pantalla dividida que muestra el mapa dinámico a un lado y la lista de opciones de parqueo al otro, permitiendo comparar alternativas fácilmente.

* Tarjetas de Información: Recuadros limpios donde se agrupa la información de cada cochera (fotos, precio por hora, dirección y calificación).

2. #### Organización en Rejilla (Grid System)

Para asegurar una presentación limpia y adaptada a distintas pantallas:

* Sistema de grilla flexible basado en 12 columnas para mantener los elementos alineados.

* Espaciado uniforme guiado por múltiplos de 8px (8px, 16px, 24px) que evita la saturación visual.

3. #### Componentes Visuales de la Interfaz

* Tablas de Historial: Utilizadas para detallar las reservas pasadas y los ingresos del propietario, incluyendo filtros por fecha y barra de búsqueda.

* Acciones Principales: En tonos azul o verde para acciones clave como "Reservar ahora" o "Publicar cochera".

* Acciones Secundarias: Botones neutros para acciones como "Ver detalles" o "Volver".

* Estados: Variaciones visuales para indicar cuando el botón está activo, en hover o deshabilitado.

* Etiquetas de Estado: Indicadores visuales en color para identificar rápidamente la situación del parqueo (Disponible, Solicitud Pendiente, Ocupado).

* Formularios: Campos sencillos con etiquetas claras superiores y validación en tiempo real (por ejemplo: "Ingrese una placa válida").

* Avisos y Notificaciones: Alertas flotantes (Toasts) que confirman la reserva o notifican cuando el tiempo de estacionamiento está por concluir.

4. #### Comportamiento Visual e Interacción

* Respuesta Inmediata: Confirmación visual instantánea tras cada acción (guardar datos, solicitar parqueo o cancelar).

* Reglas del Flujo: El sistema bloquea acciones no permitidas, como solicitar una cochera si el vehículo excede las dimensiones permitidas.

* Líneas de Tiempo: Una barra de progreso muestra la etapa actual del servicio (Solicitado > Confirmado > En uso > Finalizado).

5. Adaptación a Pantallas 

- Versión Desktop: Vista completa a pantalla dividida con el mapa interactivo y la lista de resultados en paralelo.


6. Navegación e Iconos

* Barra Superior: Acceso rápido al inicio, selector para alternar entre el perfil de Conductor o Propietario y acceso a la cuenta.

* Iconos: Símbolos simples y de rápida asociación (lupa para buscar, pin para ubicación, auto para parqueo y candado para seguridad).


### 4.2. Information Architecture.

La arquitectura de información de Proyect-Park-Share está pensada para que tanto los conductores que buscan un estacionamiento como los propietarios que alquilan su espacio puedan usar la plataforma de forma rápida, clara y sin perderse.

Se prioriza una estructura sencilla orientada a tareas directas: encontrar una cochera, reservarla o ponerla en alquiler en pocos pasos.


### 4.2.1. Organization Systems.

Los sistemas de organización estructuran los datos de la plataforma para que cualquier usuario pueda realizar sus gestiones sin complicaciones ni rodeos. Para lograrlo, combinamos formas visuales de ordenar la pantalla con listas lógicas adaptadas al uso diario.

#### Organización visual del contenido:

* Organización jerárquica: Se aplica en la pantalla principal y en los detalles del parqueo. Muestra primero la información indispensable (ubicación en el mapa, precio por hora y disponibilidad) y deja en segundo plano los datos secundarios.

* Organización secuencial (Paso a paso): Se utiliza en los procesos principales como el registro de usuarios, la verificación de identidad (DNI y placa) y el flujo de reserva. Guía al usuario paso a paso para evitar equivocaciones.

* Organización matricial: Se aplica en las tablas del panel de control (dashboard). Permite a los propietarios ver de un vistazo varios datos a la vez, como fechas, montos cobrados y estado de sus alquileres.

#### Categorización del contenido:

* Tipo de usuario: La plataforma adapta lo que muestra según el rol activo. Los conductores ven opciones de búsqueda y reservas, mientras que los propietarios acceden a la publicación y cobros.

*Por Secciones: El contenido se agrupa por áreas de interés: Búsqueda, Mis Reservas, Mis Cocheras y Pagos.

* Cronológica: Organiza los historiales de alquileres y los cobros realizados de más reciente a más antiguo.


#### Módulos principales del sistema:

* Inicio / Buscador: Vista principal con el mapa interactivo para ubicar cocheras cercanas.

* Mis Reservas: Sección donde el conductor revisa sus alquileres activos y pasados.

* Mis Cocheras: Panel del propietario para administrar sus espacios, precios y horarios.

* Pagos e Ingresos: Espacio para gestionar tarjetas de crédito/débito y revisar las ganancias obtenidas.

* Perfil y Verificación: Lugar para subir documentos personales (DNI, licencia de conducir y tarjeta de propiedad).

### 4.2.2. Labeling Systems.

El sistema de etiquetado de Proyect-Park-Share está pensado para nombrar cada parte de la plataforma de forma sencilla, breve y coherente. Su meta principal es eliminar dudas al navegar, logrando que tanto un conductor apurado por estacionar como un propietario que alquila su garaje entiendan la pantalla al instante sin encontrarse con términos raros o confusos.

Se prioriza el uso de palabras cotidianas y directas, teniendo en cuenta que los usuarios tienen diferentes niveles de experiencia usando aplicaciones.

#### Principios de etiquetado:

- Simplicidad: Usamos la menor cantidad de palabras posible en cada botón o título. Se evitan modismos técnicos o nombres complicados para que cualquiera identifique rápido para qué sirve cada opción.

- Claridad: La etiqueta indica exactamente lo que va a pasar al hacer clic o qué información contiene la sección, sin dejar espacio a malinterpretaciones.

- Consistencia: Mantenemos las mismas palabras en toda la web y la aplicación. Por ejemplo, usamos siempre el término "Cochera" en lugar de cambiar a cada rato entre "Garaje", "Estacionamiento" o "Parqueo".

- Lenguaje simple: Empleamos un vocabulario habitual y conocido por todos los conductores y dueños de casa, como "Placa", "Reserva", "Ingresos" o "Licencia".

#### Etiquetas de navegación principal (Módulos):

Representan las pantallas clave de la plataforma y permiten moverse de forma directa entre secciones:

- Inicio / Buscar: Pantalla principal con el mapa interactivo para ubicar espacios cercanos.

- Mis Reservas: Sección donde el conductor revisa sus alquileres activos, programados y pasados.

- Mis Cocheras: Panel donde el propietario administra sus espacios registrados, precios y horarios de disponibilidad.

- Mis Ingresos: Espacio para consultar las ganancias acumuladas y el historial de pagos recibidos.

- Verificación: Zona del perfil para subir documentos (DNI, licencia de conducir y tarjeta de propiedad).

- Mi Perfil: Configuración de la cuenta de usuario, teléfono y datos personales.

#### Etiquetas de acciones principales:

- Utilizan verbos claros y directos en infinitivo para indicar qué hará el sistema al presionar el botón:

- Reservar ahora: Inicia el proceso de solicitud de un espacio de parqueo.

- Publicar cochera: Abre el formulario para registrar un nuevo garaje en el sistema.

- Cancelar reserva: Anula un alquiler solicitado o confirmado.

- Confirmar llegada: Notifica al propietario que el vehículo ya ingresó al espacio.

- Finalizar parqueo: Registra la salida del vehículo y cierra el conteo de tiempo.

- Subir documento: Carga las fotos del DNI o licencia para la revisión de identidad.

- Retirar dinero: Solicita la transferencia de los ingresos hacia la cuenta bancaria del propietario.

#### Etiquetas de estado y respuesta:

Permiten al usuario entender de un vistazo la situación de su reserva o su cochera:

- Disponible: Indica que la cochera se encuentra libre para ser reservada de inmediato.

- Ocupada: Señala que el espacio ya cuenta con un vehículo en uso.

- Pendiente: Muestra que la solicitud de reserva está a la espera de confirmación.

- Verificado: Confirma que los documentos presentados han sido validados con éxito.

- En revisión: Avisa que la identidad o la propiedad del garaje aún está siendo comprobada.

#### Etiquetas de asociación:

Sirven para mostrar de forma limpia cómo se conectan los datos dentro de la plataforma sin amontonar la pantalla:

- Cochera asignada: Muestra cuál es el garaje específico vinculado a la reserva activa.

- Vehículo registrado: Indica qué auto y placa están autorizados para ingresar al espacio.

- Propietario responsable: Identifica al dueño de la cochera con quien se coordinará el acceso.

- Pago vinculado: Conecta la boleta o comprobante con el alquiler correspondiente.

### 4.2.3. SEO Tags and Meta Tags

Las etiquetas SEO y las etiquetas Meta de **Proyect-Park-Share** permiten que la plataforma se posicione adecuadamente en los motores de búsqueda como Google. Su función principal es describir de forma directa el propósito de cada vista dentro de la web para ayudar a que los conductores que necesitan estacionamiento y los dueños de estacionamientos nos encuentren fácilmente.

Se configuran directamente en el encabezado HTML de cada vista principal del sitio web y la aplicación mediante los atributos *Title*, *Meta Description*, *Keywords* y *Author*.



#### Página Principal / Bienvenida (Landing Page)

* Title: Proyect-Park-Share | Tu Red de Cocheras Privadas en Lima
* Meta Description:Olvídate del tráfico y busca un estacionamiento seguro por horas o pon en alquiler tu cochera libre para generar dinero extra.
* Keywords: parqueo en lima, estacionamiento por hora, alquilar mi cochera, estacionamiento privado, parqueo seguro
* Author: Equipo Proyect-Park-Share



#### Buscador e Integración de Mapa

* Title: Ubicar Estacionamientos Cercanos | Proyect-Park-Share
* Meta Description: Consulta las cocheras disponibles cerca de tu posición en tiempo real, compara costos por hora y realiza tu reserva al instante.
* Keywords: mapa de parqueos, cocheras libres, reservar estacionamiento, costo por hora parqueo
* Author: Equipo Proyect-Park-Share



#### Módulo de Registro de Espacios (Para Propietarios)

* Title: Publica tu Garage y Genera Ingresos | Proyect-Park-Share
* Meta Description: Registra tu espacio de parqueo desocupado, establece las horas en que está libre y recibe pagos seguros por cada alquiler.
* Keywords: ganar dinero con mi cochera, rentar garage desocupado, alquiler de estacionamiento lima
* Author: Equipo Proyect-Park-Share


#### Acceso y Registro de Usuarios

* Title: Entrar a la Plataforma | Proyect-Park-Share
* Meta Description: Inicia sesión con tu cuenta para administrar tus solicitudes de parqueo activas o revisar los alquileres de tu cochera.
* Keywords: ingreso proyect park share, entrar a mi cuenta, login estacionamiento
* Author: Equipo Proyect-Park-Share



#### Panel Principal de Gestión -Dashboard:

* Title: Resumen de Mi Cuenta | Proyect-Park-Share
* Meta Description: Administra el estado de tus reservas, verifica el conteo de tiempo de parqueo y revisa las ganancias del mes.
* Keywords: resumen de reservas, historial de pagos, panel de control cochera
* Author: Equipo Proyect-Park-Share


### 4.2.4. Searching Systems.

El sistema de búsqueda está pensado para que los conductores encuentren un parqueo disponible rápidamente y sin rodeos, evitando que pierdan tiempo dando vueltas o buscando entre opciones que no se ajustan a su viaje.

Se da prioridad a una búsqueda sencilla, directa y fácil de usar en el día a día, permitiendo ubicar el espacio ideal en pocos clics.


#### Tipos y Formas de Búsqueda

La plataforma incluye una barra de búsqueda clara en la pantalla principal y en el mapa interactivo. El usuario puede buscar un espacio utilizando distintos datos cotidianos:

* Dirección o avenida principal (por ejemplo: "Av. Javier Prado").
* Distrito o zona específica (por ejemplo: *"Surco"* o "Miraflores").
* Puntos de referencia conocidos (por ejemplo: "Cerca al centro comercial" o "Frente a la universidad").
* Nombre del propietario o código de la cochera.



#### Filtros para Ajustar la Búsqueda

Para ayudar al conductor a encontrar justo lo que necesita, el sistema permite filtrar las opciones según criterios prácticos:

##### En la búsqueda de parqueos:

* Rango de precio por hora.
* Horario y fecha necesaria.
* Tamaño del vehículo (auto compacto, camioneta, moto).
* Características (cochera techada, portón automático, vigilancia).


##### En la lista de reservas del usuario:

* Estado de la reserva (activa, pendiente, finalizada, cancelada).
* Fecha de alquiler.

##### En el panel del propietario:
* Cocheras libres u ocupadas.
* Histórico de cobros por fecha.





#### Presentación de los Resultados

Las opciones encontradas se organizan en pantalla de dos maneras fáciles de entender:

* Pines en el Mapa: Puntos de ubicación que muestran directamente el costo por hora sobre la zona seleccionada. Al presionar un punto, se abre una vista previa con la foto del garaje.
  
* Tarjetas en Lista: Cuadros ordenados por cercanía o menor precio que resumen la foto de la cochera, la distancia, la tarifa y la calificación del dueño.
  
* Resultados Ordenados: Posibilidad de ordenar la lista por el precio más bajo, la distancia más corta o las mejores opiniones.



#### Avisos y Respuestas del Sistema

La aplicación te orienta en todo momento mientras buscas:

* Sin resultados:  Si no hay lugares libres en la zona elegida, la pantalla te avisa claramente y te sugiere ampliar el radio de búsqueda a calles cercanas.
  
* Carga rápida: Si la señal está lenta, un pequeño ícono visual indica que los datos se están actualizando.
  
* Cambio al instante: Cada vez que activas un filtro (como "Cochera techada"), la lista y el mapa se actualizan inmediatamente sin necesidad de recargar la página.

### 4.2.5. Navigation Systems.

Se busca que el usuario nunca esté a más de tres interacciones de realizar una acción clave, como buscar una plaza disponible, realizar una reserva, calcular tarifas o validar credenciales.

### Navegación Global (Menú superior persistente)
Se implementa mediante una barra de navegación horizontal fija en la parte superior que otorga acceso directo a los módulos principales del sistema:
* **Search:** Búsqueda rápida de estacionamientos disponibles por ubicación o zona.
* **How it works:** Guía explicativa sobre el funcionamiento del sistema de alquiler y uso de plazas.
* **Media & Demos:** Demostraciones visuales y material interactivo de la plataforma.
* **Pricing:** Estructura de tarifas, planes y costos del servicio.
* **Calculator:** Herramienta interactiva para proyectar o estimar costos de estacionamiento.
* **Verification:** Módulo para la validación de identidad, vehículos o permisos.
* **Selector de Idioma (EN / ES):** Cambio inmediato de interfaz entre inglés y español.
* **Acceso de Usuario (Log In / Register Now):** Botones directos para la autenticación e inicio de sesión.

Esta estructura asegura una navegación clara y accesible desde cualquier sección del sitio.

---

### Navegación de Contexto (Breadcrumbs / Rutas)
Permite al usuario ubicarse dentro del flujo de la plataforma mediante rutas jerárquicas como:
* `Search` > `Lima Centro` > `Estacionamiento A` > `Reservar`
* `Calculator` > `Tarifa Nocturna` > `Estimación de Costo`
* `Verification` > `Documentación` > `Validación de Vehículo`

Esto facilita la orientación del usuario respecto a su posición actual en la aplicación.

---

### Navegación Local
Dentro de cada módulo se organizan las funcionalidades específicas mediante pestañas o secciones internas:
* **En la ficha de un estacionamiento:** Detalles de la plaza, Disponibilidad en tiempo real, Tarifas por hora/día, Reseñas.
* **En el perfil de usuario:** Historial de reservas, Métodos de pago, Vehículos registrados, Alertas.

Esto evita la saturación visual al categorizar la información relevante.

---

### Acciones Rápidas
Se integran botones de llamada a la acción (CTA) destacados para optimizar los flujos más frecuentes:
* **Register Now:** Botón principal para el registro inmediato de nuevos usuarios.
* **Log In:** Acceso directo a la cuenta personal.
* **Buscar / Reservar:** Botones directos dentro de los resultados para completar la reserva en pocos pasos.

---

### Navegación Adaptativa (Responsive)
La barra de navegación ajusta su distribución según la pantalla (desktop, tablet, móvil). En dispositivos móviles, los enlaces centrales se colapsan en un menú desplegable (hamburguesa), manteniendo los botones clave de acceso rápido para priorizar la usabilidad en pantallas pequeñas.


### 4.3. Landing Page UI Design.

### 4.3.1. Landing Page Wireframe.
**4.3.1 Landing Page Wireframe**

La *landing page* de Proyect-Park-Share presenta una estructura clara y orientada a la conversión, iniciando con una sección principal (*Hero Section*) que introduce la solución para la reserva de estacionamientos seguros y el alquiler de cocheras privadas en Lima, resaltando beneficios como el ahorro de tiempo, la transparencia en tarifas y la conexión con propietarios verificados[cite: 5].

### Estructura y Secciones del Wireframe

* **Header / Navigation Bar:**
  * **Branding:** Identificador visual y nombre del proyecto (*Proyect-Park-Share*).
  * **Menú Principal:** Enlaces de acceso rápido a los módulos principales (*Search*, *How it works*, *Media & Demos*, *Pricing*, *Calculator*, *Verification*).
  * **Herramientas y Accesos:** Selector de idioma (*EN / ES*) y botones directos para inicio de sesión (*Log In*) y registro (*Register Now*).

* **Hero Section (Búsqueda Inicial y Propuesta de Valor):**
  * Mensaje principal enfocado en encontrar parqueo seguro o monetizar cocheras privadas.
  * Selector de rol para la interfaz (*I'm a Driver* / *I'm a Parking Owner*).
  * Botones de llamada a la acción (*Book Now*, *Learn More*).
  * **Quick Garage Finder:** Formulario flotante para filtrar búsqueda por distrito/avenida, tipo de vehículo y tarifa máxima por hora.

* **Available Parking Spaces Nearby (Búsqueda en Tiempo Real):**
  * Listado de tarjetas de cocheras con precio por hora, dirección, atributos (*24/7 Surveillance*, *Automatic Gate*, *Compact Auto*) y calificación de usuarios.
  * Mapa dinámico e interactivo adjunto que muestra los marcadores de geolocalización y precios en tiempo real.

* **Platform Video Demonstrations & Case Studies (Media & Demos):**
  * Reproductores de video integrados con casos de estudio y demostraciones técnicas: *About the Team* (proceso de desarrollo y visión urbana) y *ParkShare Platform* (presentación oficial y validación de necesidades).

* **Transparent Pricing & Flexible Plans (Pricing):**
  * Comparativa de planes según el tipo de usuario:
    * **Pay As You Go (S/. 5.00/hr avg):** Para conductores ocasionales.
    * **Driver Pass (S/. 29.90/month):** Opción destacada con descuentos en tarifa horaria y cola de reserva prioritaria.
    * **Garage Owner (0% monthly fee):** Publicación gratuita y pagos automáticos para propietarios.

* **Simple Step-by-Step Flow (How It Works):**
  * Explicación del ciclo de servicio en cuatro etapas correlativas:
    1. **Requested:** Selección de cochera en el mapa y envío de solicitud.
    2. **Confirmed:** Notificación del propietario y reserva del espacio.
    3. **In Use:** Estacionamiento seguro y temporizador activo durante la estancia.
    4. **Finished:** Confirmación de salida, liberación automática de pago y evaluación mutua.

* **Calculate Your Monthly Earnings as an Owner (Calculator):**
  * Widget interactivo que permite a los propietarios estimar sus ingresos mensuales (ej. S/. 1,008.00) ajustando variables como horas disponibles al día y tarifa por hora.

* **Trust & Document Verification (Verification):**
  * Módulo enfocado en la seguridad y validación de la comunidad con opción para subir documentación (*Upload Document*):
    * **National ID / DNI:** Verificación de identidad de conductores y propietarios.
    * **Driver's License & Plate:** Confirmación de licencia autorizada y placa vehicular.
    * **Property Title or Utility Bill:** Validación de legitimidad de la propiedad o cochera.

* **Frequently Asked Questions (FAQ):**
  * Acordeón interactivo con preguntas frecuentes sobre el cálculo de tarifas, límites de tamaño vehicular y métodos de pago a propietarios.

* **Footer:**
  * Pie de página con el logo, declaración del servicio, enlaces de navegación, módulos del usuario, políticas legales/privacidad y derechos de autor.

  <div style="text-align:center;"><img src="../assets/landing-page/Landing-page-wireframe1.png" alt="texto"></div>
  <div style="text-align:center;"><img src="../assets/landing-page/Landing-page-wireframe2.png" alt="texto"></div>
  <div style="text-align:center;"><img src="../assets/landing-page/Landing-page-wireframe3.png" alt="texto"></div>
  <div style="text-align:center;"><img src="../assets/landing-page/Landing-page-wireframe4.png" alt="texto"></div>

### 4.3.2. Landing Page Mock-up.

El wireframe de la landing page en su versión de escritorio ha permitido organizar de forma clara y jerárquica los elementos principales de Proyect-Park-Share, facilitando la presentación de la propuesta de valor centrada en la búsqueda de estacionamientos seguros y la monetización de cocheras privadas en Lima. A partir de esta estructura inicial, se desarrolló el mockup de la interfaz, manteniendo coherencia con las funcionalidades definidas, como la localización en tiempo real con mapa interactivo, la simulación de ganancias, la verificación de documentos y el flujo estructurado de reserva.

En la implementación final se puede apreciar el uso consistente de una paleta de colores basada en tonos azul marino y blanco con acentos verdes para botones clave, así como una tipografía moderna seleccionada, lo que contribuye a una estética limpia y tecnológica. Además, la distribución de secciones como el explorador de parqueos cercanos (*Quick Garage Finder*), los planes flexibles, las demostraciones en video y la guía paso a paso refuerzan la claridad y usabilidad de la plataforma. En conjunto, el diseño refleja una identidad visual alineada con los valores de seguridad, claridad y eficiencia operacional, transmitiendo confianza tanto para conductores como para propietarios de cocheras

<div style="text-align:center;"><img src="../assets/landing-page/Landing-page-mockup1.png" alt="texto"></div>
<div style="text-align:center;"><img src="../assets/landing-page/Landing-page-mockup2.png" alt="texto"></div>
<div style="text-align:center;"><img src="../assets/landing-page/Landing-page-mockup3.png" alt="texto"></div>
<div style="text-align:center;"><img src="../assets/landing-page/Landing-page-mockup4.png" alt="texto"></div>

### 4.4. Web Applications UX/UI Design.
### 4.4.1. Web Applications Wireframes.
### 4.4.2. Web Applications Wireflow Diagrams.
### 4.4.2. Web Applications Mock-ups.
### 4.4.3. Web Applications User Flow Diagrams.
### 4.5. Web Applications Prototyping.
### 4.6. Domain-Driven Software Architecture.
### 4.6.1. Design-Level Event Storming.
### 4.6.2. Software Architecture Context Diagram.
### 4.6.3. Software Architecture Container Diagrams.
### 4.6.4. Software Architecture Components Diagrams.
### 4.7. Software Object-Oriented Design.
### 4.7.1. Class Diagrams.
### 4.8. Database Design.
### 4.8.1. Database Diagrams.