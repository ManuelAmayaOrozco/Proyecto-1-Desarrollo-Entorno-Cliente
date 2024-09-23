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

## Herramientas de programación

## Análisis de mercado
