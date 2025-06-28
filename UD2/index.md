---
layout: default
title: Curso de Gestión Empresarial
---


<div style="border: 2px solid #4CAF50; padding: 15px; border-radius: 10px; background-color: #f9fff9;">
  <h3>Unidades Didácticas</h3>
  <ul>
    <li>👉 <a href="../UD1/">UD1. Introducción a la gestión empresarial</a></li>
    <li>👉 <a href="../UD2/">UD2. Instalación y configuración de un ERP-CRM</a></li>
    <li>👉 <a href="../UD3/">UD3. Implantación y uso de sistemas ERP-CRM</a></li>
    <li>👉 <a href="../UD4/">UD4. Personalización y Adaptación Empresarial</a></li>
    <li>👉 <a href="../UD5/">UD5. Desarrollo de Componentes</a></li>
  </ul>
</div>


**UNIDAD 2**

**Instalación y configuración de un ERP-CRM**

**2º DAM**

**Índice**

[1\. Identificación de los diferentes tipos de licencia en Odoo 3](#_Toc202001685)

[1.1. Odoo Community 3](#_Toc202001686)

[1.2. Odoo Enterprise 4](#_Toc202001687)

[2\. Identificación Detallada de los Módulos ERP-CRM en Odoo 18 6](#_Toc202001688)

[2.1. Módulos ERP (Enterprise Resource Planning) 6](#_Toc202001689)

[2.2. Módulos CRM (Customer Relationship Management) 8](#_Toc202001690)

[3\. Realización de Instalaciones con Docker 10](#_Toc202001691)

[3.1 Instalación de Odoo 18 Community con Docker Compose en Windows 10](#_Toc202001692)

[4\. Configuración de los Módulos Instalados en Odoo 18 15](#_Toc202001693)

[4.1. Acceso y Activación del Modo Desarrollador 15](#_Toc202001694)

[4.2. Instalación de Módulos (Aplicaciones) 15](#_Toc202001695)

[4.3. Configuraciones Básicas y esenciales por módulo 16](#_Toc202001696)

[5\. Realización de instalaciones adaptadas a las necesidades planteadas en diferentes supuestos 18](#_Toc202001697)

[5.1. Identificación y Análisis de Requerimientos 20](#_Toc202001698)

[5.2. Ejemplos Prácticos de Adaptaciones 20](#_Toc202001699)

[6\. Verificación del Funcionamiento del ERP-CRM 23](#_Toc202001700)

[6.1. Estrategia de Pruebas 24](#_Toc202001701)

[7\. Documentación de las operaciones realizadas y las incidencias 25](#_Toc202001702)

[7.1. Estructura General de la Documentación 25](#_Toc202001703)

[7.2. Justificación de la Licencia Elegida 25](#_Toc202001704)

[7.3. Infraestructura y Diagrama de Despliegue con Docker 25](#_Toc202001705)

[7.4. Pasos Detallados de Instalación con Docker 26](#_Toc202001706)

[7.5. Configuración Específica de los Módulos Instalados 26](#_Toc202001707)

[7.6. Implementación de Instalaciones Adaptadas (Casos de Estudio) 26](#_Toc202001708)

[7.7. Verificación Funcional del ERP-CRM (Pruebas Funcionales) 27](#_Toc202001709)

[7.8. Gestión de Incidencias y Lecciones Aprendidas 27](#_Toc202001710)

[7.9. Conclusiones y Recomendaciones 27](#_Toc202001711)

# Identificación de los diferentes tipos de licencia en Odoo

Antes de implantar un sistema ERP-CRM como Odoo, es fundamental conocer los distintos tipos de licencia de software que pueden afectar a su uso, distribución, modificación y mantenimiento. Comprender estas licencias permite tomar decisiones informadas sobre la implementación, especialmente en entornos empresariales donde el cumplimiento legal y técnico es clave. La elección de la licencia correcta en Odoo es una decisión estratégica que impacta en:

- Costos de implementación y escalabilidad.
- Flexibilidad para personalizaciones.
- Obligaciones legales y cumplimiento de licenciamiento.
- Soporte técnico y mantenimiento a largo plazo.

## Odoo Community

Esta es la **versión de código abierto de Odoo**, completamente **gratuita** y distribuida bajo la **licencia LGPLv3**. Su desarrollo y mantenimiento son impulsados activamente por la amplia y colaborativa **comunidad global de Odoo**, que incluye desarrolladores, usuarios finales y socios de todo el mundo. Esto garantiza su constante evolución, la adición de nuevas funcionalidades y la corrección de errores, beneficiándose de una auditoría colectiva y una mejora continua.

Odoo Community ofrece un conjunto robusto de módulos esenciales para la gestión empresarial. Incluye funcionalidades completas de **CRM (Gestión de Relaciones con el Cliente)** para la administración de oportunidades, clientes potenciales y actividades de venta. En el ámbito **ERP**, cubre módulos cruciales como **Ventas** (presupuestos, pedidos, facturación), **Inventario** (gestión de almacenes, movimientos de stock), **Compras** (órdenes de compra, gestión de proveedores), **Contabilidad básica** (facturación, asientos contables), **Fabricación (MRP básico)**, **Proyectos**, **Recursos Humanos** (gestión de empleados), y **Sitio Web** (creación de páginas web y blogs).

- **Ventajas:**
  - **Costo Cero de Licencia:** Es ideal para startups, pequeñas y medianas empresas con presupuestos limitados, y, crucialmente, para **propósitos académicos y de formación**.
  - **Flexibilidad y Personalización:** Al ser de código abierto, permite a los desarrolladores y usuarios avanzados modificar el código fuente y crear módulos personalizados para satisfacer necesidades muy específicas.
  - **Comunidad Activa:** Existe una vasta comunidad de usuarios y desarrolladores que proporcionan soporte, comparten conocimientos y desarrollan módulos adicionales.
- **Limitaciones:**
  - **Funcionalidades Avanzadas:** Ciertos módulos avanzados (como MRP avanzado, VOIP, servicios de campo, calidad, etc.) y características de usabilidad (como Odoo Studio) no están disponibles.
  - **Soporte Oficial:** No incluye soporte técnico directo de Odoo S.A. Las actualizaciones y correcciones deben gestionarse manualmente o a través de la comunidad.
  - **Escalabilidad en la Nube:** No incluye los servicios de alojamiento en la nube de Odoo Online o el portal de cliente premium.

Odoo Community es una **solución potente y gratuita** para gestión empresarial básica, pero **requiere autogestión y conocimientos técnicos**. Si necesitas **módulos avanzados, soporte oficial o escalabilidad en la nube**, Odoo Enterprise (versión de pago) puede ser más adecuado.

## Odoo Enterprise

Esta es la versión de pago y comercial de Odoo, diseñada específicamente para empresas que demandan funcionalidades más avanzadas, un nivel superior de soporte y una gama de servicios adicionales que no están disponibles en la edición Community. Opera bajo un **modelo de suscripción**, donde el costo suele depender del número de usuarios activos, el tipo de alojamiento elegido y, en menor medida actualmente, las aplicaciones activadas.

A diferencia de la versión Community que es totalmente gratuita en cuanto a licencia, Odoo Enterprise implica una inversión recurrente. Específicamente, para la opción de alojamiento Odoo Online (SaaS), los costes base pueden oscilar, por ejemplo, entre **300 y 600 €** al mes para un **escenario de uso típico** en una pequeña o mediana empresa. Es crucial destacar que, desde Odoo 16 (y Odoo 18 mantiene esta política), el coste por usuario ya incluye el acceso a la mayoría de las aplicaciones Enterprise, lo que simplifica enormemente la estructura de precios y evita que el costo se dispare por añadir cada módulo individualmente, como ocurría en versiones anteriores. Sin embargo, para una estimación completa, siempre se deben considerar otros factores adicionales.

Además de todas las características de Odoo Community, Enterprise incorpora:

- - **Módulos Avanzados:** MRP avanzado (planificación detallada, gestión de lotes/series), Control de Calidad, Servicio de Campo (FSM), Gestión de Flotas, VOIP, etc.
    - **Odoo Studio:** Una herramienta visual que permite a los usuarios personalizar interfaces, crear nuevos objetos y automatizaciones sin necesidad de programación.
    - **Portal del Cliente Mejorado:** Funcionalidades avanzadas para la interacción con clientes y partners.
    - **Integraciones Nativas:** Con ciertas plataformas y servicios de pago.
- **Ventajas:**
  - **Soporte Oficial:** Acceso a soporte técnico directo de Odoo S.A., lo que es crucial para empresas con operaciones críticas.
  - **Actualizaciones Automáticas:** Garantiza que el sistema esté siempre al día con las últimas características y parches de seguridad.
  - **Alojamiento en la Nube (Odoo Online):** Opción de despliegue gestionado por Odoo en sus servidores, eliminando la necesidad de gestionar la infraestructura.
  - **Características Premium:** Acceso a módulos y herramientas que mejoran la eficiencia y la personalización sin código.
- **Desventajas:**
  - **Costo:** Implica una suscripción mensual o anual por usuario y/o por aplicación.
  - **Menos Flexibilidad en el Código:** Aunque se puede acceder al código fuente, la licencia es más restrictiva en cuanto a su distribución y modificación con fines comerciales fuera del modelo de suscripción.

Para esta unidad didactica, la **elección ideal es Odoo Community**. Esta versión proporciona todas las funcionalidades esenciales de ERP y CRM necesarias para comprender la estructura modular, realizar instalaciones, configurar procesos clave y verificar el funcionamiento. Dado que el objetivo es la comprensión conceptual y la aplicación práctica de los principios de implantación, y no la gestión de un entorno productivo de gran escala con requerimientos específicos de soporte, Odoo Community es la opción más accesible, flexible y económicamente viable. Además, el uso de Docker facilita enormemente la gestión de esta versión de código abierto.

# Identificación Detallada de los Módulos ERP-CRM en Odoo 18

Odoo 18 se caracteriza por una arquitectura modular que permite a cada aplicación (módulo) enfocarse en una función específica, mientras todas se integran formando un sistema cohesivo y eficiente. En este apartado, detallamos los módulos esenciales que constituyen los entornos ERP y CRM, los cuales serán el núcleo de tus prácticas.

## 2.1. Módulos ERP (Enterprise Resource Planning)

Estos módulos permiten gestionar de forma integral los recursos internos, optimizando operaciones financieras, logísticas y productivas dentro de la empresa.

**Inventario**

- **Funcionalidad principal:** Gestión completa del stock y almacenes.
- **Características:** Control detallado de ubicaciones (internas, clientes, proveedores), movimientos de mercancías (recepciones, entregas, transferencias internas), reglas automatizadas de reposición, trazabilidad completa por lotes o números de serie, valoración precisa del inventario.
- **Relevancia:** Imprescindible para entender cómo las operaciones logísticas se integran con ventas y compras.

**Compras**

- **Funcionalidad principal:** Optimización del proceso de adquisición de bienes y servicios.
- **Características:** Solicitudes de cotización, órdenes de compra, recepción y control de mercancías, gestión de proveedores y análisis comparativo de precios.
- **Relevancia:** Ejemplifica la cadena completa de suministro, con integración directa con inventario y contabilidad.

**Contabilidad (Invoicing/Accounting)**

- **Funcionalidad principal:** Control financiero integral y gestión contable precisa.
- **Características:** Emisión y registro de facturas a clientes y proveedores, seguimiento de pagos, gestión de diarios contables, configuración del plan contable e impuestos, conciliación bancaria e informes financieros detallados (balance, pérdidas y ganancias, flujo de caja).
- **Relevancia:** Centro neurálgico para la administración financiera. Configurarás aspectos clave como impuestos, diarios y el plan contable según normativa española.

**Fabricación (MRP - Manufacturing Resource Planning)**

- **Funcionalidad principal:** Gestión completa de procesos productivos y fabricación.
- **Características:** Creación y control de órdenes de fabricación, gestión avanzada de listas de materiales (BOM), rutas de producción, centros de trabajo y control operativo de procesos.
- **Relevancia:** Permite entender la transformación efectiva de materias primas en productos finales con total visibilidad.

**Recursos Humanos (RRHH)**

- **Funcionalidad principal:** Administración eficaz del personal.
- **Características:** Base de datos de empleados, control de ausencias (vacaciones, bajas), gestión de gastos, organigrama empresarial y contratos.
- **Relevancia:** Muestra la extensión de Odoo hacia la gestión integral del talento humano dentro de las empresas.

**Proyectos**

- **Funcionalidad principal:** Gestión y seguimiento detallado de proyectos empresariales.
- **Características:** Creación de proyectos, asignación eficiente de tareas y subtareas, monitoreo del progreso, registro preciso de horas trabajadas y planificación de recursos.
- **Relevancia:** Ideal para empresas orientadas a proyectos internos o externos.

**Sitio Web**

- **Funcionalidad principal:** Desarrollo rápido y gestión dinámica de sitios web.
- **Características:** Editor visual sencillo de usar, creación de blogs y páginas informativas, formularios integrados y gestión completa del contenido web.
- **Relevancia:** Complementa CRM captando leads desde la web y potenciando la presencia digital.

**Comercio Electrónico**

- **Funcionalidad principal:** Plataforma integral de ventas online.
- **Características:** Gestión completa de la tienda virtual, carrito de compras, pagos electrónicos, gestión y seguimiento de pedidos en tiempo real.
- **Relevancia:** Ejemplifica claramente cómo Odoo integra verticalmente el comercio electrónico con ventas, inventario y contabilidad.

### Interconexión y flujos

Durante las prácticas, presta especial atención a cómo los módulos se interconectan creando flujos operativos continuos. Por ejemplo, un lead en CRM puede evolucionar a presupuesto en Ventas, y al confirmarse afectar directamente al Inventario y Contabilidad. Este enfoque global es crucial para comprender plenamente un sistema ERP-CRM integrado

## 2.2. Módulos CRM (Customer Relationship Management)

Estos módulos permiten gestionar las interacciones con clientes y potenciales clientes, desde el contacto inicial hasta la atención post-venta, asegurando una relación fluida y eficiente.

**CRM (Gestión de Relaciones con el Cliente)**

- **Funcionalidad principal:** Gestiona de manera integral todo el ciclo de ventas.
- **Características:** Captura y cualificación de leads, conversión en oportunidades comerciales, gestión del pipeline de ventas con etapas personalizables (nuevo, calificado, propuesta, negociación, ganado/perdido), asignación de oportunidades a equipos comerciales, registro de actividades (llamadas, reuniones, tareas), historial de interacciones y pronósticos comerciales.
- **Relevancia:** Permite comprender la gestión desde el primer contacto con clientes potenciales. Deberás configurar etapas y equipos comerciales para simular diferentes escenarios de ventas.

**Ventas**

- **Funcionalidad principal:** Administración completa del ciclo comercial desde presupuestos hasta la facturación.
- **Características:** Generación de cotizaciones, conversión a pedidos con seguimiento exhaustivo, emisión y gestión de facturas (integrado con contabilidad), tarifas personalizables, condiciones de pago y descuentos aplicables.
- **Relevancia:** Su integración con CRM e inventario permite simular con precisión el ciclo comercial integral de una empresa.

**Punto de Venta (POS)**

- **Funcionalidad principal:** Facilita las ventas minoristas en establecimientos físicos.
- **Características:** Interfaz intuitiva para transacciones ágiles, gestión sencilla de productos y pagos (efectivo o tarjeta), gestión de devoluciones y reportes diarios. Funciona incluso en ausencia de conexión, sincronizando posteriormente.
- **Relevancia:** Destaca la flexibilidad y adaptabilidad de Odoo en diversos modelos de negocio minorista.

**Marketing (Automation, Email Marketing, SMS Marketing)**

- **Funcionalidad principal:** Gestión efectiva de campañas y automatización de acciones comerciales.
- **Características:** Creación y seguimiento de campañas vía email (newsletters, promociones), automatización basada en comportamiento del cliente, gestión de contactos, monitoreo de efectividad y envío de mensajes SMS.
- **Relevancia:** Demuestra cómo Odoo mejora la captación de clientes potenciales y facilita la fidelización.

# Realización de Instalaciones con Docker

Docker es una plataforma que permite empaquetar una aplicación y sus dependencias en un "contenedor" aislado. Docker Compose, a su vez, facilita la definición y ejecución de aplicaciones multi-contenedor. Esta metodología es altamente recomendada por su simplicidad, portabilidad y consistencia del entorno.

## 3.1 Instalación de Odoo 18 Community con Docker Compose en Windows

Esta guía explica paso a paso cómo instalar Odoo 18 Community utilizando **Docker Compose** en un sistema operativo **Windows**. Esta instalación es **monopuesto**, es decir, todo se ejecutará en el mismo equipo (Odoo + base de datos PostgreSQL), facilitando las pruebas y el aprendizaje del sistema ERP.

### Requisitos previos

Antes de comenzar, asegúrate de tener instalado en tu equipo:

1. Docker Desktop para Windows
2. Editor de texto (Visual Studio Code, Notepad++, etc.)
3. Conexión a internet
4. Opcional: Git (para clonar módulos o trabajar con repositorios)

### 1\. Crear el directorio de trabajo

Crea una carpeta donde guardarás el archivo docker-compose.yml y otros elementos del proyecto.

mkdir C:\\odoo18-docker

cd C:\\odoo18-docker

### 2️. Crear el archivo docker-compose.yml

Este archivo define los **servicios** que se van a utilizar: el servidor de Odoo y la base de datos PostgreSQL.

Crea un archivo llamado docker-compose.yml dentro del directorio creado y pega este contenido:

version: '3'

services:

&nbsp; web:

&nbsp;   image: odoo:18.0

&nbsp;   depends_on:

&nbsp;     - db

&nbsp;   ports:

&nbsp;     - "8069:8069"

&nbsp;   environment:

&nbsp;     - HOST=db

&nbsp;     - USER=odoo

&nbsp;     - PASSWORD=odoo

&nbsp;   volumes:

&nbsp;     - web-data-nombreApellido:/var/lib/odoo

&nbsp;     - ./config:/etc/odoo

&nbsp;     - ./addons:/mnt/extra-addons

&nbsp;     - ./log:/var/log/odoo

&nbsp;   restart: always  # Se asegura que el contenedor de Odoo se reinicie automáticamente

&nbsp; db:

&nbsp;   image: postgres:16

&nbsp;   environment:

&nbsp;     - POSTGRES_USER=odoo

&nbsp;     - POSTGRES_PASSWORD=odoo

&nbsp;     - POSTGRES_DB=postgres

&nbsp;   volumes:

&nbsp;     - db-data-nombreApellido:/var/lib/postgresql/data

&nbsp;   restart: always  # Se asegura que el contenedor de PostgreSQL se reinicie automáticamente

volumes:

&nbsp; web-data-nombreApellido:

&nbsp; db-data-nombreApellido:

**Explicación de los Servicios: web, db y volumes en Docker Compose para Odoo 18**

### 🖥️ Servicio web (Odoo)

Este servicio ejecuta la aplicación **Odoo**, la interfaz con la que interactúan los usuarios. Es el componente principal del sistema desde el punto de vista del usuario.

- **Imagen oficial odoo:18.0**

El contenedor se basa en la versión 18.0 de la imagen oficial de Odoo, lo que garantiza compatibilidad y estabilidad.

- **Se comunica con el servicio db (PostgreSQL)**

La aplicación Odoo está configurada para conectarse al servicio db, donde guarda y consulta todos los datos.

- **Expone el puerto 8069 para acceso vía navegador**

Permite que accedas a Odoo desde tu navegador web en la dirección: <http://localhost:8069>.

- **Guarda los datos en un volumen y accede a módulos personalizados**
  - Los archivos generados por Odoo (por ejemplo, documentos adjuntos, configuraciones...) se guardan de forma persistente en el volumen web-data-nombreApellido.
  - Además, carga módulos personalizados desde la carpeta addons que tú crees en tu máquina, facilitando el desarrollo y la extensión del sistema.

### 🗃️ Servicio db (PostgreSQL)

Este contenedor ejecuta **PostgreSQL**, el motor de base de datos donde Odoo guarda toda la información estructurada: productos, usuarios, ventas, configuraciones, etc.

- **Imagen oficial postgres:16**
- Utiliza la versión 16 del sistema de base de datos PostgreSQL, ampliamente utilizada y compatible con Odoo.
- **Datos persistentes gracias al volumen db-data-nombreApellido**
- El contenedor guarda toda la información en un volumen externo, garantizando que no se pierdan los datos, aunque el contenedor se detenga, reinicie o actualice.

### 💾 Volúmenes (volumes:)

Los **volúmenes** no son servicios, sino unidades de almacenamiento que permiten **persistir datos** fuera de los contenedores Docker.

- **¿Qué son los volúmenes?**
- Son espacios de almacenamiento gestionados por Docker en tu sistema operativo. Se utilizan para evitar la pérdida de datos cuando un contenedor se elimina o reinicia.
- **¿Cómo funcionan?**
  - Se “montan” en rutas específicas dentro de los contenedores.
  - Los datos escritos dentro del contenedor en esas rutas se guardan realmente en el sistema de archivos del host.
  - Esto permite mantener la información (como configuraciones o bases de datos) de forma segura y duradera.
- **En este proyecto se definen dos volúmenes:**
  - web-data-nombreApellido: Guarda los datos del contenedor Odoo: módulos instalados, configuraciones, documentos adjuntos, etc.
  - db-data-nombreApellido: Guarda todos los datos de PostgreSQL: tablas, registros y estructuras de la base de datos.

### 3\. Crear carpeta para módulos personalizados (opcional)

En el mismo directorio del proyecto, crea una subcarpeta llamada addons:

mkdir C:\\odoo18-docker\\addons

Aquí podrás añadir módulos propios o descargados de terceros.

### 4\. Iniciar Odoo con Docker Compose

Abre una terminal (PowerShell o CMD), navega hasta la carpeta del proyecto y ejecuta:

docker compose up -d

Esto:

- Descargará las imágenes de Odoo y PostgreSQL si no están instaladas.
- Creará y ejecutará los contenedores en segundo plano.
- Montará los volúmenes persistentes.

📋 Comandos útiles:

- Ver contenedores activos:

docker compose ps

- Ver logs:

docker compose logs -f

- Detener los contenedores:

docker compose down

### 5\. Acceder a Odoo desde el navegador

Abre tu navegador y entra en:

<http://localhost:8069>

Verás la pantalla de creación de la base de datos.

### 👤 Configuración inicial

- **Master Password**: contraseña general de administración (puedes definir una).
- **Database Name**: elige un nombre (por ejemplo: mi_empresa).
- **Email**: <admin@example.com>
- **Password**: define la contraseña del usuario administrador de Odoo.
- **Demo Data**: marca la casilla si quieres cargar datos de ejemplo (recomendado para aprender).
- **Language, Country**: selecciona tus preferencias.

Haz clic en **“Create database”** para terminar.

# Configuración de los Módulos Instalados en Odoo 18

Una vez que Odoo está en funcionamiento y has creado tu base de datos, la siguiente fase crítica es la configuración de los módulos para adaptarlos a las necesidades de la empresa simulada. Este proceso es donde el ERP-CRM empieza a tomar forma para un uso práctico.

## 4.1. Acceso y Activación del Modo Desarrollador

1. **Inicia Sesión en Odoo:** Accede a tu instancia de Odoo (ej., <http://localhost:8069>) con el usuario admin y la contraseña que estableciste al crear la base de datos.
2. **Activa el Modo Desarrollador (Developer Mode):** Esta es una herramienta esencial para acceder a funcionalidades avanzadas de configuración y personalización que no son visibles en el modo de usuario normal.
    - Ve a **Ajustes** (el icono del engranaje en la barra superior o en el menú principal).
    - Desplázate hasta el final de la página y haz clic en el enlace **"Activar el modo desarrollador"** (o "Activate the developer mode" si Odoo está en inglés).
    - Verás un pequeño icono de un bicho (🐞) en la parte superior derecha, junto a tu nombre de usuario, indicando que el modo desarrollador está activo.

## 4.2. Instalación de Módulos (Aplicaciones)

1. **Navega a "Aplicaciones":** En el menú principal de Odoo, haz clic en **"Aplicaciones"** (o "Apps").
2. **Explora y Busca Módulos:** Aquí verás una lista de todos los módulos disponibles. Puedes usar la barra de búsqueda para encontrar módulos específicos.
3. **Instala los módulos clave para ERP-CRM:**
    - CRM: Busca "CRM" y haz clic en "Instalar". Este es el punto de partida para la gestión de clientes y oportunidades.
    - Ventas: Busca "Ventas" (o "Sales") y haz clic en "Instalar". Este módulo es fundamental y se integra directamente con CRM e Inventario.
    - Inventario: Busca "Inventario" (o "Inventory") y haz clic en "Instalar". Es esencial para la gestión de productos y almacenes.
    - Compras: Busca "Compras" (o "Purchase") y haz clic en "Instalar". Para la gestión de proveedores y adquisiciones.
    - Contabilidad: Busca "Facturación" (o "Invoicing", que es el módulo base de contabilidad) y/o "Contabilidad" (o "Accounting" si está disponible con tu localización) y haz clic en "Instalar". Este es crucial para la gestión financiera.
    - Otros módulos según el supuesto: Si el caso de estudio lo requiere, instala "Punto de Venta", "Fabricación", "Recursos Humanos", "Proyectos", "Sitio Web", "Comercio Electrónico", etc. Odoo se encargará de instalar automáticamente las dependencias necesarias.

## 4.3. Configuraciones Básicas y esenciales por módulo

Una vez que Odoo está instalado y tienes acceso a tu base de datos el primer paso crucial para adaptar el sistema a una empresa real es configurar los ajustes generales. Esto establece las bases para todas las operaciones futuras y garantiza que la información esencial de tu compañía esté correctamente reflejada en el ERP.

##### 4.3.1. Configuración General del Sistema (Ajustes)

- **Información de la Compañía:**
  - Ve a Ajustes > Usuarios y Compañías > Compañías.
  - Selecciona tu compañía y rellena la información básica: Nombre, Dirección, NIF/CIF, Logo, Moneda (por defecto Odoo usará Euros si la localización es española). Esto aparecerá en todos los documentos (facturas, presupuestos).
- **Usuarios y Permisos:**
  - Ve a Ajustes > Usuarios y Compañías > Usuarios.
  - Crea nuevos usuarios para simular roles (ej., Comercial, Contable, Responsable de Inventario).
  - Asigna los derechos de acceso adecuados a cada usuario. Por ejemplo, a un "Comercial" le darías permisos de "Usuario" en CRM y Ventas, pero de "Ver" o "Ninguno" en Contabilidad. A un "Contable" le darías "Asesor" en Contabilidad. Esto es fundamental para la seguridad y el control interno.
- **Idiomas:**
  - Si Odoo no está en español, ve a Ajustes > Traducciones > Cargar un idioma. Busca "Español (es_ES)" y haz clic en "Cargar". Luego, puedes cambiar el idioma por defecto de la compañía o de cada usuario individualmente.
- **Diseño de Documentos:**
  - En Ajustes > General > Diseño de Documentos, puedes personalizar la apariencia de tus presupuestos, pedidos, y facturas (colores, fuentes, información de la compañía).

##### 4.3.2. Configuración Específica de Módulos

- **Módulo CRM:**
  - Equipos de Venta: Ve a CRM > Configuración > Equipos de Venta. Define diferentes equipos (ej., Ventas Online, Ventas Telefónicas, Grandes Cuentas) y asigna comerciales a cada uno.
  - Etapas de Oportunidad: Ve a CRM > Configuración > Etapas. Modifica o crea nuevas etapas del pipeline de ventas para adaptarlas al proceso de tu empresa (ej., Contacto Inicial, Calificación, Presentación de Propuesta, Negociación, Cerrada Ganada, Cerrada Perdida).
  - Actividades: Odoo viene con tipos de actividad predefinidos (llamada, reunión, email). Puedes añadir más si es necesario.
- **Módulo Ventas:**
  - Tarifas de Precios: (Si necesitas diferentes precios para diferentes clientes o volúmenes). Ve a Ventas > Configuración > Tarifas de precios.
  - Términos de Pago: (Se configura en Contabilidad, pero afecta a Ventas). Ve a Contabilidad > Configuración > Términos de pago. Define "Pago Inmediato", "Neto 30 días", etc.
  - Ajustes de Impuestos y Monedas: Asegúrate de que los impuestos configurados en Contabilidad se apliquen correctamente en los productos y las ventas.
- **Módulo Inventario:**
  - Ubicaciones: Ve a Inventario > Configuración > Ubicaciones. Odoo crea un almacén por defecto. Puedes definir ubicaciones más específicas dentro de ese almacén (ej., "Stock", "Calidad", "Estante A1").
  - Categorías de Productos: Ve a Inventario > Configuración > Categorías de Productos. Organiza tus productos para una mejor gestión y reporte. Define si se gestiona el inventario por categoría (ej., manual, automático).
  - Reglas de Reabastecimiento: (Opcional, pero muy útil). Ve a Inventario > Productos > Reglas de reabastecimiento. Permite automatizar la creación de órdenes de compra cuando el stock de un producto cae por debajo de un umbral.
- **Módulo Compras:**
  - Términos de Compra: Configura los términos y condiciones predeterminados para las órdenes de compra.
  - Productos y Proveedores: Asegúrate de que los productos tengan proveedores asociados y precios de compra definidos.
- **Módulo Contabilidad (Facturación/Accounting):**
  - Plan Contable: Ve a Contabilidad > Configuración > Plan Contable. Odoo carga un plan contable genérico o específico para la localización española si se ha configurado previamente. Revísalo y adapta las cuentas si es necesario.
  - Diarios: Ve a Contabilidad > Configuración > Diarios. Odoo crea diarios por defecto (Ventas, Compras, Banco, Caja, Varios). Asegúrate de que estén configurados correctamente para los movimientos.
  - Impuestos: Ve a Contabilidad > Configuración > Impuestos. Configura los tipos de IVA (ej., IVA 21%, IVA 10%, IVA 4%) y si son impuestos incluidos en el precio o no.
  - Posiciones Fiscales: (Configuración avanzada para impuestos según el cliente/proveedor/país).
  - Bancos y Cuentas Bancarias: Ve a Contabilidad > Configuración > Bancos. Configura las cuentas bancarias de la empresa.

**Documentación:** Para este punto, es crucial documentar cada decisión de configuración. Por ejemplo, ¿por qué se crearon ciertas etapas de CRM? ¿Qué permisos se asignaron a qué roles? Incluye capturas de pantalla de las pantallas de configuración clave.

# Realización de instalaciones adaptadas a las necesidades planteadas en diferentes supuestos

La verdadera potencia de **Odoo** como solución ERP/CRM no reside únicamente en su funcionalidad estándar, sino en su **capacidad excepcional para adaptarse** a los procesos únicos de cada organización.

Este criterio de evaluación valora precisamente esa habilidad: **transformar una instalación genérica en una herramienta estratégica** que refleje con fidelidad las necesidades específicas del negocio.

### ¿Por qué la personalización es fundamental?

- Ninguna empresa opera exactamente igual que otra.
- Los flujos de trabajo, jerarquías y necesidades de información varían significativamente.
- La personalización es clave para obtener **ventaja competitiva** y eficiencia.

### Herramientas Clave para la Personalización Avanzada en Odoo

#### 1️. Modo Desarrollador (Developer Mode)

- Permite acceder a modelos, vistas, acciones y reglas del sistema.
- Incluye herramientas de diagnóstico integradas.
- Facilita la creación y edición de campos personalizados desde la interfaz.
- Permite el registro y la auditoría de cambios técnicos.

#### 2️. Desarrollo de Módulos Personalizados

- Estructura modular basada en tecnologías estándar (Python y XML).
- Permite extender o modificar funcionalidades existentes.
- Compatible con actualizaciones progresivas sin afectar el núcleo.
- Favorece la reutilización, documentación y mantenimiento del sistema.

#### 3️. Técnicas Avanzadas de Adaptación

- Automatizaciones y tareas programadas que optimizan procesos.
- Modelado de flujos de trabajo específicos según necesidades del negocio.
- Personalización de informes y paneles de control.
- Integración con servicios externos y otras aplicaciones empresariales.

## 5.1. Identificación y Análisis de Requerimientos

Antes de cualquier adaptación, es fundamental entender el "supuesto" o caso de negocio y desglosar sus necesidades.

- **Ejemplo de supuesto:** "Una pequeña empresa de servicios de consultoría necesita gestionar sus proyectos, facturar por horas trabajadas y llevar un registro de sus clientes y las oportunidades de negocio."
- **Análisis de módulos necesarios:** CRM, Ventas, Proyectos, Contabilidad.
- **Análisis de personalizaciones:**
  - Necesidad de campos específicos en clientes o proyectos.
  - Automatizaciones para el flujo de trabajo.
  - Reportes personalizados (ej., reporte de horas por proyecto).
  - Posiblemente módulos de terceros (ej., para una integración específica de facturación electrónica si fuera el caso).

## 5.2. Ejemplos Prácticos de Adaptaciones

##### 5.2.1. Creación de Campos Personalizados (Usando Modo Desarrollador)

Odoo permite añadir campos a cualquier modelo (ej., Cliente, Producto, Oportunidad) sin escribir código, directamente desde la interfaz de usuario en modo desarrollador.

1. **Activar Modo Desarrollador:** Asegúrate de que el modo desarrollador esté activo (🐞).
2. **Identificar el Modelo:** Navega al formulario donde necesitas el nuevo campo (ej., un contacto en Contactos para añadir un "Código de Cliente Externo").
3. **Abrir el Inspector:** Haz clic en el icono del bicho (🐞) y selecciona "Editar Vista" o "Ver Campos" (dependiendo de dónde quieras añadirlo y si ya existe). Alternativamente, pasa el ratón sobre un campo existente y haz clic en el icono del bicho que aparece, luego selecciona "Ver Campos".
4. **Añadir un Nuevo Campo:**
    - En la ventana de información técnica que se abre, selecciona el modelo al que deseas añadir el campo (ej., res.partner para contactos).
    - Haz clic en **"Añadir Campo Nuevo"**.
    - Rellena los detalles:
        - Etiqueta de Campo: El nombre visible para el usuario (ej., "Código de Cliente Externo").
        - Nombre de Campo: Un nombre técnico único (ej., x_codigo_cliente_externo). Odoo añade x_ a los campos personalizados.
        - Tipo de Campo: Texto, Numérico, Booleano, Fecha, Selección, Relacional (Many2one, One2many, Many2many), etc.
        - Otros atributos: Requerido, Solo lectura, Default, etc.
    - Haz clic en "Guardar".
5. **Añadir el Campo a la Vista:**
    - Vuelve al formulario donde querías añadirlo.
    - Haz clic en el icono del bicho y selecciona "Editar Vista (Formulario)".
    - En el editor XML de la vista, busca la ubicación donde quieres que aparezca el campo y añade la línea: &lt;field name="x_codigo_cliente_externo"/&gt;. (Si no te sientes cómodo con XML, a veces Odoo Studio en Enterprise lo simplifica. En Community, el editor XML es la forma más directa).
    - Haz clic en "Guardar".
    - Recarga la página para ver el nuevo campo.

##### 5.2.2. Instalación de Módulos de Terceros o Personalizados

Si las funcionalidades estándar no son suficientes, la comunidad de Odoo ofrece una gran cantidad de módulos adicionales.

1. **Obtener el Módulo:**
    - Descarga el módulo desde la Odoo App Store (<https://apps.odoo.com>) o un repositorio de GitHub. Los módulos suelen venir en formato ZIP o como un directorio.
2. **Colocar el Módulo en la Carpeta addons:**
    - Descomprime el archivo ZIP (si es el caso) y coloca el directorio del módulo (ej., mi_modulo_facturacion) dentro de la carpeta ~/odoo18-docker/addons que creaste en la sección de instalación.
    - Asegúrate de que la estructura sea ~/odoo18-docker/addons/mi_modulo_facturacion/, y que dentro de mi_modulo_facturacion esté el archivo \__manifest_\_.py.
3. **Actualizar la Lista de Aplicaciones en Odoo:**
    - En Odoo (con el modo desarrollador activo), ve a Aplicaciones.
    - Haz clic en "Actualizar lista de aplicaciones". Odoo escaneará la carpeta addons y detectará el nuevo módulo.
4. **Instalar el Módulo:**
    - Busca el nombre de tu nuevo módulo en la lista de aplicaciones y haz clic en "Instalar".

##### 5.2.3. Automatizaciones de Acciones (Flujos de Trabajo Sin Código)

Odoo permite crear reglas automatizadas que disparan acciones cuando se cumplen ciertas condiciones. Esto es muy potente para implementar lógicas de negocio.

1. **Activar Modo Desarrollador:** Asegúrate de que el modo desarrollador esté activo (🐞).
2. **Navegar a Acciones Automatizadas:** Ve a **Ajustes > Técnico > Automatización > Acciones Automatizadas**.
3. **Crear una Nueva Acción Automatizada:**
    - Haz clic en **"Crear"**.
    - Modelo: Selecciona el modelo sobre el cual se aplicará la automatización (ej., Oportunidad si quieres automatizar algo en el pipeline de ventas).
    - Disparador: Define cuándo se activará la acción (ej., "Al crear", "Al actualizar", "Al eliminar", "En el cron").
    - Condición: Establece los criterios que deben cumplirse para que la acción se ejecute (ej., "Etapa de Oportunidad = Propuesta").
    - Acciones a Realizar:
        - **Actualizar el registro:** Modificar un campo del registro (ej., "Asignar Comercial = \[Nuevo Comercial\]").
        - **Crear un nuevo registro:** Crear una nueva tarea, una nota, etc.
        - **Enviar email:** Enviar un correo electrónico a un contacto o comercial.
        - **Ejecutar código Python:** Para lógicas más complejas (requiere conocimientos de Python).
        - **Actividades:** Programar una actividad (ej., una llamada de seguimiento).
    - Ejemplo: Cuando una "Oportunidad" cambia a la etapa "Ganada", automáticamente envía un correo de felicitación al cliente y crea una tarea de "Preparar Proyecto" para el equipo de Proyectos.

##### 5.2.4. Integraciones Mediante API REST (Concepto)

Aunque la implementación de una API REST va más allá de la configuración sin código, es importante entender que Odoo expone una API robusta para integrarse con otros sistemas (ej., una tienda online externa, un sistema de logística de terceros). Odoo utiliza XML-RPC y JSON-RPC para su API. Permite crear, leer, actualizar y eliminar registros de Odoo desde aplicaciones externas.

**Para este apartado, tu documentación debe ser muy detallada:**

- Descripción del supuesto: Define claramente el escenario de negocio y los problemas a resolver.
- Decisiones de diseño: Explica por qué elegiste ciertas configuraciones o módulos (estándar, personalizado, de terceros).
- Pasos de implementación: Describe detalladamente cómo realizaste las adaptaciones (con capturas de pantalla).
- Resultados esperados: Qué se logró con la adaptación.

# Verificación del Funcionamiento del ERP-CRM

La fase de verificación es, sin lugar a dudas, uno de los **pilares más críticos** en cualquier implementación de un sistema ERP-CRM como Odoo. No se trata solo de comprobar si el sistema se enciende, sino de asegurar exhaustivamente que **Odoo**, en su configuración específica, cumple fielmente con todos los requisitos de negocio del caso de estudio y que cada módulo, tanto individualmente como en su interacción con otros, opera de manera impecable y coherente. Es una simulación controlada y sistemática del uso diario del sistema, diseñada para detectar y corregir cualquier desviación antes de la puesta en marcha real.

## 6.1. Estrategia de Pruebas

Una estrategia de pruebas bien definida es la hoja de ruta indispensable para una verificación exitosa de cualquier sistema ERP-CRM como Odoo. Implica un enfoque metódico y disciplinado para planificar, ejecutar y documentar cada paso, asegurando que el sistema no solo funcione, sino que funcione correctamente para las necesidades de la empresa. La calidad de esta estrategia impacta directamente en la estabilidad, fiabilidad y éxito de la implementación de Odoo.

Aquí detallamos una estrategia de pruebas funcional:

1. **Definición de Casos de Prueba:** Para cada módulo clave y para los flujos inter-módulos, define escenarios de prueba específicos.
2. **Ejecución de Pruebas:** Realiza cada caso de prueba paso a paso.
3. **Registro de Resultados:** Documenta los resultados de cada prueba: si fue exitosa, si hubo incidencias, y cualquier observación.
4. **Validación de Datos:** Verifica que los datos se guardan y se actualizan correctamente.
5. **Pruebas de Integración:** Asegúrate de que los flujos entre módulos (ej., Venta > Inventario > Contabilidad) funcionan sin problemas.
6. **Pruebas de Roles:** Si configuraste diferentes usuarios y permisos, prueba cada caso con los usuarios correspondientes para validar que solo acceden a lo que deben.

Documentación de Verificación: Cada prueba debe ser documentada con:

- **ID del Caso de Prueba:** (ej., TC-CRM-001).
- **Descripción del Caso de Prueba:** Breve explicación de lo que se va a probar.
- **Precondiciones:** Qué debe estar configurado antes de la prueba.
- **Pasos Detallados:** Instrucciones paso a paso.
- **Resultado Esperado:** Cómo debería comportarse el sistema.
- **Resultado Obtenido:** Lo que realmente sucedió.
- **Capturas de Pantalla:** Evidencia visual de los pasos y resultados.
- **Estado:** (Éxito / Fallo / Observación).

# Documentación de las operaciones realizadas y las incidencias

La documentación es una parte fundamental del proceso de implantación. No solo demuestra lo que se ha hecho, sino que también sirve como recurso para futuras referencias, resolución de problemas y formación.

La documentación es un componente crucial en cualquier proceso de implantación ERP-CRM. No solo acredita el trabajo realizado, sino que además actúa como un recurso clave para futuras consultas, resolución ágil de incidencias y formación continua.

## 7.1. Estructura General de la Documentación

Esta sección organiza el manual o informe de tu proyecto:

1. **Portada e Índice:** Datos básicos (título, autor, fecha) y un índice que ayuda a navegar por el documento.
2. **Resumen Ejecutivo:** Un breve resumen del proyecto, sus metas y lo que se logró.
3. **Introducción:** Explica el propósito de este manual, qué abarca el proyecto, una breve descripción de Odoo 18 y cómo se usó Docker.
4. **Análisis de Requerimientos:** Describe el problema de negocio que Odoo resuelve, los procesos clave involucrados y cómo Odoo se adaptó a ellos.

## 7.2. Justificación de la Licencia Elegida

Aquí explicas por qué se usó Odoo Community Edition:

- **Tipo de Licencia:** Confirmar que se eligió Odoo Community Edition.
- **Argumentación:** Explicar las razones de esta elección: es código abierto (gratuito), tiene módulos esenciales, es ideal para aprender o para pequeñas empresas, y evita los costos y la complejidad de la versión Enterprise.

## 7.3. Infraestructura y Diagrama de Despliegue con Docker

Esta sección describe el entorno técnico donde se instaló Odoo:

- **Descripción del Entorno:**
  - Sistema operativo de tu ordenador o servidor.
  - Características del hardware (RAM, procesador, almacenamiento).
  - Versiones de Docker, Docker Compose, Odoo 18 y PostgreSQL que usaste.
  - Detalles de red (direcciones IP, puertos abiertos como 8069).
- **Diagrama de Arquitectura:** Un dibujo claro que muestra visualmente:
  - Tu ordenador (máquina anfitriona).
  - Docker funcionando.
  - Las "cajas" (contenedores) de Odoo y PostgreSQL.
  - Los "espacios de guardado" (volúmenes persistentes).
  - Cómo los usuarios se conectan al sistema.

## 7.4. Pasos Detallados de Instalación con Docker

Aquí documentas cómo se instaló Odoo con Docker:

- **Instalación de Prerrequisitos:** Cómo se instaló Docker y Docker Compose, con ejemplos de lo que se vio en la terminal.
- **Configuración del Directorio de Trabajo:** Pasos exactos para crear la carpeta del proyecto.
- **Archivo docker-compose.yml:** Incluir el contenido completo del archivo, con notas sobre qué hace cada parte.
- **Comandos Esenciales:** Cómo iniciar, detener y manejar los contenedores Docker.
- **Creación Inicial de Base de Datos:** Guía paso a paso, con imágenes, sobre cómo configurar Odoo por primera vez desde el navegador.
- **Configuración de Acceso Remoto (si aplica):** Si permites el acceso desde otros ordenadores, explica cómo configuraste el firewall o un servidor web como NGINX.

## 7.5. Configuración Específica de los Módulos Instalados

Documenta cómo configuraste cada módulo importante de Odoo:

- Para cada módulo (CRM, Ventas, Inventario, Contabilidad), explica:
  - **Propósito del Módulo:** Para qué sirve.
  - **Funcionalidades Configuradas:** Qué opciones específicas activaste (ej., etapas en CRM, tarifas en Ventas, almacenes en Inventario, plan contable en Contabilidad).
  - **Capturas de Pantalla:** Imágenes de las pantallas de configuración relevantes.
  - **Justificación:** Por qué se hicieron esas configuraciones (razones técnicas o de negocio).
- **Configuraciones Generales:** También documenta la configuración inicial de la empresa, la creación de usuarios y roles, y los idiomas.

## 7.6. Implementación de Instalaciones Adaptadas (Casos de Estudio)

Aquí describes cómo personalizaste Odoo para necesidades específicas:

- **Descripción del Caso Específico:** Explica la situación que requirió una adaptación.
- **Requerimientos Especiales:** Detalla qué Odoo estándar no cubría.
- **Soluciones Implementadas:** Cómo se resolvió:
  - Creando **campos personalizados**.
  - Instalando **módulos adicionales o propios**.
  - Configurando **tareas automatizadas**.
  - Explicando cómo se podría **integrar** con otros sistemas.
  - Siempre con capturas de pantalla y el motivo de cada solución.

## 7.7. Verificación Funcional del ERP-CRM (Pruebas Funcionales)

Demuestra que el sistema funciona como se espera:

- **Tabla de Casos de Prueba:** Una tabla que resume cada prueba: qué se probó, cómo se hizo, qué se esperaba, qué pasó y si fue éxito o fallo.
- **Evidencias:** Imágenes claras de las pruebas exitosas.
- **Análisis de Resultados:** Comentarios sobre si Odoo cumple con todos los requisitos.

## 7.8. Gestión de Incidencias y Lecciones Aprendidas

Cómo se manejaron los problemas y qué se aprendió:

- Para cada problema encontrado:
  - **Detalle del Problema:** ID, fecha, descripción, contexto, imágenes/logs.
  - **Análisis y Causa:** Por qué ocurrió.
  - **Solución Aplicada:** Qué se hizo para arreglarlo.
  - **Validación:** Cómo se comprobó que estaba resuelto.
  - **Lecciones Aprendidas:** Qué se aprendió para evitar problemas futuros.

## 7.9. Conclusiones y Recomendaciones

El cierre del proyecto:

- **Síntesis del Proyecto:** Un resumen final de la implantación.
- **Principales Logros:** Qué objetivos se lograron.
- **Retos Superados:** Dificultades y cómo se resolvieron.
- **Conocimientos Adquiridos:** Qué aprendiste (Docker, Odoo, etc.).
- **Recomendaciones Futuras:** Sugerencias para mejorar el sistema o futuras fases.
- **Valor Empresarial Añadido:** Cómo Odoo beneficia a la empresa simulada (más eficiencia, mejor gestión).
