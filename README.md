<h1 align="center"> Guia de comandos útiles en Git </h1>
<p align="left"> <img src="https://blog.desafiolatam.com/wp-content/uploads/2016/05/git-github-logo.jpg"> </p>
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
<p>⚠️Quiero dejarte algo claro, hay muchos mas comandos con muchas mas utilidades pero para iniciar, creeme esto son los mas importantes que vas a necesitar mientras vas aprendiendo⚠️.</p>
<h2 align="center"> Ahora que ya aprendiste lo básico, vamos a crear nuestro repositorio desde cero</h2>
<p>Ten en cuenta algo importante y es que para poder iniciar con esta serie de comandos primero debes haber establecido mediante tu consola de comandos o tu Git Bash la ubicación de tu carpeta donde vas a crear tu repositorio. Recuerda que eso lo haces con los comandos que vimos al inicio de esta guía.</p>
<p>Si tienes dudas de como hacerlo simplemente abre tu consola de comandos o tu Git Bash que debe estar previamente instalado y coloca el siguiente comando:</p>
<p><strong>cd D:\repositorio</strong></p>
<p>En este ejemplo estamos accediendo al Disco Local D: y estamos entrando en una carpeta que ya existe llamada "repositorio". Habran casos donde las carpetas tendran nombres con espacio u otro tipo de caracteres, notaras que al ejecutar este mismo comando pero usando solo la dirección de la carpeta no bastara, ya que obtendras un error. Para poder dar solucion basta con agregar comillas dobles al nombre de la carpeta("nombrecarpeta"). Es decir si mi carpeta se llama "repositorio JS" o "Desarrollo Web" deberas hacer lo siguiente:</p>
<p>Primero para no complicarte y liberarte de errores entra al Disco Local D:, eso lo hacemos de la siguiente manera:</p>
<p><strong>cd D:\</strong></p>
<p>Luego de que ya estas dentro de Disco Local D: y sabes que tu carpeta llamada "Desarrollo Web" esta ahi, haces lo siguiente:</p>
<p><strong>cd "Desarrollo Web"</strong></p>
<p>Bingo 👌, estas dentro de tu carpeta lista para ser nuestro nuevo repositorio.</p>
<p>Antes que nada quiero que conozcas los comandos básicos para poder crear tu repositorio, los listare a continuación:</p>
<ul>
  <li><strong>git init : </strong> Inicializa un repositorio de GIT en la carpeta donde se ejecute el comando.</li>
  <li><strong>git add nombrearchivo.extension (o tambien se puede colocar un punto(.) en vez del nombrearchivo para que se actualice todos los archivos en la carpeta) : </strong> Añade los archivos especificados al área de preparación (staging).</li>
  <li><strong>git commit -m “commit description” : </strong> Confirma los archivos que se encuentran en el área de preparación y los agrega al repositorio.</li>
  <li><strong>git commit -am “commit description” : </strong> Añade al staging area y hace un commit mediante un solo comando. (No funciona con archivos nuevos)</li>
  <li><strong>git status : </strong> Ofrece una descripción del estado de los archivos (untracked, ready to commit, nothing to commit).</li>
  <li><strong>git rm (. -r, filename) (–cached) : </strong> Remueve los archivos del index.</li>
  <li><strong>git config --global user.email tu@email.com : </strong> Configura un email.</li>
  <li><strong>git config --global user.name : </strong> Configura un nombre.</li>
  <li><strong>git config --list : </strong> Lista las configuraciones.</li>
</ul>

