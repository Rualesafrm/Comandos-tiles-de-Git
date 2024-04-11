<h1 align="center"> Guia de comandos útiles en Git </h1>
<a href="#"><img src="https://blog.desafiolatam.com/wp-content/uploads/2016/05/git-github-logo.jpg"></a>
<p align="justify">Este repositorio contiene una recopilación de comandos esenciales de Git que te ayudarán a dominar el control de versiones y la colaboración en proyectos de desarrollo de software. Ya sea que estés comenzando con Git o que desees mejorar tus habilidades, aquí encontrarás una guía práctica y fácil de seguir para navegar por las funcionalidades más comunes de esta poderosa herramienta.</p>
<h2 align="center"> Primero lo básico: Saber moverte en tu entorno</h2>
<p align="justify">Para empezar con nuestro repositorio, inicialmente debemos conocer como podemos movernos entre las carpetas es decir entrar o salir de ellas, como crear archivos o carpetas, tambien como mover o renombrar archivos y carpetas. Otras cosas que debemos saber es como mostrar todos los archivos que contiene la carpeta en la que estamos situados, entre otras cosas que veremos aqui que se pueden realizar.</p>
<h2> Comencemos:</h2>
<ul>
  <li><strong>cd nombrecarpeta : </strong>Sirve para moverme y entrar en una carpeta.</li>
  <li><strong>cd .. : </strong>Sirve para salir de la carpeta actual.</li>
  <li><strong>cd mkdir nombrecarpeta : </strong>Sirve para crear una carpeta con el nombre especificado en el directorio actual. </li>
  <li><strong>touch nombre_archivo.extension : </strong>Sirve para crear un archivo usando el comando touch seguido del nombre del archivo que deseas crear y con el punto(.) defino al extension del archivo.</li>
  <li><strong>ls : </strong>Sirve para mostrar todos los archivos en la carpeta actual.</li>
  <li><strong>mv : </strong>Mueve o renombra archivos y carpetas. Por ejemplo, mv archivo.txt Carpeta/ moverá el archivo "archivo.txt" a la carpeta "Carpeta".</li>
  <li><strong>cp : </strong>Copia archivos y carpetas. Por ejemplo, cp archivo.txt Carpeta/ copiará el archivo "archivo.txt" a la carpeta "Carpeta".</li>
  <li><strong>cat : </strong>Muestra el contenido de un archivo de texto. Por ejemplo, cat archivo.txt mostrará el contenido del archivo "archivo.txt".</li>
  <li><strong>pwd : </strong>Muestra la ruta del directorio actual.</li>
  <li><strong>clear : </strong>Limpia la pantalla del terminal o la ventana de la consola.(Si por alguna razon no te sirve y estas en Windows usa ctrl + L)</li>
</ul>
<p align="justify">⚠️Quiero dejarte algo claro, hay muchos mas comandos con muchas mas utilidades pero para iniciar, creeme esto son los mas importantes que vas a necesitar mientras vas aprendiendo⚠️.</p>
<h2 align="center"> Ahora que ya aprendiste lo básico, vamos a crear nuestro repositorio desde cero</h2>
<p align="justify">Ten en cuenta algo importante y es que para poder iniciar con esta serie de comandos primero debes haber establecido mediante tu consola de comandos o tu Git Bash la ubicación de tu carpeta donde vas a crear tu repositorio. Recuerda que eso lo haces con los comandos que vimos al inicio de esta guía.</p>
<p align="justify">Si tienes dudas de como hacerlo, simplemente abre tu consola de comandos o tu Git Bash que debe estar previamente instalado y coloca el siguiente comando:</p>
<p align="justify"><strong><code>cd D:/repositorio</code></strong></p>
<p align="justify">En este ejemplo estamos accediendo al Disco Local D: y estamos entrando en una carpeta que ya existe llamada "repositorio". Habran casos donde las carpetas tendran nombres con espacio u otro tipo de caracteres, notaras que al ejecutar este mismo comando pero usando solo la dirección de la carpeta no bastara, ya que obtendras un error. Para poder dar solucion basta con agregar comillas dobles al nombre de la carpeta("nombrecarpeta"). Es decir si mi carpeta se llama "repositorio JS" o "Desarrollo Web" deberas hacer lo siguiente:</p>
<p align="justify">Primero para no complicarte y liberarte de errores entra al Disco Local D:, eso lo hacemos de la siguiente manera:</p>
<p><strong><code>cd D:/</code></strong></p>
<palign="justify">Luego de que ya estas dentro de Disco Local D: y sabes que tu carpeta llamada "Desarrollo Web" esta ahi, haces lo siguiente:</p>
<p><strong><code>cd "Desarrollo Web"</code></strong></p>
<p align="justify">Bingo 👌, estas dentro de tu carpeta lista para ser nuestro nuevo repositorio.</p>
<p align="justify">Ahora para poder crear nuestro repositorio debemos segir los siguientes pasos:</p>
<ul>
  <li><strong>git init : </strong> Inicializa un repositorio de GIT en la carpeta donde se ejecute el comando.</li>
  <li><strong>git add nombrearchivo.extension (o tambien se puede colocar un punto(.) en vez del nombrearchivo para que se actualice todos los archivos en la carpeta) : </strong> Añade los archivos especificados al área de preparación (staging).</li>
  <li><strong>git config --global user.email tu@email.com : </strong> Configura un email.</li>
  <li><strong>git config --global user.name : </strong> Configura un nombre.</li>
  <li><strong>git commit -m “commit description” : </strong> Confirma los archivos que se encuentran en el área de preparación y los agrega al repositorio.</li>
  <li><strong>git status : </strong> Ofrece una descripción del estado de los archivos (untracked, ready to commit, nothing to commit).</li>
</ul>
<p align="justify">Este par de lineas de comando solo se usaran la primera vez que creamos desde cero nuestro repositorio, ya que nos ayudara a identificar y controlar quien ha hecho los cambios:</p>
<ul>
  <li><strong>git config --global user.email tu@email.com : </strong> Configura un email.</li>
  <li><strong>git config --global user.name : </strong> Configura un nombre.</li>
</ul>
<p align="justify">Estas otras lineas de comando son opcionales ya que nos serviran si necesitamos hacer alguna modificación:</p>
<ul>
  <li><strong>git commit -am “commit description” : </strong> Añade al staging area y hace un commit mediante un solo comando. (No funciona con archivos nuevos)</li>
  <li><strong>git rm (. -r, filename) (–cached) : </strong> Remueve los archivos del index.</li>
  <li><strong>git config --list : </strong> Lista las configuraciones.</li>
</ul>
<h2 align="center"> Excelente, nuestro siguiente objetivo es subir nuestro repositorio a GitHub</h2>
<p align="justify">Hemos avanzado mucho desde que iniciamos, ahora nuestra proxima tarea sera subir nuestro repositorio a la plataforma GitHub para poder compartirlo con las demas personas y poder trabajar en colaboracion con otros desarrolladores.</p>
<p align="justify">Bien, ahora debemos seguir una serie de pasos muy sencillos para lograrlo, te los enlisto a continuación:</p>
<ol>
<li><strong>Crear un repositorio en GitHub:</strong> Ve a la página principal de GitHub, inicia sesión en tu cuenta y haz clic en el botón "New" (Nuevo) en la esquina superior derecha para crear un nuevo repositorio. Dale un nombre al repositorio, elige si será público o privado, y opcionalmente agrega una descripción. Luego, haz clic en "Create repository" (Crear repositorio).</li>
<li><strong>Inicializar un repositorio local:</strong> Si aún no tienes un repositorio local para tu proyecto, inicializa uno en tu máquina local. Abre una terminal o línea de comandos, navega hasta el directorio donde tienes tu proyecto y ejecuta el 	siguiente comando para inicializar un nuevo repositorio Git:<br>
<code>git init</code></li>
<li><strong>Agregar archivos al repositorio local:</strong> Agrega los archivos y carpetas de tu proyecto al repositorio local usando el comando git add. Por ejemplo, para agregar todos los archivos y carpetas, puedes usar:<br>
<code>git add .</code></li>
<li><strong>Confirmar los cambios:</strong> Después de agregar los archivos, realiza un commit para confirmar los cambios en el repositorio local. Puedes hacerlo con el siguiente comando:<br>
<code>git commit -m "Mensaje de commit descriptivo"</code></li>
<li><strong>Conectar tu repositorio local a GitHub:</strong>En la página de tu repositorio en GitHub, copia la URL del repositorio remoto. Luego, en tu terminal, ejecuta el siguiente comando para agregar el repositorio remoto:<br>
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
<p>Excelente con esto que hemos hecho se subirá los cambios de tu rama local main al repositorio remoto en GitHub. Ahora si estas listo para compartir tu repositorio con las demas personas del mundo.</p>
<h2 align="center">Hagamos una pausa, quiero que pienses en lo siguiente</h2>
<p align="center"><a href="#"><img src="https://www.portafolio.co/files/article_new_multimedia/uploads/2017/09/11/59b6fefd616bf.jpeg" alt="Imagen" width="100%"></a></p>
<p align="justify">Quiero que entiendas lo poderoso de esta herramienta y los beneficios que te puede traer a ti como desarrollador ya que compartir tus repositorios en plataformas como GitHub te permite colaborar con otros desarrolladores, aumentar tu visibilidad en la comunidad, mantener un historial de cambios detallado, recibir feedback y revisión de otros, y contribuir al conocimiento colectivo al compartir tus proyectos y soluciones con la comunidad de desarrollo de software.</p>
<p align="justify">Imaginemos por un momento que tu quieres ser un Freelancer, hay varias plataformas donde tu puedes encontrar el trabajo remoto bien remunerado que todos queremos, pero necesitas mostrar que sabes hacer no importa si tiene experiencia o no, debes contar con un portafolio que demuestre tus conocimuientos para que seas un perfil atractivo para las empresas. Entonces adivina que?. Exacto ahi entra en juego tu repositorio que acabas de crear y subir para que otros vean tus trabajos por eso quiero que entiendas lo siguiente:</p>
<p align="justify">Tener tu propio repositorio en GitHub como freelancer es una jugada inteligente que puede transformar tu carrera. No solo es una ventana abierta a un mundo de oportunidades, sino que también es tu tarjeta de presentación en el universo digital. Al exhibir tu talento y proyectos en una plataforma tan influyente, te destacas entre la multitud, atrayendo clientes potenciales y colaboradores interesados. Además, es un arsenal de herramientas poderosas: te brinda el control de versiones para tus proyectos, facilita la colaboración con clientes y colegas, y te permite compartir tus innovaciones con la comunidad global de desarrolladores.<br><br>
Tu repositorio en GitHub no es solo un lugar para almacenar código, ¡es el epicentro de tu éxito como freelance en el mundo digital!</p>





