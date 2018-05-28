## Miniproyecto Sistemas Operativos

**Universidad ICESI**  
**Curso:** Sistemas Operativos  
**Docente:** Daniel Barragán C.  
**Tema:**  LXC/LXD Containers  
**Correo:** daniel.barragan at correo.icesi.edu.co

**Código:** AXXXXXXXXX  
**Nombre:** Juan Camilo Villada

**Código:** AXXXXXXXXX  
**Nombre:** Ándres Felipe Pérez

**Código:** A00054000  
**Nombre:** Jonatan Ordoñez Burbano

**Repositorio GitHub:** https://github.com/JonatanOrdonez/so-project/tree/so-project

## Aproviosionamiento básico de máquina virtual: instalación de sistema operativo, configuración de interfaces de red, minimo 4 núcleos
* Para instalar Ubuntu 16.04, creamos una nueva máquina virtual utilizando VirtualBox. Para ello, ejecutamos la aplicación y presionamos en el botón azul 'Nueva'. En el cuadro emergente le asignamos un nombre a nuestra máquina, en este caso nuestra máquina virtual se va a llamar ubuntu y presionamos en la opción 'Next'.

![](imgs/cmv/captura_1.PNG)

* Luego le asignamos aproximadamente 2GB de memoria RAM a nuestra máquina virtual y presionamos en 'Next'.

![](imgs/cmv/captura_2.PNG)

* Lo siguiente que hacemos es crear un espacio virtual para el disco duro de nuestra máquina, para ello seleccionamos la opción 'Crear un disco duro virtual ahora' y luego presionamos en 'Next'.

![](imgs/cmv/captura_3.PNG)

* En la siguiente ventana seleccionamos la opción 'Reservado dinamicamente' para que nuestro espacio virtual de disco duro crezca según su uso. Luego presionamos en 'Next'.

![](imgs/cmv/captura_4.PNG)

* En la siguiente pantalla le asignamos un espacio mínimo de capacidad de disco duro virtual a nuestra máquina. En este caso dejamos el valor por defecto que son 10GB. Finalmente presionamos en la opción 'Crear'.

![](imgs/cmv/captura_5.PNG)

* En la siguiente imagen podemos ver que nuestra máquina virtual se ha creado exitosamente. Ahora vamos a configurar nuestra interfaz de red seleccionando nuestra máquina y presionando en la opción 'Configuración'.

![](imgs/cmv/captura_6.PNG)

* En el siguiente panel emergente vamos a la opción 'Red' y en la pestaña de 'Adaptador 2', habilitamos el adaptador de red. Después, en la opción 'Conectado a', seleccionamos aquella que dice 'Adaptador puente'. Finalmente seleccionamos la interfaz provistas por el computador y en nuestro caso seleccionaremos la interfaz inalambrica.

![](imgs/cmv/captura_7.PNG)

* Finalmente, aceptamos la configuración y procedemos a ejecutar la máquina virtual. En el siguiente cuadro emergente indicamos la ruta donde se encuentra la ISO con S.O y presionamos en la opción 'Iniciar'.

![](imgs/cmv/captura_8.PNG)

* Como se puede ver en la siguiente imagen, debemos seleccionar el idioma de instalación de Ubuntu. Selecionaremos la opción 'Español' y luego en 'Instalar ahora'.

![](imgs/iu/captura_1.PNG)

* En la siguiente pantalla seleccionamos ambas opciones para instalar las actualizaciones de ubuntu y softwares de terceros para la compatibilidad del audio y video de nuestro computador. Luego presionamos en la opción 'Continuar'.

![](imgs/iu/captura_2.PNG)

* Debido a que se trata de una instalación limpia, selecionaremos la opción 'Borrar disco e instalar ubuntu' como se muestra en la siguiente imagen. Luego presionamos en 'Instalar ahora'.

![](imgs/iu/captura_3.PNG)

* En la siguiente ventana vamos a selecionar la ciudad donde nos encontremos, en nuestro caso vamos a escribir 'Bogota' y continuaremos con nuestra instalación.

![](imgs/iu/captura_4.PNG)

* A continuación, vamos a seleccionar la disposición de teclado. Por defecto, ubuntu detecta nuestra configuración que es 'Español (latinoamericano)'. Después de esto selecionamos la opción 'Continuar'.

![](imgs/iu/captura_5.PNG)

* En la siguiente pantalla vamos a crear un usuario para nuestro S.O. Vamos a indicarle que el nombre de la máquina sea 'operativos' al igual que el nombre de isuario y la contraseña.

![](imgs/iu/captura_6.PNG)

* Dejaremos que la instalación empiece y una vez finalice nos aparecerá un cuadro indicandonos que deberemos reiniciar la máquina. Después de reiniciar la máquina virtual iniciaremos sesión con nuestro usuario creado en el paso anterior.

![](imgs/iu/captura_7.PNG)

![](imgs/iu/captura_8.PNG)

![](imgs/iu/captura_9.PNG)

## Instalación de LXC/LXD con permisos para el usuario operativos
* Después de completar la instalación del sistema operativo ubuntu, vamos a ejecutar el siguiente comando para instalar el hypervisor LXD, el cual es un administrador de contenedores de linux y que sirve de complemento para LXC, añadiendo más funcionalidades y facilitando el uso de contenedores a través de comandos simples.

```Console
$ apt install lxd lxd-client
```

### ¿Qué es un storage pool?
* Un storage pool es la agrupación de varios discos SSD en un entorno de almacenamiento compartido, logrando que el sistema operativo vea todos estos disco como un solo disco grande. Cada disco que agregamos a un storage pool se particiona en cuatro segmentos y cada segmento de cada disco se agrupa con una partición de los otros discos creando un Raid Group, finalmente cada Raid Group recibe como nombre Allocation Unit.

### ¿Qué es ZFS?

## Bibliografía
* https://community.netapp.com/t5/Espa%C3%B1a/Storage-Pools/ba-p/99752