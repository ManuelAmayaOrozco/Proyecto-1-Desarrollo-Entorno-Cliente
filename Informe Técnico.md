# Informe Técnico

## Modelos cliente/servidor

La arquitectura cliente-servidor consiste en la conexión de uno o varios clientes a un servidor especifico, que se encarga de proveer a los clientes con los servicios que estos soliciten.
Esto se realiza a través de una comunicación entre ambas partes, hecha de esta manera para poder diviir las funciones y otras responsabilidades entre capas, el cliente solicita un servicio al servidor a través de la red, al servidor luego responde tras procesar la solicitud, tras la cual este envia una respuesta al cliente, lo cual normalmente resulta en una salida por parte del cliente.

Algunas de las principales ventajas de este modelo son su facilidad para administrar datos y su seguridad, una escalabilidad superior que resulta muy actualizable y manejable, un mantenimiento por capas que ayuda a aislar problemas, mayor flexibilidad en el uso de aplicaciones y además el desarrollo es mucho menos dependiente, pudiendo separar el desarrollo en diversos proyectos que pueden controlar varios equipos.
Sin embargo, este modelo también posee ciertos inconvenientes, entre ellos el hecho de depender de una red para poder funcionar, una falla en el servidor puede causar inconvenientes para todos los clientes o hasta que el modelo deje de funcionar enteramente hasta que el error se soluciones y también el estar expuestos a la red trae posibilidad de más ciberataques.

Hay algunos tipos especificos de estos modelos, los cuales son los siguientes:

- **Arquitectura de dos niveles (2-Tier):** Es el modelo más habitual en el que los clientes realizan sus solucitudes directamente hacia el servidor sin ningún otro intermediario.
- **Arquitectura de tres niveles (3-Tier):** Al modelo anterior se le pueden añadir niveles adicionales, como en el caso del 3-Tier (pueden llegar a cualquier número de tiers, siendo así n-Tiers), en el que se añade un intermediario a la conexión entre el cliente y el servidor, normalmente para cumplir funciones de capa lógica de negocio, asi consiguiendo una mayor separación de responsabilidad y mejor fluidez, aunque esto conlleve a una mayor complejidad del código.

Toda la información de este segmento está sacada de esta [página](https://www.arsys.es/blog/todo-sobre-la-arquitectura-cliente-servidor).

## Lenguajes de programación

Como mencioné anteriormente, el lenguaje de programación principal que voy a utilizar será **Java**.

Java es uno de los lenguajes de programación a la hora de desarrollar aplicaciones web a fondo, siendo conocido por su robustez y su amplia comunidad, por lo que posee mucha documentación a cerca de su uso; es estable y con mucha escalabilidad, además de poseer una gran seguridad para sus datos (autenticación avanzada, control de acceso, encriptación, etc.). Al ser tan conocido y utilizado, Java también es compatible con un sinfin de bibliotecas, APIs y herramientas de desarrollo para todo tipo de proyectos. Aunque como todo, Java también tiene algunas desventajas a considerar, entre ellas su rendimiento más lento en comparación a otros lenguajes de programación, puede requerir más memoria que otros lenguajes de programación y también puede sobrecargar código en ciertos casos, por lo que hay que estar muy pendiente a ello para que no ocurra. 

Toda la información de este segmento está sacada de estas páginas ([mytaskpanel](https://www.mytaskpanel.com/java-soluciones-enterprise/#:~:text=Java%20es%20uno%20de%20los,la%20portabilidad%20y%20la%20escalabilidad.), [hubspot](https://blog.hubspot.es/website/ventajas-desventajas-java)).

## Compatibilidad en navegadores

La compatibilidad en navegadores se define básicamente en la capacidad de una página web para poder cargar y mantener su diseño original sin importar el tipo de navegador que se esté utilizando para abrir la página web, hoy en dia ya no hay tantos problemas en cuanto a esto como solía haber anteriormente, ahora es mayormente en cuanto a la capacidad de una página web de abrir en un teléfono móvil por ejemplo, ya que tiene características muy distintas en comparación a un ordenador habitual. Sin embargo, la compatibilidad entre navegadores sigue siendo un factor muy importante a tener en cuenta para que todo tipo de gente puede acceder a la página, aunque estén utilizando dispositivos anticuados. Para evitar estos problemas es importante hacer muchos testeos con diferentes navegadores, utilizar herramientas que puedan ayudar en el testeo y mantener en cuenta un análisis constante de los resultados.

Hay problemas particulares de compatibilidad que suelen ser muy comunes, estos son algunos ejemplos:

- **Validación de HTML y CSS:** La mayoria de las veces, el problema surge porque un navegador lee el código de la página de una manera distinta a otro, causando que esta no pueda cargarse o se vea de manera distinta, la mejor manera de lidiar con ellos es a través de herramientas de validación de código (Jigsaw CSS Validator, W3C HTML Validator, etc.)
- **Falta de Resets CSS:** Para que una página web utilice su propio diseño es necesario sobreescribir el predeterminado, lo cual causa que la página web se vea de manera distinta entre navegadores, lo mejor para evitar esto es añadiendo hojas de estilo de reset CSS (Normalize.css, HTML5Reset, etc.), las cuales se encargan de resetear la página web a su estado por defecto.
- **Error de DOCTYPE:** Prescindir del DOCTYPE suele causar errores de representación con facilidad, especialmente en navegadores más antiguos; siempre hay que mantener el código Doctype en la parte superior del código.

Otros problemas pueden ser causados por ciertos lenguajes de programación como JavaScript, que puede conllevar problemas si se usan funciones de versiones más modernas en navegadores antiguos, por ello es importante adaptar estas funciones dependiendo de los navegadores; por suerte esto mayormente ocurre en la programación front-end, lenguajes deprogramación back-end como Java se adaptan de mejor manera entre los diversos navegadores y puede ser entendido por casi todos los navegadores existentes, incluyendo versiones antiguas.

Toda la información de este segmento está sacada de estas páginas ([pedalo](https://www.pedalo.co.uk/browser-compatibility/), [comparium](https://comparium.app/es/blog/cross-browser-compatibility-issues/))

## Mecanismos de integración

El lenguaje de marcas pensado para este proyecto es HTML, comunmente utilizado por la gran mayoria de otras páginas web, este lenguaje es de marcado descriptivo, o sea, utiliza etiquetas para para describir los fragmentos de texto sin especificar su orden o como deben ser representados. HTML no tiene ningún problema a la hora de funcionar en los diferentes navegadores disponibles actualmente, incluso si llegan a ser antiguos. Para integrar apropiadamente Java en HTML hay diversas opciones:

- **Servlets y JSP:** Usando servlets (clases de Java que se ejecutan en un servidor web) y JavaServer Pages, los cuales son archivos HTML que pueden contener código Java sin problemas, permiten el uso de Java con HTML siempre que se usen conjuntamente, dejando que los JSP sean procesados por el servlet antes de ser enviados al navegador.
- **Frameworks y librerias:** Hay diversas librerias y frameworks que ayudan a integrar, como es el caso de Spring Boot que ayuda a desplegar webs Java y admite varias plantillas.
- **Componentes web y JavaScript:** Otra opción sería el uso de componentes web los cuales son reutilizables y personalizables, pudiendo encapsular el comportamiento y funcionalidad de Java, haciendo uso de JavaScript.

Toda la información de este segmento está sacada de estas páginas ([wikipedia](https://es.wikipedia.org/wiki/Lenguaje_de_marcado), [linkedin](https://es.linkedin.com/advice/1/how-can-you-integrate-java-html-css-skills-web-development-2ftle?lang=es))

## Herramientas de programación

Como herramientas de programación, estaré utilizando tanto **intelliJ** y **Visual Studio Code** para ayudarme a la hora de programar.

IntelliJ IDEA es un entorno de programación que es muy util a la hora de crear programas en lenguajes como Java o Kotlin. Es capaz de proveer plantillas prediseñadas, hacer tests de compatibilidad y depurar, su interfaz gráfica es simple y efectiva, ademas de que ayuda a la hora de corregir errores y permite instalar diferentes plugins que hará la experiencia aún más favorable.

Visual Studio Code es un editor de código que permite editar y crear cualquier tipo de código, es especialmente útil en programación front-end y lenguajes de marcado como HTML y CSS, también permite la depuración del código, gestionar diversos proyectos, integrar control de versiones a través de Git, permite extensiones y plugins, es eficiente, ágil y permite diversos frameworks con los que trabajar.

Toda la información de este segmento está sacada de estas páginas ([capterra](https://www.capterra.es/software/136010/intellij-idea), [arsys](https://www.arsys.es/blog/que-es-visual-studio-code-y-cuales-son-sus-ventajas))

## Análisis de mercado

No existen muchas otras páginas que se dediquen a proporcionar guias de videojuegos de manera eficiente, la mayoría se tratan de foros en los que la gente sube sus propias guias a base de texto, como por ejemplo [GameFAQs](https://gamefaqs.gamespot.com/) o [Game8](https://game8.co/); sin embargo, mi vision es para una guía más visual, con menos texto y que sea más parecido a poder crear tu propia lista de tareas para poder seguir tu propio progreso mientras juegas, además de poder compartirlo entre otros usuarios de la página para que ellos puedan también generar su propia versión de la plantilla, o simplemente mostrar su compleción del juego a todos los demás. Mi objetivo es crear algo nunca visto, y considero que al no existir ninguna página web parecida, tendria la ventaja de ser novedosa a pesar de tener competencia al ya existir otras páginas de guias.
