# Capstone Project

Usted es un Ingeniero de Calidad de Software en BAZ y acaba de ser asignado a un nuevo proyecto de automatización. Este proyecto tiene por objetivo que usted ponga en práctica lo aprendido en semanas anteriores acerca de cómo crear un marco de trabajo (framework) de automatización siguiendo guías, patrones de diseño y las mejores prácticas de calidad de la industria.

**El entregable final se compone en su totalidad de las siguientes partes:**

**Proyecto de API**: Un proyecto de API el cual realizará una serie de solicitudes contra la API de Pokemon. 

**Proyecto de Appium**: Un framework que ejecutará una series de escenarios de automatización en móvil sobre la aplicación de  saucedemo. 

**Proyecto de Python**: TBD


**La elección del software a utilizarse será:**
- Python
- Pycharm
- Appium
- Behave

**Las fecha de entrega son las siguientes:**
- **Proyecto de API**: Primer entregable - 17 de Febrero
- **Proyecto de POM en Python**: Segundo entregable - 24 de Febrero
- **Proyecto de Appium**: Tercer entregable - 2 Marzo



# Proyecto de API
El objetivo de este proyecto es poder construir colecciones de Postman, y ordenar adecuadamente las solicitudes “requests” de manera que sigan una serie de acciones que hagan sentido al usuario final. Al evaluar la respuesta de una API permite enfocarse en más puntos que conforman el cuerpo de la respuesta.

**Fecha de entrega: 17 de Febrero de 2023**

**Para este proyecto es importante que se apoye de la documentación disponible en pokemon API para poder realizar lo siguiente:**
- Elija su pokemon favorito (almacenar esta información en un archivo de variables de ambiente) y buscar la información sobre sus movimientos.
- Elija el primer movimiento de la lista, almacene esa información en el archivo de variables de ambiente (nombre, y url).
- Busque toda la información disponible para ese movimiento
- Busque toda la información relacionada para el movimiento seleccionado, validar el nombre del movimiento, y que dentro de la sección “learned_by_pokemon” se muestre el nombre del pokemon favorito seleccionado
- En otro request, realizar una validación similar a la del paso anterior, sin embargo agregar la validación por medio de la url del movimiento.

**Para cada uno de los request, validar lo siguiente:**
- Evaluar los códigos de respuesta (HTTP) según corresponda para cada request.
- Agregar una función de prueba que valide el tiempo de respuesta bajo de 700 ms
- Crear una función para validar el json schema (esto aplica para movimientos - movimiento del punto número 1.
- Usar variables de ambiente durante todo el proceso.
- Hacer uso de la pestaña "Pre-request Script" cuando sea posible crear una variable, y asignarle un valor antes de realizar una petición al servidor.
- Incluir una colección exclusivamente para escenarios negativos, como por ejemplo: consultar la información de un pokemon inexistente, en este caso recuerde evaluar correctamente el mensaje de error (HTTP Status Code, y el mensaje de error asociado a la respuesta).

**Envío para revisión:** 
Los entregables de este proyecto son la colección generada por Postman en formato .json, al igual que un archivo para las variables de ambiente, igual en formato .json.

Envío para revisión: 17 de Febrero


# Proyecto POM en Python
En este proyecto construiremos un framework de automatización desde cero siguiendo lo aprendido en la ruta de autoestudio de Python proporcionada al inicio de este módulo, así como también poner el conocimiento adquirido en las sesiones en vivo, con instructores presenciales, así como el apoyo de sus mentores. 

**Herramientas:**
- IDE: Pycharm
- Lenguaje: Python
- Test Runner: Pytest
- Framework de automatización: Appium

**Fecha de entrega: 24 de Febrero de 2023**

Se sugiere al estudiante familiarizarse con la aplicación saucedemo de manera que pueda replicar los casos de prueba a mano antes de proceder a automatizarlos. 

**Para que su proyecto sea aceptado, debe cumplir con los siguiente requisitos:**
- El proyecto debe iniciarse correctamente a través de los comandos vistos en clase. Esto significa que como resultado debe estar organizado en carpetas, páginas, datos, reportes, así como cualquier otra carpeta o archivo necesario para la ejecución y correcto funcionamiento del proyecto.
- Implementar el patrón de diseño Page Object Model (POM) y su correcta distribución de carpetas y archivos.
- Utilizar selectores que sean fáciles de leer, mantenibles, y cumpliendo con las mejores prácticas descritas.
- Hacer uso de “Fixtures” de manera que el código resultante se beneficie de esta funcionalidad. Utilice esta funcionalidad tanto como usted crea conveniente.
- Los casos de prueba deben de crearse de manera individual, es decir, no se permitirá que un caso de prueba “evalúe” dos funcionalidades distintas a la vez.
- Una vez creados los casos de prueba suficientes, se deberán diseñar los scripts que permitan correr las suites de pruebas de humo, así como la suite de regresión.
- Instalar y configurar una herramienta que permita el análisis de código estático de su proyecto (ejemplo: Flake8).
- Configurar una herramienta que permita generar un reporte después de la ejecución de los scripts. Dicho reporte deberá ser visual y proveer la información necesaria para la toma de decisiones por parte del negocio, es decir, no se aceptarán reportes en texto plano (ejemplo: Allure).
- Incluir toda la información necesaria (dependencias, configuraciones, notas, etcétera) de manera que cualquier persona pueda leer su archivo readme y pueda ejecutar su proyecto sin ningún problema.


**Los casos de prueba a implementar son los siguientes:**
- Inicio de sesión válido. Definir un caso de prueba que permita validar un inicio de sesión, las credenciales deben de estar almacenadas en un archivo aparte y leerse a través del uso de variables.
- Inicio de sesión incorrecto. Definir al menos tres casos de prueba negativos donde se permita el inicio de sesión al sitio web. Puede re-utilizar la función diseñada para el caso de prueba anterior.

# Proyecto de Appium
El propósito de este proyecto es construir un framework de automatización desde 0 siguiendo lo aprendido en la ruta de autoestudio de Python proporcionada al inicio de este módulo, así como también poner el conocimiento adquirido en las sesiones en vivo, con instructores presenciales, así como el apoyo de sus mentores. 

**Fecha de entrega: 02 de Marzo del 2022**

Se sugiere al estudiante familiarizarse con la aplicación saucedemo de manera que pueda replicar los casos de prueba a mano antes de proceder a automatizarlos. 

**Para que su proyecto de front-end sea aceptado como candidato de envío, debe cumplir con los siguiente requisitos**
- El proyecto debe iniciarse correctamente a través de los comandos vistos en clase. Esto significa que como resultado debe estar organizado en carpetas, páginas, datos, así como cualquier otra carpeta o archivo necesario para la ejecución y correcto funcionamiento del proyecto.
- Implementar el patrón de diseño Page Object Model (POM) y su correcta distribución de carpetas y archivos.
- Utilizar selectores que sean fáciles de leer, mantenibles, y cumpliendo con las mejores prácticas descritas.
- Los casos de prueba deben de crearse de manera individual, es decir, no se permitirá que un caso de prueba “evalúe” dos funcionalidades distintas a la vez.
- Una vez creados los casos de prueba suficientes, se deberán agregar las etiquetas correspondiente a los casos de prueba que permitan correr las suites de pruebas de humo, así como la suite de regresión.
- Los casos de prueba deberán encontrase divididos por archivos .feature de tal manera que estén agrupados según las funcionalidad que se esté probando
- Seguir estructura de Gherkin para los archivos tipo feature:
  - Background
  - Given
  - When
  - Then
- Los archivos de pantallas, pasos y datos deberán de tener el mismo nombre base para saber a qué pantalla se refiere. Por ejemplo:
  - Pantalla_principial_pantalla.py
  - Pantalla_principal_steps.py
  - Pantalla_principal_texts.py  
- Incluir toda la información necesaria (dependencias, configuraciones, notas, etcétera) de manera que cualquier persona pueda leer su archivo readme y pueda ejecutar su proyecto sin ningún problema.


**Los casos de prueba a implementar son los siguientes:**

- Detalle del artículo (Utilizar Scenario Outline para validar con 3 artículos). Una vez que ha iniciado sesión en el sistema, hacer tap sobre cualquiera de los artículos disponibles y proceder a validar la información relevante de dicho artículo (Nombre, descripción, precio).
- Agregar artículo al carrito de compras y validar que la información que se muestra sobre dicho artículo es correcta.  Considere evaluar atributos como nombre, precio, descripción, cantidad, etc, según usted considere conveniente.
- Finalizar compra. Una vez que ha agregado múltiples artículos a su carrito de compras, proceder a concluir el proceso de pago y envío. Validar que puede realizar una compra sin ningún problema.

**Opcional**

Realizar tap sobre el filtro que se encuentra en la esquina superior derecha de la página de productos, elegir la opción ordenar por precio de “menor a mayor” y validar que los artículos de la página en cuestión están correctamente ordenados.

# Enviando los entregables
Para publicar tu trabajo, deberás seguir estos pasos:

- Crear un pull request, apuntando a la rama master. La rama del pull request deberá tener la siguiente nomenclatura. <br>
* Folder: entregables>nombre_completo <br>
* 1er subfolder: API 
* 2do subfolder: POM 
* 3er subfolder: APPIUM <br>
* Folder: entregables>nombre_completo <br>
* 1er subfolder: API 
* 2do subfolder: POM 
* 3er subfolder: APPIUM

&nbsp;&nbsp;├── entregables <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── nombre_completo <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── API <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── POM <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├── APPIUM <br>

[Llenar este formato](https://forms.gle/Eq3NFcA1xusAgqfX8)
- Mantenerte al pendiente de la retroalimentación.
- Generar los cambios conforme a los comentarios de tu mentor.

