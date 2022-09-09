# Node.js-Trucos (Linkedin)

*Introducción:
¿Ya estás trabajando con Node pero te encuentras que los ejemplos de tus libros no se parecen a los del mundo real? Si ya tienes las bases de Node y quieres ir más allá
de la teoría, este es el curso que estabas buscando. Este curso de LinkedIn Learning está cargado de consejos y trucos de Node que te ayudarán a ser más efectivo en tu 
trabajo diario. Sin importar que seas un desarrollar experimentado o apenas des tus primeros pasos en Node, tenemos algo para todos los niveles. Y hablaremos de casos, 
tareas y problemas comunes que solo aparecen cuando comienzas a crear proyectos en un entorno profesional. Vamos a llevar tu código al siguiente nivel. Exploraremos la 
configuración perfecta de tu entorno de trabajo. Trucos de optimización, herramientas para controlar y monitorear el uso de recursos de tus aplicaciones y hasta software 
avanzado de depuración, para que no se te escape el más minimo error. Soy Carlos Solís, autor y desarrollador. Y durante este curso voy a mostrarte todos mis trucos para 
crear aplicaciones. Ahórrate dolores de cabeza y reduce la curva de aprendizaje con este curso práctico de Node.

*Qué versión de Node elegir y cómo instalarla
Comencemos hablando sobre cómo descargar Node. Puede parecer la cosa más sencilla del mundo, pero si ya tienes tiempo trabajando en informática, sabrás que no importa lo 
sencillo que parezca, siempre tiene algún truco o algún detalle. Lo mismo ocurre con Node. Si entramos a la página nodejs.org, vamos a encontrar que nos ofrecen dos 
diferentes versiones. Esta es la primera elección que vas a tener que tomar. La versión LTS es la versión Long Term Support o la versión que va a tener soporte a largo 
plazo. Esta es la versión recomendada si estás trabajando en un proyecto grande que no necesite API particularmente nuevas y que tengas que asegurarte de que va a tener 
siempre disponibles parches de seguridad. En la versión más actualizada, en este caso, la versión 12.8, vamos a tener acceso a las últimas API. Si estás haciendo una 
aplicación que necesita en particular una API moderna, te recomiendo que utilices la versión actual. Puedes revisar dentro de este enlace que aparece en la parte 
inferior cuál va a ser el calendario de soporte. Por ejemplo, la versión 12 va a tener soporte hasta más allá del año 2022. Mientras que la versión 8 dejará de tener 
soporte en el año 2019. Así vas a tener un panorama claro de qué versión va a funcionar mejor dentro del proyecto específico en el que vas a trabajar. Pasemos a la 
sección de Descargas. Acá vas a tener una opción para cada sistema operativo. Asegúrate de utilizar la misma versión que utilizan todos los desarrolladores de tu equipo. 
¿Cómo saber cuál es la versión que estamos utilizando? Bueno, simplemente, después de instalar Node, busca en la terminal y escribe el comando node -v y vas a obtener la 
versión que está instalada en tu sistema. ¿Qué pasa si, por ejemplo, te solicitan instalar una versión diferente de la que aparece en tu sistema? Bueno, también tienes 
una opción dentro de la sección de Descargas. Simplemente, tienes que buscar por los lanzamientos anteriores o Previous Releases, y acá vas a tener todas las diferentes 
versiones de Node. Asegúrate, muy importante, de desinstalar completamente Node de tu sistema antes de instalar una nueva versión. No es una buena idea tener varias 
versiones de Node instaladas en el mismo sistema. Puedes tener resultados indeseables. Finalmente, si eres usuario de Mac, te recomiendo que no utilices el instalador 
que aparece en la página oficial y que busques una mejor opción, como la opción de Homebrew. En la dirección que está acá en pantalla puedes descargar Homebrew, 
simplemente, copiando este enlace dentro de la terminal y presionando Enter. Una vez que está instalado, Homebrew se va a encargar de todos los detalles de instalación 
para que quede perfectamente configurado dentro de tu sistema. Simplemente, tienes que incluir el comando brew install node, y así, vas a tener Node instalado dentro de 
tu sistema operativo.

*Configuración estandarizada de editores con editorConfig
Si trabajas en un equipo donde hay muchos desarrolladores, de seguro que ya te has encontrado que todos tienen diferentes gustos para elegir su editor de código. 
El asunto es que los diferentes editores de código tienen diferentes configuraciones por defecto, y vamos a encontrar inconsistencia en la forma en que anotamos 
nuestro código. Tenemos una solución para esto, y se llama EditorConfig. EditorConfig es un archivo que incluímos en la raíz de nuestro proyecto y que define la 
configuración que va a tener el editor. La mejor parte es que es compatible con la mayoría de los editores. Puedes encontrar más información en editorconfig.org. 
Y puedes encontrar acá la sintaxis de este archivo, así como los diferentes editores que están soportados. Posiblemente veas acá una imagen de tu editor favorito. 
Yo te voy a mostrar cómo configurarlo en Visual Studio Code. Yo aca tengo una aplicación donde estoy trabajando en Visual Studio Code y voy a incluir el archivo 
EditorConfig. Simplemente tengo que ponerlo en la raíz de mi aplicación:.editorconfig. Ese es el nombre que tiene que tener el archivo. Recuerda que tiene que 
comenzar con .editorconfig. Ahora, una vez que ya tenemos este archivo, tenemos que incluirle las diferentes reglas que vamos a aplicarle dentro de todos los 
documentos del proyecto. Acá, estoy utilizando el patrón general de sintaxis. Puedes encontrar más información en la página de EditorConfig, pero básicamente lo 
que estamos diciendo es que acá vamos a crear un patron universal que va a tener una serie de reglas. También podemos definirlo en archivos específicos, para que 
tenga diferentes reglas de acuerdo al lenguaje o al formato que estamos trabajando. Podemos hacer cosas como definir que la indentación siempre represente espacios 
o tabs. Esa discusión tienes que tenerla con los demás compañeros de tu equipo. En este caso, estamos definiendo que, cada vez que alguien haga una indentación, 
el editor automáticamente va a definir dos espacios. Voy a guardar mi archivo de configuración, y, antes, tengo que asegurarme de que tengo instalado una extensión 
que le va a dar soporte a esta configuración. Para eso, tengo que ir a la sección de Extensiones, en el caso de Visual Studio Code, y buscar una extensión que se 
llama Editor for VS Code. Una vez que está instalada, el sistema va a leer automáticamente la información que está en EditorConfig y va a aplicarla a la configuración
por defecto. Voy a abrir un documento de JavaScript y voy a definir un texto sin tener que hacer ningún detalle especial. Ahora voy a poner las llaves acá y voy a 
presionar Enter, es todo lo que voy a hacer. Y el sistema automáticamente va a poner dos espacios porque eso es lo que tiene definido por defecto en la configuración. 
Vemos que hay uno, dos espacios. Si yo quisiera cambiar esto, por ejemplo, me vengo acá al editorconfig, le digo que ya no quiero que sean dos espacios sino que sean 
cinco. Vamos a guardar, voy a abrir mi aplicación y, en este caso, nada más voy a presionar Enter. Y, como puedes ver, la indentación se está haciendo automáticamente 
de cinco espacios. La mejor parte es que una vez que yo ya tenga configurada todas las reglas para mi documento, le puedo enviar este archivo a los demás miembros del 
equipo y, en sus editores, van a aplicar exactamente las mismas reglas.

*Estandarización de formatos con la extensión Prettier
Un código consistente nos va a ayudar a ser mucho más eficientes y también a entendernos mejor entre los miembros de un equipo. Si todos tenemos exactamente el 
mismo formato, es mucho más fácil entender qué es lo que estamos haciendo. Además, a la hora de hacer un envío de nuestro código utilizando repositorios como Git, 
nos va ayudar a que enviemos menos cambios innecesarios porque todos vamos a tener exactamente el mismo formato. Te voy a mostrar cómo aprovechar este principio a 
través de una extensión que se encuentra disponible dentro de Visual Studio Code. Vamos a ir a la sección de Extensiones y vamos a buscar una extensión que se llama 
Prettier. Esta extensión nos ayuda a darle formato a nuestro código. Además de eso, te voy a mostrar un pequeño detalle para darle una configuración mucho más 
personalizada y también que todos los miembros del equipo pueden utilizar exactamente esa misma configuración. Acá yo estoy trabajando en un proyecto de Node y, 
como todos los proyectos de Node, tengo un archivo package.json. Voy a agregarle un valor adicional, que va a ser prettier. Y acá, le puedo definir propiedades de 
configuración a esta extensión. Lo que significa que si otro desarrollador está utilizando el mismo proyecto y tiene instalado Prettier, va a tener exactamente las 
mismas reglas que hemos definido acá. Yo ya tengo algunas reglas previamente escritas, y te las voy a explicar. Por ejemplo, acá estoy definiendo que en vez de 
utilizar tabs, utilicemos espacios. En caso de que desees la opcion opuesta, simplemente tienes que poner true, y automáticamente, el código, cuando se aplique el 
formato de Prettier, va a aplicar tabs. Vamos a mantenerlo ahora con espacios. También podemos definir con esta propiedad que se aplique el punto y coma, o semicolons. También podemos definir que en vez de utilizar comillas simples, se trabajen comillas dobles, y trabajar con diferentes formatos dentro de nuestro código. Ahora que ya tenemos formato definido, como queremos que trabaje Prettier, voy a ir acá, a mi código, y voy a poner una función que no va a tener ningún formato. Simplemente vamos a poner function test. Vamos a poner acá unos argumentos. Vamos a utilizar un formato bastante inconsistente. Por ejemplo, acá pongo muchos espacios, acá no pongo espacio, vamos a poner llaves, voy a poner una variable y la voy a poner con comillas simples, punto y coma, y voy a poner otra, que va a tener comillas dobles, sin punto y coma. Ahora, ¿cómo vamos a arreglar esto? Obviamente, cualquier desarrollador que se respeta, cuando ve este código, va a tener un problema cuando lo vean. Y, si otra persona lo revisa, posiblemente ni siquiera entienda qué es lo que está pasando. Pero entonces hacemos clic derecho, buscamos la opción Format Document y listo, ya tenemos nuestro código en el formato que nosotros queremos, con los espacios estandarizados, las comillas, los puntos y comas, y no tuve que hacer nada más. Así, antes de enviar nuestro código, simplemente le aplicamos este formato y vamos a tener resultados consistentes, no solo dentro de nuestro código, sino también a lo largo de todo el proyecto, con todos los miembros que participan en él.

*Prevención de errores con esLint y opciones de configuración
Prevenir errores a tiempo nos puede hacer muchísimo más eficientes. A todos nos ha pasado que una vez que ya tenemos una aplicación lista, la probamos, 
encontramos que tiene algún problema, pero es muy difícil identificar exactamente dónde está ocurriendo. Sería mejor que en el momento en que vamos escribiendo 
nuestro código encontremos esos pequeños errores que son los que generalmente nos quitan más tiempo. Te voy a mostrar cómo hacer eso con una simple herramienta 
llamada ESLint. Para hacer eso, yo acá tengo un proyecto de Node. Voy a instalar a través del npm, la herramienta ESLint. Esto le va a dar soporte a ESLint dentro 
de mi proyecto. Pero también como consejo te recomiendo que la instales de forma global. Entonces para hacer eso vamos a poner: npm install -g eslint. En este caso, 
lo estoy haciendo de las dos formas porque quiero que quede instalado dentro del proyecto, porque lo vamos a utilizar, pero también quiero que quede instalado en el 
sistema para que los diferentes editores puedan accederlo de forma más consistente. Vamos a presionar Enter, y esto va a instalarlo en ambas opciones. Mientras eso 
ocurre, vamos a ir al package.json y vamos a agregar algunos elementos específicos de configuración de ESLint. Afortunadamente, tenemos un formato que nos permite 
incluirlo dentro de este package.json, y así poder distribuir la misma configuración dentro de todos los miembros del equipo. Yo acá acabo de incluir la opción 
eslintConfig dentro de mi package.json y acabo de incluir, por ejemplo, la opción extends me permite acoplar eslintConfig con la extensión Prettier. También estoy 
definiendo algunas reglas como, por ejemplo, que me marque con errores si no incluyo un punto y coma o si no utilizo las comillas de acuerdo al formato que estamos 
trabajando en este proyecto. Voy a guardar, y ahora voy a abrir un archivo donde yo ya tengo la información que está definiendo mi código. Ahora que tengo instalado 
ESLint, voy a poder detectar los errores de formato en tiempo real. Por ejemplo, vamos a crear una tercera variable, en este caso, tenemos var test1, 2. Vamos a poner 
una variable que se llama test3. Pero, en este caso, le vamos a asignar un valor y se me va a olvidar incluirle el igual. Como puedes ver, acá me está apareciendo una 
línea roja, donde me dice que tenemos un error y que tengo que incluir el código correcto. De esta forma, cualquier pequeño error de sintaxis que tengamos, se va a ir 
detectando y marcando en nuestro código en tiempo real y nos va a ahorrar muchísimo tiempo, no solo a la hora de crear, sino también a la hora de detectar esos 
pequeños errores que son generalmente los que más tiempo nos toman en detectar.
