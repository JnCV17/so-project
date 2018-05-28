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

![](imgs/cmv/captura_6.png)

* En el siguiente panel emergente vamos a la opción 'Red' y en la pestaña de 'Adaptador 2', habilitamos el adaptador de red. Después, en la opción 'Conectado a', seleccionamos aquella que dice 'Adaptador puente'. Finalmente seleccionamos la interfaz provistas por el computador y en nuestro caso seleccionaremos la interfaz inalambrica.

![](imgs/cmv/captura_7.png)

* Finalmente aceptamos la configuración y ejecutamos la máquina virtual.

![](imgs/cmv/captura_8.png)