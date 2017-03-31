La carpeta pintos/src/ contiene el código original del SO que se va a modificar.

Las carpetas y una explicación de su contenido es:

	- devices: Esta carpeta contiene el código fuente para la interconexión de los dispositivos de entrada/salida: teclado,temporizador, disco, etc.

	- filesys: Esta carpeta contiene el código fuente para un sistema de archivos básico.

	- lib: Esta carpeta contiene una implementación de un subconjunto de la biblioteca estandar de C. Tanto en el kernel de pintos, como en los programas de usuario, los headers que contiene esta carpeta puden ser incluidos usando la notacion #include<...>.

	- misc: Contiene patches e información para instalar y depurar PintOS

	- threads: Esta contiene el código fuenta para el kernel básico.

	- userprog: Aquí se encuentra el código fuente para cargar los programas de usuario y así poder ser ejecutados.

	- utils: Contiene archivos para utilizar PintOS en una computadora

	- vm: Esta carpeta está destinada para que dentro de ella se realice la implementacion de una memoria virtual.

Dentro de la carpeta threads/ encontramos los siguientes archivos:

	- flags.h:Macros que definen unos bits en el registro 80x86 de banderas 

	- init.c: El código dentro de este archivo permite la inicialización del kernel, include el main(), el programa principal del kernel.
	- init.h: Es el header el archivo init.c.

	- interrupt.c: Aquí se encuentra el código para el manejo básico de interrupciones y funciones para activar y desactivar interrupciones.
	- interrupt.h: Es el header del archivo interrupt.c.
	
	- intr-stubs.S: aquí está el código de ensamblaje para el manejo de interrupciones de bajo nivel.
	- intr-stubs.h: Es el header del archivo intr-stubs.S.

	- io.h: Aquí están las funciones para el acceso al puerto de Entrada/Salida. Es utilizado principalmente por los códigos fuente del directorio 'devices'.

	- kernel.lds.S: Es el script de enlace para vincular el kernel. Este establece la dirrecion de carga del kernel.

	- loader.S: Este es el cargador del kernel. El cual reúne 512 bytes de código y datos que el BIOS del PC carga en la memoria y que a su vez encuentra el kernel en el disco, lo carga en la memoria y salta a star() del archivo star.S
	- loader.h: Es el header del archivo loader.S

	- Make.vars: Variables de compilación

	- Makefile: Archivo con instrucciones para compilar

	- malloc.c: Contiene una simple implementación de malloc () y free () para el kernel, para la solicitud y liberación de memoria respectivamente.
	- malloc.h: Es el header del archivo malloc.c

	- palloc.c: Asignador de páginas, reparte la memoria en páginas de 4kb
	- palloc.h: Es el header del archivo palloc.c

	- pte.h: Contiene funciones y macros para trabajar con direcciones virtuales y entradas de la tabla de páginas.

	- start.S: Hace la configuración básica para la protección de memoria y operaciones de 32 bits en CPUs 80x86

	- switch.S: Contiene una rutina de lenguaje ensamblador para la conmutación de hilos.
	- switch.h: Es el header el archivo switch.S.

	- synch.c: Aquí se encuentran las primitivas básicas de sincronización: semáforos, bloqueos, variables de condición y barreras de optimización.
	- synch.h: Es el header del archivo synch.c.

	- thread.c: Este código brinda el soporte básico de hilos.
	- thread.h: Es el header del archivo thread.c

	- vaddr.h: Contiene funciones y macros para trabajar con direcciones virtuales y entradas de la tabla de páginas.

