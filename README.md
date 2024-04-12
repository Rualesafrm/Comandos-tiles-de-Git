<h1 align="center"> Guia de comandos útiles en Git </h1>

<a href="#"><img src="https://blog.desafiolatam.com/wp-content/uploads/2016/05/git-github-logo.jpg"></a>

<p align="justify">Este repositorio contiene una recopilación de comandos esenciales de Git que te ayudarán a dominar el control de versiones y la colaboración en proyectos de desarrollo de software. Ya sea que estés comenzando con Git o que desees mejorar tus habilidades, aquí encontrarás una guía práctica y fácil de seguir para navegar por las funcionalidades más comunes de esta poderosa herramienta.</p>

<h2 align="center"> Primero lo básico: Saber moverte en tu entorno</h2>

<p align="justify">Para empezar con nuestro repositorio, inicialmente debemos conocer como podemos movernos entre las carpetas, es decir, entrar o salir de ellas, como crear archivos o carpetas, también como mover o renombrar archivos y carpetas. Otras cosas que debemos saber es como mostrar todos los archivos que contiene la carpeta en la que estamos situados, entre otras cosas que veremos aquí que se pueden realizar.</p>

<h2> Comencemos:</h2>

<ul>
  <li><strong>cd nombrecarpeta : </strong>Sirve para moverme y entrar en una carpeta.</li>
  <li><strong>cd .. : </strong>Sirve para salir de la carpeta actual.</li>
  <li><strong>cd mkdir nombrecarpeta : </strong>Sirve para crear una carpeta con el nombre especificado en el directorio actual. </li>
  <li><strong>touch nombre_archivo.extension : </strong>Sirve para crear un archivo usando el comando touch seguido del nombre del archivo que deseas crear y con el punto(.) defino la extensión del archivo.</li>
  <li><strong>ls : </strong>Sirve para mostrar todos los archivos en la carpeta actual.</li>
  <li><strong>mv : </strong>Mueve o renombra archivos y carpetas. Por ejemplo, mv archivo.txt Carpeta/ moverá el archivo "archivo.txt" a la carpeta "Carpeta".</li>
  <li><strong>cp : </strong>Copia archivos y carpetas. Por ejemplo, cp archivo.txt Carpeta/ copiará el archivo "archivo.txt" a la carpeta "Carpeta".</li>
  <li><strong>cat : </strong>Muestra el contenido de un archivo de texto. Por ejemplo, cat archivo.txt mostrará el contenido del archivo "archivo.txt".</li>
  <li><strong>pwd : </strong>Muestra la ruta del directorio actual.</li>
  <li><strong>clear : </strong>Limpia la pantalla del terminal o la ventana de la consola.(Si por alguna razón no te sirve y estás en Windows usa ctrl + L)</li>
</ul>

<p align="justify">⚠️Quiero dejarte algo claro, hay muchos más comandos con muchas más utilidades, pero para iniciar, créeme, esto son los más importantes que vas a necesitar mientras vas aprendiendo⚠️.</p>

<h2 align="center"> Ahora que ya aprendiste lo básico, vamos a crear nuestro repositorio desde cero</h2>

<p align="justify">Ten en cuenta algo importante y es que para poder iniciar con esta serie de comandos primero debes haber establecido mediante tu consola de comandos o tu Git Bash la ubicación de tu carpeta donde vas a crear tu repositorio. Recuerda que eso lo haces con los comandos que vimos al inicio de esta guía.</p>

<p align="justify">Si tienes dudas de como hacerlo, simplemente abre tu consola de comandos o tu Git Bash que debe estar previamente instalado y coloca el siguiente comando:</p>
<p align="justify"><strong><code>cd D:/repositorio</code></strong></p>

<p align="justify">En este ejemplo estamos accediendo al Disco Local D: y estamos entrando en una carpeta que ya existe llamada "repositorio". Habrá casos donde las carpetas tendrán nombres con espacio u otro tipo de caracteres, notaras que al ejecutar este mismo comando, pero usando solo la dirección de la carpeta, no bastara, ya que obtendrás un error. Para poder dar solución basta con agregar comillas dobles al nombre de la carpeta("nombrecarpeta"). Es decir, si mi carpeta se llama "repositorio JS" o "Desarrollo Web" deberás hacer lo siguiente:</p>

<p align="justify">Primero para no complicarte y liberarte de errores entra al Disco Local D:, eso lo hacemos de la siguiente manera:</p>
<p><strong><code>cd D:/</code></strong></p>

<p align="justify">Luego de que ya estás dentro de Disco Local D: y sabes que tu carpeta llamada "Desarrollo Web" está ahí, haces lo siguiente:</p>
<p><strong><code>cd "Desarrollo Web"</code></strong></p>

<p align="justify">Bingo 👌, estás dentro de tu carpeta lista para ser nuestro nuevo repositorio.</p>

<p align="justify">Ahora para poder crear nuestro repositorio debemos seguir los siguientes pasos:</p>

<ul>
  <li><strong>git init : </strong> Inicializa un repositorio de GIT en la carpeta donde se ejecute el comando.</li>
  <li><strong>git add nombrearchivo.extension (o tambien se puede colocar un punto(.) en vez del nombrearchivo para que se actualice todos los archivos en la carpeta) : </strong> Añade los archivos especificados al área de preparación (staging).</li>
  <li><strong>git config --global user.email tu@email.com : </strong> Configura un email.</li>
  <li><strong>git config --global user.name : </strong> Configura un nombre.</li>
  <li><strong>git commit -m “commit description” : </strong> Confirma los archivos que se encuentran en el área de preparación y los agrega al repositorio.</li>
  <li><strong>git status : </strong> Ofrece una descripción del estado de los archivos (untracked, ready to commit, nothing to commit).</li>
</ul>

<p align="justify">Este par de líneas de comando solo se usaran la primera vez que creamos desde cero nuestro repositorio, ya que nos ayudara a identificar y controlar quien ha hecho los cambios:</p>
<ul>
  <li><strong>git config --global user.email tu@email.com : </strong> Configura un email.</li>
  <li><strong>git config --global user.name : </strong> Configura un nombre.</li>
</ul>
<p align="justify">Estas otras líneas de comando son opcionales, ya que nos servirán si necesitamos hacer alguna modificación:</p>
<ul>
  <li><strong>git commit -am “commit description” : </strong> Añade al staging area y hace un commit mediante un solo comando. (No funciona con archivos nuevos)</li>
  <li><strong>git rm (. -r, filename) (–cached) : </strong> Remueve los archivos del index.</li>
  <li><strong>git config --list : </strong> Lista las configuraciones.</li>
</ul>
<h2 align="center"> Excelente, nuestro siguiente objetivo es subir nuestro repositorio a GitHub</h2>

<p align="justify">Hemos avanzado mucho desde que iniciamos, ahora nuestra próxima tarea será subir nuestro repositorio a la plataforma GitHub para poder compartirlo con las demás personas y poder trabajar en colaboración con otros desarrolladores.</p>

<p align="justify">Bien, ahora debemos seguir una serie de pasos muy sencillos para lograrlo, te los enlisto a continuación:</p>

<ol>
  <li><strong>Crear un repositorio en GitHub:</strong> Ve a la página principal de GitHub, inicia sesión en tu cuenta y haz clic en el botón "New" (Nuevo) en la esquina superior derecha para crear un nuevo repositorio. Dale un nombre al repositorio, elige si será público o privado, y opcionalmente agrega una descripción. Luego, haz clic en "Create repository" (Crear repositorio).</li>
  <li><strong>Inicializar un repositorio local:</strong> Si aún no tienes un repositorio local para tu proyecto, inicializa uno en tu máquina local. Abre una terminal o línea de comandos, navega hasta el directorio donde tienes tu proyecto y ejecuta el 	siguiente comando para inicializar un nuevo repositorio Git:<br>
  <code>git init</code></li>
  <li><strong>Agregar archivos al repositorio local:</strong> Agrega los archivos y carpetas de tu proyecto al repositorio local usando el comando git add. Por ejemplo, para agregar todos los archivos y carpetas, puedes usar:<br>
  <code>git add .</code></li>
  <li><strong>Confirmar los cambios:</strong> Después de agregar los archivos, realiza un commit para confirmar los cambios en el repositorio local. Puedes hacerlo con el siguiente comando:<br>
  <code>git commit -m "Mensaje de commit descriptivo"</code></li>
  <li><strong>Conectar tu repositorio local a GitHub:</strong> En la página de tu repositorio en GitHub, copia la URL del repositorio remoto. Luego, en tu terminal, ejecuta el siguiente comando para agregar el repositorio remoto:<br>
  <code>git remote add origin URL_DEL_REPOSITORIO_GITHUB</code><br><br>Reemplaza URL_DEL_REPOSITORIO_GITHUB con la URL que copiaste de GitHub.<br><br>
  <strong>Nota:<br></strong>
  Si ingresas mal el link o necesitas simplemente cambiarlo haces lo siguiente:<br><br>
  <strong>Verificar la URL remota actual:</strong> Puedes verificar la URL remota actual ejecutando el siguiente comando en Git Bash:<br>
  <code>git remote -v</code><br><br>
  <strong>Cambiar el link:</strong><br>
  <code>git remote set-url origin nueva_url</code><br><br>
  <strong>Volver a verificar el link:</strong><br>
  <code>git remote -v</code></li><br>
  <li><strong>Subir los cambios al repositorio remoto:</strong> Una vez que hayas conectado tu repositorio local a GitHub, puedes subir los cambios al repositorio remoto ejecutando el siguiente comando:<br>
  <code>git push -u origin main</code>(o tambien puede ser master depende como lo llames)<br><br>
  </li>
</ol> 

<p align="justify">Excelente con esto que hemos hecho se subirá los cambios de tu rama local main al repositorio remoto en GitHub. Ahora si estás listo para compartir tu repositorio con las demás personas del mundo.</p>

<h2 align="center">Hagamos una pausa, quiero que pienses en lo siguiente</h2>
<p align="center"><a href="#"><img src="https://www.portafolio.co/files/article_new_multimedia/uploads/2017/09/11/59b6fefd616bf.jpeg" alt="Imagen" width="100%"></a></p>

<p align="justify">Quiero que entiendas lo poderoso de esta herramienta y los beneficios que te puede traer a ti como desarrollador, ya que compartir tus repositorios en plataformas como GitHub te permite colaborar con otros desarrolladores, aumentar tu visibilidad en la comunidad, mantener un historial de cambios detallado, recibir feedback y revisión de otros, y contribuir al conocimiento colectivo al compartir tus proyectos y soluciones con la comunidad de desarrollo de software.</p>

<p align="justify">Imaginemos por un momento que tú quieres ser un Freelancer, hay varias plataformas donde tú puedes encontrar el trabajo remoto bien remunerado que todos queremos, pero necesitas mostrar que sabes hacer no importa si tiene experiencia o no, debes contar con un portafolio que demuestre tus conocimientos para que seas un perfil atractivo para las empresas. ¿Entonces adivina qué? Exacto ahí entra en juego tu repositorio que acabas de crear y subir para que otros vean tus trabajos, por eso quiero que entiendas lo siguiente:</p>

<p align="justify">Tener tu propio repositorio en GitHub como freelancer es una jugada inteligente que puede transformar tu carrera. No solo es una ventana abierta a un mundo de oportunidades, sino que también es tu tarjeta de presentación en el universo digital. Al exhibir tu talento y proyectos en una plataforma tan influyente, te destacas entre la multitud, atrayendo clientes potenciales y colaboradores interesados. Además, es un arsenal de herramientas poderosas: te brinda el control de versiones para tus proyectos, facilita la colaboración con clientes y colegas, y te permite compartir tus innovaciones con la comunidad global de desarrolladores.<br><br>
Tu repositorio en GitHub no es solo un lugar para almacenar código, ¡es el epicentro de tu éxito como freelance en el mundo digital!</p>

<h2 align="center">Muy bien, continuemos donde lo dejamos</h2>

<p align="justify">Ahora que ya conocemos como movernos entre carpetas usando la consola de comandos o el Git Bash, sabemos crear nuestro repositorio de forma local y subirlo a la plataforma de GitHub para que otros interactúen con él, quiero mostrarte algunos comandos que te ayudaran en tu trabajo: </p>

<h2>Analizar cambios en los archivos de un proyecto Git:</h2>

<p align="justify">Para lograr visualizar que cambios hemos hecho desde que se creó nuestro repositorio, disponemos de comandos tales como:</p>

<ul>
  <li><strong>git log : </strong>Lista de manera descendente los commits realizados.</li>
  <li><strong>git log --stat : </strong>Además de listar los commits, muestra la cantidad de bytes añadidos y eliminados en cada uno de los archivos modificados.</li>
  <li><strong>git log --all --graph --decorate --oneline : </strong>Este comando mostrará una representación gráfica y compacta de toda la historia del repositorio, con cada commit representado por una sola línea.</li>
  <li><strong>git show filename : </strong>Permite ver la historia de los cambios en un archivo.</li>
  <li><strong>git diff : </strong>Este comando compara los cambios entre el directorio de trabajo y el área de preparación (staging area), mostrando las diferencias entre los archivos que han sido modificados, pero no han sido aún añadidos al área de preparación.</li>
</ul>

<h2>Volver en el tiempo con reset, rm y checkout:</h2>

<p align="justify">¿Pero por qué decimos volver en el tiempo? Porque por ejemplo con git reset, puedes deshacer commits y moverte a un estado anterior del proyecto, conservando o eliminando cambios según lo necesites. Por otro lado, con git checkout, puedes explorar versiones anteriores del proyecto sin modificar la historia de cambios, simplemente cambiando temporalmente tu vista al estado de un commit específico. En esencia, estos comandos te permiten retroceder en el tiempo para entender, corregir o restaurar el estado de tu proyecto en momentos anteriores.</p>

<p>Asi que vamos a verlos a continuación:</p>

<ul>
  <li><strong>git reset --soft referencia : </strong>Este comando deshace el último commit, pero mantiene los cambios que habías realizado en el área de preparación (staging area), lo que te permite volver a confirmarlos con un nuevo mensaje de commit. (referencia: Puede ser un hash de commit, una rama, o una etiqueta, que especifica el commit al que deseas retroceder.)</li>
  <li><strong>git reset --hard referencia : </strong>En cambio, este comando deshace el último commit y borra todos los cambios posteriores realizados en el directorio de trabajo y el área de preparación. Los cambios se pierden permanentemente.</li>
  <li><strong>git checkout nombre_rama : </strong>Este comando se utiliza principalmente para cambiar entre ramas en Git. Al especificar el nombre de una rama, Git te llevará al estado de esa rama, actualizando tu directorio de trabajo y el estado del área de preparación para reflejar el estado de esa rama.</li>
  <li><strong>git checkout - : </strong>Este comando te permite cambiar entre la rama actual y la última rama en la que estuviste trabajando. Es útil para alternar rápidamente entre dos ramas. Además, si has realizado cambios en un archivo y luego has cambiado de rama sin confirmar esos cambios, <strong>git checkout - </strong> te permite volver al estado anterior del archivo antes de que realizaras esos cambios.</li>
</ul>

<p align="justify">Ahora exploraremos el comando <strong>git rm </strong>.</strong></p>
<p align="justify">Empecemos con <strong> git rm</strong> que tiene como funcion ayudar a eliminar archivos de Git sin eliminar su historial del sistema de versiones. Esto quiere decir que si necesitamos recuperar el archivo solo debemos “viajar en el tiempo” y recuperar el último commit antes de borrar el archivo en cuestión pero algo debemos tener muy en cuenta y es que git rm no puede usarse por sí solo, así nomás. 
<p align="justify">Por ejemplo para borrar una archivo usamos el comando:</p>
<code>git rm miarchivo.txt</code><br><br>  
<p align="justify">Se debe utilizar uno de los flags para indicar a Git cómo eliminar los archivos que ya no se necesitan en la última versión del proyecto:</p>
<ul>
  <li><strong>git rm --cached : </strong>Elimina los archivos del área de Staging y del próximo commit, pero los mantiene en nuestro disco duro.</li>
  <li><strong>git rm --force : </strong>Elimina los archivos de Git y del disco duro. Git siempre guarda todo, por lo que podemos acceder al registro de la existencia de los archivos, de modo que podremos recuperarlos si es necesario (pero debemos aplicar comandos más avanzados).</li>
</ul>
<h2>¿Que son las ramas en git?</h2>
<p align="justify">Las ramas en Git son líneas independientes de desarrollo que te permiten trabajar en diferentes características de tu proyecto de forma aislada. Cada rama tiene su propio conjunto de commits y cambios, lo que facilita la colaboración y la implementación de nuevas características sin interferir con el código principal.</p>
<p align="justify">En palabras mas sencillas al crear una nueva rama se copia el último commit en esta nueva rama. Todos los cambios hechos en esta rama no se reflejarán en la rama master hasta que hagamos un merge.</p>
<h2>¿Por que usar ramas?</h2>
<ul>
  <li><strong>Desarrollo paralelo: </strong>Las ramas te permiten trabajar en diferentes funcionalidades o correcciones de errores de forma simultánea sin afectar el código en otras ramas.</li>
  <li><strong>Experimentación segura: </strong>Puedes probar nuevas ideas o implementaciones en una rama separada sin afectar la estabilidad del código principal.</li>
  <li><strong>Colaboración:  </strong>Facilita la colaboración en equipo al permitir que múltiples desarrolladores trabajen en diferentes partes del proyecto al mismo tiempo.</li>
</ul>
<h2>Uso básico de ramas en Git</h2>
<p>Quiero mostrarte una guia de como puedes gestionar tus ramas en tus repositorios. Asi que empecemos:</p>
<ol>
  <li><strong>Crear una nueva rama: </strong><br><code>git branch nombre_de_la_rama</code><br><br>Esto crea una nueva rama con el nombre especificado pero no cambia a esa rama.</li>
  <li><strong>Cambiar a una rama existente o la que acabamos de crear: </strong><br><code>git checkout nombre_de_la_rama</code><br><br>Esto cambia tu directorio de trabajo y tu HEAD a la rama especificada, permitiéndote trabajar en esa rama.<br><br>
  Otra forma de hacer lo anterior pero en un solo paso es asi:<br><br><code>git checkout -b nombre_de_la_rama</code></li>
  <li><strong>Ver todas las ramas: </strong><br><code>git branch</code><br><br>Esto muestra todas las ramas en tu repositorio local y resalta la rama en la que te encuentras actualmente.</li>
  <li><strong>Eliminar una rama: </strong><br><code>git branch -d nombre_de_la_rama</code><br><br>Esto elimina la rama especificada. Ten en cuenta que no podrás eliminar una rama si tienes cambios que aún no han sido fusionados en otra rama.</li>
</ol>
<h2>Ejemplo de uso de ramas en Git:</h2>
<p align="justify">Supongamos que estás trabajando en un proyecto y deseas implementar una nueva funcionalidad llamada "nueva-caracteristica". Puedes seguir estos pasos:</p>
<ol>
  <li><strong>Crear una nueva rama para la nueva funcionalidad: </strong><br><code>git checkout -b nueva-caracteristica</code><br><br></li>
  <li><strong>Realizar los cambios necesarios y confirmarlos en la nueva rama: </strong><br><code>git add .</code><br><code>git commit -m "Implementar nueva característica"</code><br><br></li>
  <li><strong>Cambiar de nuevo a la rama principal (por ejemplo, main o master): </strong><br><code>git checkout main</code><br><br></li>
  <li><strong>Fusionar los cambios de la rama de la nueva característica en la rama principal: </strong><br><code>git merge nueva-caracteristica</code><br><br></li>
  <li><strong>Finalmente, eliminar la rama de la nueva característica si ya no es necesaria: </strong><br><code>git branch -d nueva-caracteristica</code><br><br></li>
</ol>
<h2 align="center">Sigamos con nuestro camino</h2>
<p align="justify">Este viaje ha sido genial , contamos con conocimientos suficientes para manejar y gestionar nuestros repositorios en Git y GitHub, pero espera aun falta algo muy importante y son los "Pull request"</p>
<p align="justify">Un Pull Request es una herramienta esencial en el mundo del desarrollo colaborativo que te permite proponer cambios en un proyecto de manera clara y organizada. Es una puerta abierta a la colaboración, donde puedes compartir tus ideas, recibir retroalimentación de colegas y asegurarte de que tus contribuciones se fusionen de manera segura en el código principal.</p>
<p align="justify">Espero que con esa breve descripcion que te acabo de proporcionar comprendas lo importante del asunto. Ahora te guiare a como hacer un pull request para que tengas los conocimientos necesarios para cuando lo necesites realizar en tu trabajo.</p>
<h2>¡Realicemos nuestro primer pull request!, Pero antes ten en cuenta esto 😅:</h2>
<p align="justify">Una buena práctica es mantener tu repositorio local sincronizado con el repositorio remoto antes de enviar un Pull Request. Esto garantiza que estés trabajando sobre la versión más reciente del código y evita conflictos innecesarios al momento de fusionar tu Pull Request.</p>
<p align="justify">Para sincronizar tu repositorio local con el repositorio remoto, puedes seguir estos pasos:</p>

<ol>
  <li><strong>Primero, revisa en que rama estás ubicado: </strong><br><code>git branch</code><br><br>Esto enumerará todas las ramas y indicará en verde la rama actual o activa.<br><br></li>
  <li><strong>Cambia a la rama maestra: </strong><br><code>git checkout master</code><br><br></li>
  <li><strong>Agrega el repositorio original como un repositorio upstream: </strong><br>Para poder extraer los cambios desde el repositorio original a tu versión local, necesitas agregar el repositorio Git original como un repositorio upstream.<br><code>git remote add upstream [HTTPS]</code><br><br>Aquí, [HTTPS] es el URL que debes copiar del repositorio del propietario.<br><br></li>
  <li><strong>Busca (fetch) el repositorio: </strong>Busca todos los cambios  del repositorio original. Las confirmaciones (commits) del repositorio original serán almacenadas en una rama local llamada upstream/master.<br><code>git fetch upstream</code><br><br></li>
  <li><strong>Fusionala: </strong><br>Fusiona los cambios de la rama upstream/master a tu rama maestra local. Esto hará que tu rama maestra se sincronice con el repositorio upstream sin perder tus cambios locales.<br><code>git merge upstream/master</code><br><br></li>
  <li><strong>Envía (push) los cambios a GitHub: </strong><br>En este punto tu rama local está sincronizada con la rama maestra del repositorio original. Si deseas actualizar el repositorio de GitHub, necesitas enviar tus cambios.<br><code>git push origin master</code><br><br></li> 
</ol>

<p align="justify">Excelente, ahora si!!😎</p>
  
<h2>¡Realicemos nuestro primer pull request!</h2>

<ol>
  <li><strong>Fork del repositorio: </strong>En GitHub, visita el repositorio al que deseas contribuir y haz clic en el botón "Fork" en la esquina superior derecha de la página. Esto creará una copia del repositorio en tu propia cuenta de GitHub.</li>
  <li><strong>Clona el repositorio: </strong><br>Ahora, clona tu repositorio forked (copiado) en tu máquina local utilizando el comando git clone.<br><code>git clone URL_de_tu_repositorio_forked</code><br><br></li>
  <li><strong>Crea una nueva rama: </strong><br>Cambia a una nueva rama donde realizarás tus cambios. Esto te permitirá trabajar de manera aislada sin afectar la rama principal del repositorio original.<br><code>git checkout -b nombre_de_tu_rama</code><br><br></li>
  <li><strong>Realiza los cambios: </strong><br>Haz los cambios necesarios en los archivos de tu proyecto en tu editor de código favorito.<br><br></li>
  <li><strong>Agrega y confirma los cambios:  </strong><br>Agrega los archivos modificados al área de preparación y confirma los cambios con un mensaje descriptivo.<br><code>git add .</code><br><code>git commit -m "Descripción de tus cambios"</code><br></li>
  <li><strong>Sube la rama al repositorio remoto:  </strong><br>Sube la nueva rama y los cambios asociados a tu repositorio forked en GitHub.<br><code>git push origin nombre_de_tu_rama</code><br><br></li>
  <li><strong>Crea el Pull Request en GitHub: </strong><br><ul>
  <li>Visita tu repositorio forked en GitHub.</li>
  <li>En la página principal de tu repositorio, cambia a la rama que acabas de subir.</li>
  <li>Haz clic en el botón "Pull Request" (o "Crear Pull Request").</li>
  <li>Selecciona la rama base (normalmente la rama principal) del repositorio original y la rama que acabas de subir desde tu repositorio forked.</li>
  <li>Proporciona un título y una descripción para el Pull Request, explicando los cambios realizados y por qué son necesarios.</li></ul><br></li>
  <li><strong>Solicita la revisión: </strong> Etiqueta a los colaboradores relevantes y solicita su revisión en el Pull Request. Esto les notificará y les permitirá dejar comentarios y realizar revisiones de código.</li>
  <li><strong>Espera la aprobación y fusión: </strong> Una vez que los cambios hayan sido revisados y aprobados, el propietario del repositorio original puede fusionar el Pull Request en su rama principal.</li>
</ol>
<p align="justify">Siguiendo estos pasos, podrás contribuir efectivamente a proyectos de código abierto o colaborar con tu equipo de desarrollo utilizando Pull Requests en GitHub.</p>







