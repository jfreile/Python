## Contenido del curso

# Python
Análisis y visualización de datos
## TEMARIO
 ### Objetivo: 
 Desarrollar en los participantes dos nociones fundamentales para el desarrollo de sus actividades, este curso pretende abordar el frente de capacitación en 
 Python sobre los tópicos de Estadística y Procesamiento de datos en Python, en donde se desarrollarán las siguientes habilidades:
 * Manejo y modelación de datos textuales y numéricos en Python
 * Diseño de tópicos (temas) por documentos
 * Limpieza de Datos
 * Comprensión de documentos textuales
 * Análisis visual de datos para la toma de decisiones

## APLICACIONES
* kaggle: Your Machine Learning and Data Science Community --> https://www.kaggle.com/
* Python: lenguaje de programación --> https://www.python.org/downloads/release/python-3812/
* Anaconda: es un ambiente de trabajo para la ciencia de datos que permite hacer funcionar aplicaciones y administrar fácilmente distintos paquetes --> https://www.anaconda.com/products/individual
* Visual Studio Code: editor de código fuente --> https://code.visualstudio.com/download
* GIT: software de control de versiones --> https://git-scm.com/download/win

## EJEMPLOS

|Tema|Ejercicios|
|-----:|-----:|
|GIT| <ul><li> [Resumen y ejercicio con GIT y GITHUB](https://github.com/jfreile/Python/blob/main/Resumen_GIT.pdf) </li> 
|Python| <ul><li>[Instalacion de Extensiones](https://github.com/jfreile/Python/blob/main/Notebooks/Instalacion_Python.ipynb)</li><li>[Comandos basicos](https://github.com/jfreile/Python/blob/main/Notebooks/Ejemplo_comandos_Python.ipynb) </li><li>[Ejemplo con parametros de entrada](https://github.com/jfreile/Python/blob/main/Notebooks/Ejemplo_con_param_entrada.ipynb)</li><li>[Resumen](https://github.com/jfreile/Python/blob/main/Notebooks/Resumen_Python.ipynb)</li>
|Pandas|<ul><li>[Conceptos Basicos](https://github.com/jfreile/Python/blob/main/Notebooks/Introduccion_pandas.ipynb)</li><li>[Ejemplo con BD (archivo csv)](https://github.com/jfreile/Python/blob/main/Notebooks/Ejemplo_BD.ipynb) </li><li>[Ejercicios varios](https://github.com/jfreile/Python/blob/main/Notebooks/ejercicio_1_pandas.ipynb)</li><li>[Resumen](https://github.com/jfreile/Python/blob/main/Notebooks/Resumen_Pandas.ipynb)</li>|
|Estadistica| <ul><li> [Introducción a la estadistica](https://github.com/jfreile/Python/blob/main/Notebooks/Resumen_Estadistica.ipynb) </li> |
|Titanic|<ul><li> [Ejercicio con BD Titanic](https://github.com/jfreile/Python/blob/main/Notebooks/Ejemplo_BD_TITANIC.ipynb) </li> |

## INSTALACION Y CONFIGURACION DE PYTHON EN VISUAL STUDIO CODE
1. Instalar Visual Studio Code
2. Instalar Anaconda (ya viene con Python 3.8)
3. instalar las extensiones:
	- Python
	- Jupiter
	- R Extension
4. En VS Code sacar la paleta de comandos
	-  Menu/view/Command Palette 
	- (CTRL + Shift + P en Windows)
	Digitar Jupyter: Create new Jupyter notebook
5. Instalar las librerias requeridas para Python (en el notebook) digitar:
	- pip install pandas
		Si sale mensaje: Note: you may need to restart the kernel to use updated packages.
		!pip install --upgrade pandas
	- pip install numpy
		pip install --upgrade pip
		pip install --upgrade requests
	- pip install matplotlib
	- pip install seaborn
	- pip install empiricaldist
	- pip install missingno
	- pip install sklearn
	- pip install statsmodels
	- pip install seaborn
	- import pandas
	- pip install tensorflow
6. Instalar GIT para windows
7. crear cuenta de GitHub
8. Agregar extension R	

-- validar versiones instaladas
	- pip list

## GIT
	Ir a la carpeta del proyecto y se crea carpeta raiz:
	se debe ir a la carpta del proyecto y se crea carpeta raiz
    cd ruta
    mkdir mis_tareas (para crear una nueva carpeta)
    cd mis_tareas (para ingresar a dicha carpeta)
    git init (Para iniciar el git)
    * Autentificarnos
        * git config --global user.name "Jose Freile"
        * git config --global user.email "jose.freile@jep.gov.co" (debe coincidir con el correo en GITHUB)
        * git config --list (para listar el correo y usuario) 
        
    * Cree una llave ssh:
        Si es Windows: ssh-keygen -t rsa -b 4096 -C "jose.freile@jep.gov.co"
        > Enter a file in which to save the key (/c/Users/you/.ssh/id_algorithm):[Press enter]
        > Enter passphrase (empty for no passphrase): [Type a passphrase]        [Press enter]  
        > Enter same passphrase again:                [Type passphrase again]    [Press enter]    
        
        dicho archivo se guarda por defecto en la ruta --> ~/.ssh/id_rsa
        se debe agregar la llave SSH al agente ssh
            eval "(ssh-agent -s)"
            > Agend pid XXX
            ssh-add ~/.ssh/id_rsa
        se debe abrir el archivo: id_rsa.pub
 
	
### Comandos mas utilizados:
* ls -la           (para ver los archivos)
* ls -lh           (para ver los archivos de forma humana)
* touch jose.txt   (crea el archivo)
* vi jose.txt      (para abrir el editor de text vi y agregar contenido)
* git add jose.txt (para agregar el archivo al git)
* git commit -m "primer commit" (para agregar el archivo, el comentario y subir a la rama master)
* git show         (muestra el commit recientemente añadido y el texto modificado en el archivo)
* git log          (muesstra los commits agregados)
* cat jose.txt     (muestra el contenido del archivo)
* git reset --hard 6109fee68bb672eed854604cd1de5c9f32095966 (nombre del commit que se quiere eliminar)
* Autentificarnos:
	* git config --global user.name "Jose Freile"
	* git config --global user.email "jose.freile@correo.com"
	* git config --list (para listar el correo y usuario) 
* git push          (para subir al git hub)
	
* generar llave de encriptacion
	- ssh-keygen (para crear la carpeta .ssh)
	- ssh-keygen -t rsa -b 4096 -C "jose.freile@jep.gov.co"	

* evaluar el estado de la llave
	- start-ssh-agent.cmd
	
*Buscar archivo id_rsa.pub (llave de encriptacion)
	- ir a github, logearse, settings, ssh and GPG keys
	- agregar neva llave
	- titulo: pc personal
	- key: pegar clave
	- add ssh key
	
* luego de incluirse en el proyecto del profesional
	- pulsar boton code
	- clonar ssh y copiar
	
* git bash
	- ir al directorio donde se quiere dejar el proyecto (cd Desktop)
	- git clone (ruta del ssh)
	
* git branch (para verificar las ramas creadas)
* git branch jose_freile (para crear un branch con ese nombre)
* git checkout jose_freile (para pasarme al branch)
* git add Ejemplo.txt para subir archivo a la rama

* BAJAR CAMBIOS A LA RAMA DIF A MASTER
	* git checkout jose_freile  (ubicarse en la rama)
    * git merge master          (nombre de la rama a fusionarse y bajar los cambios)

* edicion del branch
	- mkdir mis_tareas (para crear una nueva carpeta)

* en vs code	
	- creo un arhivo, lo edito y lo guardo con nombre "Tarea1.txt"
	- en source control agregar comentario y subir el cambio	
	
## GITHUB con Visual Studio Code
### Requisitos
* Haber instalado y configurado Visual Studio Code (extension @builtin git)
* Haber instalado Git
* Cuenta en GitHub
* Tener un repositorio en GitHub

### GITHUB
 - Luego de crear la cuenta se debe generar una llave tipo SSH
 - Ingresar al perfil/setting/SSH and GPG key
 - title: ingresa titulo 
 - key: pegar clave previamente generada en GIT (id_rsa.pub)
 - add ssh key
 
 - Generar llave de encriptacion
    ssh-keygen (para crear la carpeta .ssh)
    ssh-keygen -t rsa -b 4096 -C "jose.freile@jep.gov.co"    
	
### CREACION REPOSITORIO REMOTO (GITHUB)
	En github, buscar opcion crear un nuevo repositorio (de forma publica, la privada tiene costo) 

### CLONACION REPOSITORIO DESDE GITHUB
	-- Pagina GITHUB
	- En GITHUB, se puede obteber la url haciendo clic en el botón "Clone or download".
	- ejemplo: https://github.com/jfreile/Python.git
	
	-- Maquina local
	Cree un directorio (en el pc) donde se guardarán los repositorios:
	Abra el directorio en Visual Studio Code (menú Archivo > Abrir carpeta ...):
	En Code abra la ventana de comandos con Ctrl+Mayús+p
	digite el comando --> git: clone 
	pegue la URL del repositorio: https://github.com/jfreile/Python.git
	escriba la ruta de destion en el pc
	
### COMANDOS EN VISUAL STUDIO CODE
	Luego de editar / crear / eliminar archivos se debe seleccionar la opcion "source control" donde se listan los archivos y sus cambios
	en la sección CAMBIOS, mostrará todos los archivos en los que ha realizado cambios.
		a la derecha de uno de los archivos verás 4 íconos. 
		* El primer  abrirá el archivo. 
		* El segundo icono revertirá los cambios en el archivo. 
		* El tercero "+" organizará los cambios. No podrá realizar commit con su repositorio local sin preparar sus cambios (staged changesl). 
		* El cuarto indicará el tipo de cambio en el archivo 
			M: el archivo se ha modificado. 
			A: archivo nuevo.
	Al marcar el archivo "+", se movera la sección "STAGED CHANGES- CAMBIOS POR ETAPAS".
	En la etapa de "STAGED CHANGES", Si decide no realizar el cambio, puede eliminarla de esta etapa haciendo clic en  "-", y el archivo se moverá de nuevo a la sección CAMBIOS.

###	CONFIRMAR CAMBIOS EN EL REPOSITORIO LOCAL
	Para continuar con la confirmación  local (commit) (lo estamos enviando a nuestro repositorio clonado localmente) haciendo clic en el icono “✓”.
		* se debe agregar un mensaje antes del commit explicando el motivo de los cambios.
		
###	CONFIRMAR CAMBIOS EN EL REPOSITORIO REMOTO - GITHUB
	En la parte inferior izquierda de Vs Code se ve:
		* una flecha apuntando hacia abajo con un cero al lado. Esta es una indicación de que no hay código en el repositorio remoto que deba descargarse localmente. 
		* La otra flecha apuntando hacia arriba con un 1 al lado es una indicación de que actualmente tenemos 1 confirmación que aún no se ha enviado al repositorio remoto.
	Para actualizar nuestro repositorio remoto con nuestros cambios, localice el icono "..." y haga clic en él. 
	Haga clic en el botón "Push" para enviar nuestros cambios al repositorio remoto.
	
	
### NOMENCLATURA:
	A - Added     (This is a new file that has been added to the repository)
	M - Modified  (An existing file has been changed)
	D - Deleted   (a file has been deleted)
	U - Untracked (The file is new or has been changed but has not been added to the repository yet)
	C - Conflict  (There is a conflict in the file)
	R - Renamed   (The file has been renamed)
	S - Submodule (In repository exists another subrepository)
	Push          (enviar nuestros cambios al repositorio remoto)
	pull          (descargar las actualizaciones del repositorio remoto al repositorio local)
	

## PYTHON 
Python es un lenguaje de programación multiparadigma: soporta parcialmente la orientación a objetos, programación imperativa y programación funcional

### EXTENSIONES
	- Pandas:     es una librería de Python especializada en el manejo y análisis de estructuras de datos
	- numpy :     es una librería de Python especializada en el cálculo numérico y el análisis de datos, especialmente para un gran volumen de datos.
	- seaborn:    es una librería de visualización de datos para Python.  Ofrece una interfaz de alto nivel para la creación de atractivas gráficas.
	- Matplotlib: es una biblioteca para la generación de gráficos a partir de datos contenidos en listas o arrays en lenguaje Python y su extensión matemática NumPy
	- time:       proporciona un conjunto de funciones para trabajar con fechas y/o horas
 	
### COMANDOS FRECUENTES

### INPUT
	caracter #                   --> Comenarios
	input("Valor X : ")  --> para solicitar ingresar valores

### PRINT
	print ("Hola")       --> para imprimir en pantalla
	print('{} grados {}'.format(c, f)) --> para imprimir con vbles 
	print(i, end=', ')  --> imprimir en una sola linea
	print('='*32)       --> imprime el caracter = 32 veces

	mensaje_1 = 'Hola '
	mensaje_2 = 'Jose'
	print(mensaje_1 + mensaje_2) --> impresion concatenada

### VARIABLES
	x  = 1              --> para crear y asignarle valores a una vble
	x += 1              --> aumenta en 1 la vble
	x = (30/4)          --> division sencilla
	x = (30//4)         --> division redondeada al proximo entero

### LISTAS - ARRAYS
	lista = []                --> crear lista vacia
	lista = list(range(1,10)) --> se crea una lista con los # del 1 al 10
	lista.append(i)           --> para agregar contenido a la lista
	nums = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16] --> llenado de forma manual
	indice = [(i, numero) for i, numero in enumerate(numeros)] --> lectura optimizada para leer una lista
	una_lista_optima = [nombre for nombre in nombreCompleto if len(nombre) >= 6]

### CICLOS
	for i in range(n-2,2,-1): --> for que va desde n-2, hasta 2, en mayor a menor
	for i in range(1, 1363): --> ciclo for que va desde 1 hasta 1363
	if i % 3 == 0:	     --> condicional if
	if i > 3: 
	pass              --> Se uiliza para seguir o saltar una condicón una vez se encuentre
	else :               --> si no
	print(i+1)
			
	while i < 10:        --> ciclo while
